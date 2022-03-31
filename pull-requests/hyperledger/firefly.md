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
                PR <a href="https://github.com/hyperledger/firefly/pull/630" class=".btn">#630</a>
            </td>
            <td>
                <b>
                    Do not return an error from status if node lookup fails
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In `v0.14.0` if you register your org (only), and then call `/api/v1/status` you receive:

```js
{"error":"FF10277: Identity could not be resolved via DID 'did:firefly:node/zzhc7hdmc0'"}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-25 20:15:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/629" class=".btn">#629</a>
            </td>
            <td>
                <b>
                    [ui-v0.6.3] v0.6.3 release of ui in manifest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Echelberger <eberger727@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-25 19:23:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/627" class=".btn">#627</a>
            </td>
            <td>
                <b>
                    Simplfy solc compilation of BatchPin contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a slight simplification to the way the BatchPin contract is compiled at build time. This allows us to remove some deprecated code in the FireFly CLI and goes along with the changes in https://github.com/hyperledger/firefly-cli/pull/165
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-24 19:41:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/626" class=".btn">#626</a>
            </td>
            <td>
                <b>
                    Add pool config to activate call
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Enables https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/36
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-24 18:40:07 +0000 UTC
    </div>
</div>

