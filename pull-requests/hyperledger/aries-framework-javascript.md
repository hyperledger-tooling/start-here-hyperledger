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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1523" class=".btn">#1523</a>
            </td>
            <td>
                <b>
                    ci: persist credentials to push tags
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Should fix the broken canary release pipeline
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-25 09:11:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1521" class=".btn">#1521</a>
            </td>
            <td>
                <b>
                    feat(anoncreds): auto create link secret
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As discussed in July 6th WG call, here we add an optional configuration parameter for  anoncreds-rs and indy-sdk modules that makes holder services to auto create a default link secret if no one has been created yet. This check is performed only when it is actually needed (i.e. when creating a credential request) rather than at agent initialization.

It defaults to true, meaning that normally it will not be needed to the consumer to do any specific logic to use AnonCreds as a holder.

Superseeds #1491 and fixes #1490
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-22 17:17:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1519" class=".btn">#1519</a>
            </td>
            <td>
                <b>
                    ci: set npm registry for releases
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Explicitly set npm registry in order to attempt to fix #1518 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-21 21:02:53 +0000 UTC
    </div>
</div>

