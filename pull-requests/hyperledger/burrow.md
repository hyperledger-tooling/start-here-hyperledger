---
layout: default
title: burrow
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/burrow
---

# burrow <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/burrow){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/burrow/pull/1491" class=".btn">#1491</a>
            </td>
            <td>
                <b>
                    Fix collisions in ABI output, submit contract metadata on deploy, remove GRPC dependencies from codegen interface.gd.ts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Switched to a hierarchical bin folder to only require contract names
to be unique within their own directory
- Send contract ABIs to Burrow from codegen deploy function
- Remove dependency on GRPC types to improve ergonomics and not couple
GRPC codegen to the provider interface hopefully to give better
compatibility between versions
- Use duck-typed interface for CancelStreamSignal so that cancel signal
is not path dependent (for compatibiltiy between multiple Burrow
versions where possible in same project)

Signed-off-by: Silas Davis <silas@monax.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-26 17:21:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/burrow/pull/1490" class=".btn">#1490</a>
            </td>
            <td>
                <b>
                    Return bytesNN as Buffer and inline sources
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Silas Davis <silas@monax.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-24 12:08:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/burrow/pull/1489" class=".btn">#1489</a>
            </td>
            <td>
                <b>
                    Fix finitely bounded event streams in the presence of empty blocks.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ExecutionEventsServer assumes every block will be represented in
state, but this is not true for empty blocks.

Signed-off-by: Silas Davis <silas@monax.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 15:20:50 +0000 UTC
    </div>
</div>

