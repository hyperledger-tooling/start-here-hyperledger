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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/416" class=".btn">#416</a>
            </td>
            <td>
                <b>
                    Update Java dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Only run Checkstyle with Java 11+ as v10 does not support earlier Java versions.
- Run dependency vulnerability scan plugin directly for improved performance.
- Store vulnerability scan results as a build artifact.

Signed-off-by: Mark S. Lewis <mark_lewis@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-23 21:09:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/415" class=".btn">#415</a>
            </td>
            <td>
                <b>
                    Additional staticcheck and gofmt checks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Removal of the deprecated golint left some gaps in checking for correct godoc comments and recommended naming. Enabling additional (non-default) staticcheck rules covers at least some of these linting gaps.

Added a check of all Go files with gofmt to ensure recommended formatting.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-23 12:03:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/414" class=".btn">#414</a>
            </td>
            <td>
                <b>
                    file checkpointer for go
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
        Created At 2022-03-23 08:14:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/413" class=".btn">#413</a>
            </td>
            <td>
                <b>
                    Use @hyperledger/fabric-protos package in Node client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Use compiled protobuf and gRPC service stubs from @hyperledger/fabric-protos package instead of compiling and embedding within the fabric-gateway package.

Work-in-progress: Currently bundling proposed @hyperledger/fabric-protos package within fabric-gateway as a proof-of-concept.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-19 16:15:08 +0000 UTC
    </div>
</div>

