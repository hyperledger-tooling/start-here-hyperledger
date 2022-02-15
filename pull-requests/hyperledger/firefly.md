---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/501" class=".btn">#501</a>
            </td>
            <td>
                <b>
                    Re-work batch logic for simplicity, efficiency, and restart recovery
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This leads on from the investigation in #421 and then #499

At the moment this is how the batching logic works:

## OLD

![batch_logic](https://user-images.githubusercontent.com/6660217/150621839-468e5be6-e1b5-4ac6-8086-34b4b9d73281.jpg)

- The assembly loop of each batch dispatcher is able to keep accepting work as long as the last batch has been successfully dispatched.
- The assembly loop passes work to the persistence loop, which has as many slots in its channel input as there are slots in the batch.
- The persistence loop keeps continually recording data to the database.
- The offset on the batch manager that's reading from the messages queue, is updated as soon as the assembly loop picks up the message

This design evolved from a similar design in the previous generation of Asset Trail technology.

Given this most recent issue, and some inefficiency and crash recovery challenges that exist in the design after it's port over to FireFly and evolution, I'm planning an updated design.

## NEW

This PR updates it to simplify it (even beyond the previous proposal in #421):

![batching_v2](https://user-images.githubusercontent.com/6660217/153135529-e81ff098-5266-44df-8021-849af7882fd2.jpg)

- We remove two of the loops
- Persistence only happens once for each batch in the final stage when the batch is sealed
- Dispatching is synchronous to the assembler
- The assembler only allows one batch to be in assembly before it blocks waiting for the dispatch completion
- The batch manager just has in-memory offset state, and on restart it looks from time-zero again
- We introduce a new `sent` state for messages that go into a batch
- Anything that doesn't reach that state is eligible for re-send after restart (at least once delivery)
- The manager can rewind at any time, because everything will either:
  - Be persisted with a batch ID so skipped
  - Be already in-flight
- The processor keeps track of sequences its flushing, and does duplicate detection
- The processor orders the assembly batch in sequence order


Note this means if things are appearing at once across a batch assembly window of 0.5s, it's very likely all messages will be sent in DB sequence order (even though the DB doesn't guarantee that's the order they'll become visible in).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 06:38:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/498" class=".btn">#498</a>
            </td>
            <td>
                <b>
                    Misc fixes for operations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Ensure the operations for tokens and custom contracts behave as expected in success/failure scenarios.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 22:08:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/497" class=".btn">#497</a>
            </td>
            <td>
                <b>
                    Pass requestId to DX and remove backend_id from Operation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Follow the convention of all other plugins by passing a request ID into the
connector, rather than reading one from the connector response. This will be
enforced as a requirement for future connectors, so backend_id is removed from
the operations table.

Depends on https://github.com/hyperledger/firefly-dataexchange-https/pull/54
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 17:44:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/496" class=".btn">#496</a>
            </td>
            <td>
                <b>
                    Rewind when messages appear behind offset
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix for #493 

Observed reviewing the logs for #493 that the messages were never being picked up by the batch processor, and the perf tool is submitting them in a highly parallel way. My analysis is that with PSQL as used in this test (or any production ready database) parallel writing of messages to the DB could result in the commit order of the transactions, being mismatched with the sequence allocation to the rows. 

The code in the batch manager did not handle this - it would simply do a shoulder tap to re-read from the DB when a message was created, but not check if that message had appeared behind the offset and it needed to do a rewind.

This code change implements a simple rewind (like we have for the event aggregator).
Note this means that in the case of parallel REST API submission of messages, the final delivery order might not match the local sequence order. However, that's in-line with the assurances FireFly provides - as application should only be able to depend on.

- The local order they submitted in (in this case there is parallel submission, so the order is not deterministic) - but they should only rely on this for their own participation, and cannot consider this the global order across participants.
- The final order as ordered by the blockchain, when pinning is used.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 17:16:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/495" class=".btn">#495</a>
            </td>
            <td>
                <b>
                    Pass arguments from Makefile to docker build script
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This should fix the failing docker latest / release builds after we merge PRs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 16:09:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/494" class=".btn">#494</a>
            </td>
            <td>
                <b>
                    Compile directly with solc to avoid full Node.js npm install of Truffle
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Saves a lot of time and I/O activity during the docker build.

The `jq` command converts the `combined.json` output from `solc` in this syntax of JSON required by the CLI (which is a subset of the Truffle output):
https://github.com/hyperledger/firefly-cli/blob/680665495e45074b250e5ed5a74e8f152774254c/pkg/types/ethconnect.go#L19-L23
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 15:39:37 +0000 UTC
    </div>
</div>

