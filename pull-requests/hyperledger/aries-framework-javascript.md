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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/999" class=".btn">#999</a>
            </td>
            <td>
                <b>
                    chore(release): v0.2.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ci-test</span>
            </td>
            <td>
                Release version 0.2.3
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 10:34:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/995" class=".btn">#995</a>
            </td>
            <td>
                <b>
                    docs(demo): faber creates invitation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It's better if Faber creates an invitation than Alice does because we can test mobile agents with Faber more easily.
- Now, Faber creates an invitation and Alice receives it.
- I didn't change the code but just exchanged connection-related code between Alice and Faber.
- The second commit(1e6af7a) is a minor bug fix.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-29 08:37:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/994" class=".btn">#994</a>
            </td>
            <td>
                <b>
                    feat: connection type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added a connection type enum to the connection record so that you can filter the connections based on type. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-26 18:03:03 +0000 UTC
    </div>
</div>

