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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3252" class=".btn">#3252</a>
            </td>
            <td>
                <b>
                    feat: Full EDV provider support for AND+OR multiple tag queries
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The EDV storage provider can now do full AND+OR tag querying. The SetStoreConfig method no longer calls the "add index" endpoint as it won't be added to the spec (indexing will be automatically by the EDV server).

Also updated storage interface documentation for the Query method to accommodate the new functionality.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-02 22:24:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3251" class=".btn">#3251</a>
            </td>
            <td>
                <b>
                    chore: add is did comm v2 method to service endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Firas Qutishat <firas.qutishat@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-02 19:01:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3250" class=".btn">#3250</a>
            </td>
            <td>
                <b>
                    fix: did doc parsing to properly distinguish V1 vs V2 types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Signed-off-by: Baha Shaaban [baha.shaaban@securekey.com](mailto:baha.shaaban@securekey.com)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-02 16:03:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3249" class=".btn">#3249</a>
            </td>
            <td>
                <b>
                    feat: separate cache from token.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Volodymyr Kubiv <volodymyr.kubiv@euristiq.com>

**Title:**
VC Wallet: decoupling KMS cache & token

**Description:**
Closes #2556

**Summary:**

Move token management from keyManager into a separate sessionManager.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-02 09:38:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3247" class=".btn">#3247</a>
            </td>
            <td>
                <b>
                    chore: create didcomm v1 and v2 keys in mediator service
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Firas Qutishat <firas.qutishat@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-31 16:44:00 +0000 UTC
    </div>
</div>

