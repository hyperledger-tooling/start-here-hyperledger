---
layout: default
title: besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3615" class=".btn">#3615</a>
            </td>
            <td>
                <b>
                    rename premerge fork to paris, keep premerge as an alias
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
rename the merge fork to `paris`
keep `premerge` as an alias for paris 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #3608

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-19 14:52:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3611" class=".btn">#3611</a>
            </td>
            <td>
                <b>
                    [DO NOT MERGE] During Fast Sync execute World State Construction before Blocks Import
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Performance Test :
During Fast Sync execute World State Construction before Blocks Import

Signed-off-by: Ameziane Hamlat ameziane.hamlat@consensys.net

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 13:39:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3610" class=".btn">#3610</a>
            </td>
            <td>
                <b>
                    Tune transaction synchronization parameter to adapt to mainnet traffic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
This PR is composed of the tuning of some internal parameters related to the transaction synchronization.

1. Currently Besu handles hundreds of transaction message per seconds, so having a queue of 1M messages result in a lot of expired messages, make sense to reduce the capacity to drop incoming messages that could not be handled anyway.
2. Currently on mainnet there are many thousand of pending transactions exchanged between peers, but Besu has a short memory of what has been exchanged with a specific peer, with the result that the same transaction is often exchanged back and forth with the same peer, expecially when the peer is another Besu (below a sample of one transaction exchanged many time between peers) so it is necessary to remember more transactions seen with peers.
3. Added detailed information about exchanged transactions at trace log level.

This is a sample extraction from the trace logs of one transactions, peers `0x0b7cbef740d1af50cf`, `0xec1e73d0839ec87abe`, `0x364c56424b81989e57` are other Besus
[tx-sample.pdf](https://github.com/hyperledger/besu/files/8303223/tx-sample.pdf)


Running this patch on a 4 Besu nodes for some hours, showns that CPU and memory usage is significantly reduced
![image](https://user-images.githubusercontent.com/91944855/159009115-a5673f15-e722-4ac3-86d2-a65c1aa68848.png)


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->


<!-- Example: "fixes #2" -->
fixes #3524 
## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 09:31:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3607" class=".btn">#3607</a>
            </td>
            <td>
                <b>
                    Bugfix/stuck at ttd
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
* fix a corner case where besu does not recognize TTD block descending from TTD
* extend the distance that besu will 'look back' for TTD block in the case of a long period on non-finality post-merge
* added MergeCoordinator.addNewPayloadToSync to append newPayload to backward sync if we short circuit newPayloads early due to missing parent hash

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #3609

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 04:42:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3606" class=".btn">#3606</a>
            </td>
            <td>
                <b>
                    quorum ATs task does not depend on building docker image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

remove gradle dependency

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 04:25:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3604" class=".btn">#3604</a>
            </td>
            <td>
                <b>
                    [MINOR] add RPC method name to log for InvalidParams
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>
BEFORE
```
2022-03-18 13:38:22.593+10:00 | vert.x-worker-thread-0 | DEBUG | JsonRpcHttpService | Invalid Params
org.hyperledger.besu.ethereum.api.jsonrpc.internal.exception.InvalidJsonRpcParameters: Invalid json rpc parameter at index 1
Caused by: com.fasterxml.jackson.databind.exc.ValueInstantiationException: Cannot construct instance of `org.hyperledger.besu.ethereum.api.jsonrpc.internal.parameters.TraceTypeParameter`, problem: Invalid trace types supplied: foo
 at [Source: (String)"["foo","stateDiff"]"; line: 1, column: 19]
```
AFTER:
```
2022-03-18 13:38:22.593+10:00 | vert.x-worker-thread-0 | DEBUG | JsonRpcHttpService | Invalid Params for method: trace_rawTransaction
org.hyperledger.besu.ethereum.api.jsonrpc.internal.exception.InvalidJsonRpcParameters: Invalid json rpc parameter at index 1
Caused by: com.fasterxml.jackson.databind.exc.ValueInstantiationException: Cannot construct instance of `org.hyperledger.besu.ethereum.api.jsonrpc.internal.parameters.TraceTypeParameter`, problem: Invalid trace types supplied: foo
 at [Source: (String)"["foo","stateDiff"]"; line: 1, column: 19]
```

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 03:42:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3602" class=".btn">#3602</a>
            </td>
            <td>
                <b>
                    [MINOR] added toString for TraceTypeParameter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

so that logging can work properly

See https://github.com/hyperledger/besu/issues/3528

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-17 23:33:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3601" class=".btn">#3601</a>
            </td>
            <td>
                <b>
                    SNAPSYNC add request task
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">snapsync</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

PR that adds the different request tasks necessary for the snapsync as well as a utility to manage the ranges of requests 

Snapsyc is still an experimental feature more tests will be added when the feature will be completed

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-17 15:54:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3595" class=".btn">#3595</a>
            </td>
            <td>
                <b>
                    added download links for 22.1.2 and moved bonsai change to 22.1.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Added 22.1.3 section to changelog

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-16 09:23:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3594" class=".btn">#3594</a>
            </td>
            <td>
                <b>
                    change snapshot version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Frank Li <b439988l@gmail.com>

Change snapshot version to 21.1.3
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-16 05:59:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3592" class=".btn">#3592</a>
            </td>
            <td>
                <b>
                    address some sonar cloud bugs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

constants for strings and check some optionals.
Also changed the engineHttpUrl() method to use the engine host 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-16 05:14:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3591" class=".btn">#3591</a>
            </td>
            <td>
                <b>
                    Display data storage options in CLI help
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Diego López León <dieguitoll@gmail.com>

## PR description
This is a leftover from #3578 to display the new stable options in the `--help` output
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-16 04:52:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3590" class=".btn">#3590</a>
            </td>
            <td>
                <b>
                    Do not merge: test tuweni 2.2 RC
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Only for testing the tuweni 2.2 RC

Signed-off-by: Stefan Pingel <stefan.pingel@consensys.net>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-16 04:42:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3589" class=".btn">#3589</a>
            </td>
            <td>
                <b>
                    Release 22.1.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-16 04:30:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3585" class=".btn">#3585</a>
            </td>
            <td>
                <b>
                    Add group heading to command options
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

This PR continues to group the CLI options together.

- JSON-RPC HTTP
- JSON-RPC WebSockets
- Metrics
- Miner
- Privacy
- Permissions
- Tx poo

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
fixes #2757 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-15 10:30:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3580" class=".btn">#3580</a>
            </td>
            <td>
                <b>
                    [MINOR] corrections to changelog and typos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Fixed some typos including in the CHANGELOG

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-14 01:40:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3579" class=".btn">#3579</a>
            </td>
            <td>
                <b>
                    WebSocket batch test - remove Ignore
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-13 23:43:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3578" class=".btn">#3578</a>
            </td>
            <td>
                <b>
                    Remove -x flag for bonsai CLI options
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Frank Li <b439988l@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Removes -X from the bonsai flags so users feel safer using the options as bonsai have been tested extensively, note forest will still be the default storage format.

## Changelog
Add to breaking changes (should we support the -X flag for a little longer?)

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-13 23:37:42 +0000 UTC
    </div>
</div>

