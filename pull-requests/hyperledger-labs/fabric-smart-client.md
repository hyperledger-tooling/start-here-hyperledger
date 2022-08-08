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

