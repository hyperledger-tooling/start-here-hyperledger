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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1013" class=".btn">#1013</a>
            </td>
            <td>
                <b>
                    fix(ledger): check taa version instad of aml version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1010 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-06 11:59:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1011" class=".btn">#1011</a>
            </td>
            <td>
                <b>
                    fix(ledger): remove poolConnected on pool close
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes issue where cannot reconnect to ledger after rotating wallet key

Signed-off-by: Niall Shaw <niall.shaw@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-06 07:34:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1003" class=".btn">#1003</a>
            </td>
            <td>
                <b>
                    fix: unable to resolve nodejs document loader in react native runtime environment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Should fix #993 by conditionally importing the XHR and NodeJS document loaders, based on the runtime environment.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-01 11:03:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1001" class=".btn">#1001</a>
            </td>
            <td>
                <b>
                    fix(question-answer): question answer protocol state/role check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Some fixes and additional checks in process methods from `QuestionAnswerService` that are preventing it to correctly accept/reject the received message.

Add some service tests as well as a simple E2E module test that allowed to find and fix a weird issue with parameter construction: `ValidResponse` takes another `ValidResponse` as input and this could make message validation to fail.

No API changes were introduced apart from adding a `findById` method.

Signed-off-by: Ariel Gentile <gentilester@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-31 02:56:04 +0000 UTC
    </div>
</div>

