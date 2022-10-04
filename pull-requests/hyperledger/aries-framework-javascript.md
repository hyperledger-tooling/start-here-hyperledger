---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1043" class=".btn">#1043</a>
            </td>
            <td>
                <b>
                    feat: possibility to set masterSecretId inside of WalletConfig
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
        Created At 2022-10-04 15:48:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1040" class=".btn">#1040</a>
            </td>
            <td>
                <b>
                    feat(question-answer): separate logic to a new module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Separated the question-answer logic to a new module.

Since it is now a separate module, if core gets released before the question-answer module it will not be included in the core anymore. This is a breaking change and might cause some headaches.

We can just merge it in after 0.3.0 is released and take our time with a strategy to add it back into the core for now. 

---

I could also keep the question-answer module inside the core and release this one separately. When we do a new 0.3.1 or 0.4.0 release the can remove it and make it dependent on this one.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-02 15:45:39 +0000 UTC
    </div>
</div>

