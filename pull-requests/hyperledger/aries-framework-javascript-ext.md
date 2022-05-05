---
layout: default
title: aries-framework-javascript-ext
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript-ext
---

# aries-framework-javascript-ext <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript-ext){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript-ext/pull/114" class=".btn">#114</a>
            </td>
            <td>
                <b>
                    chore: add revocation notification event listening for react-hooks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Made it so Revocation Notification events will also trigger the CredentialProvider listener.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-04 22:33:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript-ext/pull/113" class=".btn">#113</a>
            </td>
            <td>
                <b>
                    fix(react-hooks): Update providers on delete events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There were no delete events in `core` package, so providers only listen to change events. Whenever a record is deleted, for example with: 
```
agent.credentials.deleteById(credentialId)
```
provider is not updated, and the `useCredentials` hook does not update returned credentials array.
This branch utilizes changes made in https://github.com/hyperledger/aries-framework-javascript/pull/716 and adds delete events listeners to fix that issue.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-28 11:52:19 +0000 UTC
    </div>
</div>

