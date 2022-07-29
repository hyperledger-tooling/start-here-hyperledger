---
layout: default
title: fabric-smart-client
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-smart-client
---

# fabric-smart-client <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-smart-client){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/334" class=".btn">#334</a>
            </td>
            <td>
                <b>
                    Reduce staticcheck warnings (SA1019)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As part of issue #50, removed warnings related to:
* SA1019: replaced deprecated protobuf with an adapter package

Signed-off-by: Alexandros Filios <alexandros.filios@ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-29 10:25:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/333" class=".btn">#333</a>
            </td>
            <td>
                <b>
                    Add mbrandenburger to maintainers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Marcus Brandenburger <bur@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-29 09:55:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/332" class=".btn">#332</a>
            </td>
            <td>
                <b>
                    Reduce staticcheck warnings (ST1001)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As part of issue #50, removed warnings related to:
* ST1001: should not use dot imports (excluded assertion-related packages)

Signed-off-by: Alexandros Filios <alexandros.filios@ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-29 07:46:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/330" class=".btn">#330</a>
            </td>
            <td>
                <b>
                    KVS extensions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Return the key when iterating 
- Add support function for splitting keys
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-28 07:12:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/329" class=".btn">#329</a>
            </td>
            <td>
                <b>
                    Issue50 reduce staticcheck issues - Not for review
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
        Created At 2022-07-27 12:53:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/328" class=".btn">#328</a>
            </td>
            <td>
                <b>
                    Reduce staticcheck warnings (SA1019)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As part of issue #50, removed warnings related to:
* SA1019: removed deprecated grpclog.SetLogger and ptypes

Signed-off-by: Alexandros Filios <alexandros.filios@ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-27 09:36:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/325" class=".btn">#325</a>
            </td>
            <td>
                <b>
                    Reduce staticcheck warnings (ST1019, S1023)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As part of issue #50, removed warnings related to:
* ST1019: imported more than once

Signed-off-by: Alexandros Filios <alexandros.filios@ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-26 12:51:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/324" class=".btn">#324</a>
            </td>
            <td>
                <b>
                    Optimize msp cache
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Applying changes from https://github.com/hyperledger-labs/fabric-token-sdk/pull/304

Signed-off-by: Marcus Brandenburger <bur@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-26 12:10:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/323" class=".btn">#323</a>
            </td>
            <td>
                <b>
                    Remove GetCachedStateRangeScanIterator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Remove GetCachedStateRangeScanIterator
- Badger autoclean
- Add simple badger benchmark

Signed-off-by: Marcus Brandenburger <bur@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-26 11:25:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/322" class=".btn">#322</a>
            </td>
            <td>
                <b>
                    Reduce staticcheck warnings (ST1005)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As part of issue #50, removed warnings related to:
* ST1005: error string format

Signed-off-by: Alexandros Filios <alexandros.filios@ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-26 10:59:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/321" class=".btn">#321</a>
            </td>
            <td>
                <b>
                    Removed simple gogo/protobuf/proto dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As part of issue #174, replaced most dependencies of gogo/protobuf/proto with golang/protobuf/proto. The remaining occurrences reside in p2p.go and their removal requires handling of the dependency from the package gogo/protobuf/io.

Signed-off-by: Alexandros Filios <alexandros.filios@ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-25 13:19:43 +0000 UTC
    </div>
</div>

