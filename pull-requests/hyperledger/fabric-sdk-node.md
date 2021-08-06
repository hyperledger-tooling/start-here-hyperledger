---
layout: default
title: fabric-sdk-node
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-node
---

# fabric-sdk-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/480" class=".btn">#480</a>
            </td>
            <td>
                <b>
                    [bug-fix] eventhub status value is now interpreted as http code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                instead of string like "NOT_FOUND", we see the actual value is 404
Signed-off-by: DavidLiu <david.yx.liu@oracle.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-06 03:38:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/479" class=".btn">#479</a>
            </td>
            <td>
                <b>
                    FABN-1724: add support async signing of message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `ICryptoSuite` interface of `fabric-common` support only synchronous `sign()` method. Which sound correct for `Default X509 Identity` and `HSM X509 Identity` provider. But to support other kind of identity providers (like Vault Transit Engine/PKCS#11 Proxy) which require network `I/O` to get the message signed, will require `sign()` function to be an asynchronous.

Main change in this PR

*From*
```js
export interface ICryptoSuite {
     // ....
     sign(key: ICryptoKey, digest: Buffer): Buffer ;
}
```
*To*
```js
export interface ICryptoSuite {
     // ....
     sign(key: ICryptoKey, digest: Buffer): Buffer | Promise<Buffer>;
}
```
[FABN-1724](https://jira.hyperledger.org/browse/FABN-1724?filter=-2)

Signed-off-by: Pritam Singh <pkspritam16@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-04 14:34:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/478" class=".btn">#478</a>
            </td>
            <td>
                <b>
                    Reference Asset Transfer samples in SDK docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Reference Asset Transfer samples in SDK docs instead of
Fabcar and Commercial Paper.  The Asset Transfer
samples have corresponding beginner tutorials and
Fabric docs and is the recommend place to start now.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-30 22:34:18 +0000 UTC
    </div>
</div>

