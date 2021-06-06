---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/287" class=".btn">#287</a>
            </td>
            <td>
                <b>
                    Release 0.18.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-02 15:29:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/285" class=".btn">#285</a>
            </td>
            <td>
                <b>
                    Require storage_credentials and storage_config wallet parameters to be Strings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previous refactoring has allowed `storage_credentials` and `storage_config` to be passed as Object - that would however end up in error on lower indy layers. This is PR is tightening the validation, so if `storage_credentials`, `storage_config` are not strings, it will throw early, on aries-vcx layer.

Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-02 10:06:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/284" class=".btn">#284</a>
            </td>
            <td>
                <b>
                    Rebuild Cargo.lock
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-31 12:47:46 +0000 UTC
    </div>
</div>

