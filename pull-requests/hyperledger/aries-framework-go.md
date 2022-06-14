---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3261" class=".btn">#3261</a>
            </td>
            <td>
                <b>
                    feat: validate data model of objects saved in a wallet.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Volodymyr Kubiv <volodymyr.kubiv@euristiq.com>

**Title:**
VC Wallet Data Model validation

**Description:**
https://github.com/hyperledger/aries-framework-go/issues/3260

**Summary:**
Data models are validated against their JSON LD context before being saved into the wallet content store.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-13 08:33:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3259" class=".btn">#3259</a>
            </td>
            <td>
                <b>
                    refactor: remote cryptobox URLs renamed to /wrap and /unwrap
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                this change updates the remote CryptoBox api URIs to point to remote KMS's key /wrap and /unwrap to match ECDH-ES and ECDH-1PU key wrapping.

This change requires the KMS server to udpate /easy to /wrap, /easyOpen and /sealOpen to /unwrap

Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-09 17:38:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3257" class=".btn">#3257</a>
            </td>
            <td>
                <b>
                    feat: interop support for did service refactor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-07 20:36:23 +0000 UTC
    </div>
</div>

