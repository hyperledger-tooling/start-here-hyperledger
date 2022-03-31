---
layout: default
title: fabric-gateway
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-gateway
---

# fabric-gateway <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-gateway){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/421" class=".btn">#421</a>
            </td>
            <td>
                <b>
                    Fix CodeQL scan of Java client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Autobuild was insufficient for Java as the compiled protos are required.

Signed-off-by: Mark S. Lewis <Mark.S.Lewis@outlook.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-26 09:32:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/419" class=".btn">#419</a>
            </td>
            <td>
                <b>
                    Refactor Go checkpointing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Filename capitalisation corrections.
- Additional godoc.
- Hold an open file handle in a FileCheckpointer instead of open/write/close on every save, giving orders of magnitutude better I/O performance.
- Include Close() method for FileCheckpointer to close file handle after use.
- Add option to Sync() FileCheckpointer to reduce risk of data loss at significant I/O performance cost.
- Simplify InMemoryCheckpointer API instead of keep it common with FileCheckpointer
- Remove Checkpointer interface from public API as it was never used.

Signed-off-by: Mark S. Lewis <mark_lewis@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-26 00:04:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/418" class=".btn">#418</a>
            </td>
            <td>
                <b>
                    Explicit typing of StatusCode in Node API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The typing implicitly referenced a protobuf stub and produced no detail on the type members in the tsdoc output. Add explicit type definition so the tsdoc includes all the field names and corresponding values.

Signed-off-by: Mark S. Lewis <mark_lewis@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-25 15:11:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/417" class=".btn">#417</a>
            </td>
            <td>
                <b>
                    WIP:Checkpointer implemention in java 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: sapthasurendran <saptha.surendran@ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-25 10:22:46 +0000 UTC
    </div>
</div>

