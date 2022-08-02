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
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/340" class=".btn">#340</a>
            </td>
            <td>
                <b>
                    Reduce staticcheck warnings (S1000)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As part of issue #50, removed warnings related to:
* S1000: removed redundant single-case selects for channels

Signed-off-by: Alexandros Filios <alexandros.filios@ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-02 12:11:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/336" class=".btn">#336</a>
            </td>
            <td>
                <b>
                    Enable staticcheck via make checks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Runs staticcheck with `make checks`.

Currently, this is supposed to fail via CI until #50 is resolved.

Signed-off-by: Marcus Brandenburger <bur@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-02 07:06:57 +0000 UTC
    </div>
</div>

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
                <span class="chip">cleanup</span>
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

