---
layout: default
title: fabric-operations-console
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-operations-console
---

# fabric-operations-console <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-operations-console){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/94" class=".btn">#94</a>
            </td>
            <td>
                <b>
                    fix commit flow - org without signature
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Varad Ramamoorthy <varad@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-30 22:21:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/93" class=".btn">#93</a>
            </td>
            <td>
                <b>
                    prevent setting multiple timeouts and intervals
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I noticed some of the long lived timeouts and intervals set in `app.js` were not protected from being set multiple times. Under normal circumstances they shouldn't be created more than once... however this PR will make sure that only 1 timeout/interval will be set.

Signed-off-by: David Huffman <dshuffma@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-30 20:41:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/92" class=".btn">#92</a>
            </td>
            <td>
                <b>
                    update stitch deps to fix buffer issue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes error introduced in the latest stitch. `Buffer is not defined`
Signed-off-by: David Huffman <dshuffma@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-30 20:26:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/91" class=".btn">#91</a>
            </td>
            <td>
                <b>
                    prevent doc conflicts during backup api
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The backup api had a doc conflict issue. The previous backup's `_rev` was being kept around instead of resetting. This error would prevent a db backup from being saved.

Signed-off-by: David Huffman <dshuffma@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-30 20:21:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/88" class=".btn">#88</a>
            </td>
            <td>
                <b>
                    added release notes
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
        Created At 2021-11-29 15:04:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/87" class=".btn">#87</a>
            </td>
            <td>
                <b>
                    create setting to allow users to keep default pass
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                added the setting `allow_default_password`
- if `true` users are allowed to keep the default password
- if `false` users will be forced to set a new password after their first login
- defaults `false`

https://github.com/hyperledger-labs/fabric-operations-console/issues/79
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-24 20:14:42 +0000 UTC
    </div>
</div>

