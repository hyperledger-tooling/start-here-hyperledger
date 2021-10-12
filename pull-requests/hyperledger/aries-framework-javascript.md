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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/482" class=".btn">#482</a>
            </td>
            <td>
                <b>
                    fix(core): improved present-proof tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Added some additional checking at the `proofs.test.ts`.
- I mainly copied it from the `credentials.test.ts`, but I am not sure if this is the correct way.
  - #363 mentions consistent tests ([eslint-plugin-jest](https://github.com/jest-community/eslint-plugin-jest))

Interested to hear some opinions on how we should deal with tests right now / in the future.

resolves #481 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-11 10:38:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/480" class=".btn">#480</a>
            </td>
            <td>
                <b>
                    fix(core): export AgentMessage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Berend Sliedrecht <berend@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 12:35:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/479" class=".btn">#479</a>
            </td>
            <td>
                <b>
                    fix(core): convert legacy prefix for inner msgs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit adds legacy type prefix support for CredentialPreview,
PresentationPreview and SignatureDecorator.

It does this by replacing the `did:sov:BzCbsNYhMrjHiqZDTUASHg;spec` legacy prefix with the newer `https://didcomm.org` prefix.

Signed-off-by: Karim Stekelenburg <karim@animo.id>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 13:21:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/478" class=".btn">#478</a>
            </td>
            <td>
                <b>
                    docs: update dev readme with changed setup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-06 13:04:52 +0000 UTC
    </div>
</div>

