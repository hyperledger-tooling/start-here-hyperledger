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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/393" class=".btn">#393</a>
            </td>
            <td>
                <b>
                    fix(core): requested predicates transform type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Type: Bug</span>
            </td>
            <td>
                Incorrect `@Type` transform was added to requested predicates, overriding `@RecordTransformer`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-19 09:59:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/392" class=".btn">#392</a>
            </td>
            <td>
                <b>
                    feat(node): add http and ws inbound transport
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Moves http and ws inbound transports to the node package. I know there's still work to be done on the transports, but this makes it 1000x easier to set up an agent. They're in the node package, so not strictly tied to core
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-19 09:21:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/390" class=".btn">#390</a>
            </td>
            <td>
                <b>
                    feat(core): add discover features protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add discover features protocol.

Currently working on aries-toolbox integration where this is required for.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-16 22:06:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/388" class=".btn">#388</a>
            </td>
            <td>
                <b>
                    feat(redux-store): move from mobile agent repo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Moves the `@aries-framework/redux-store` package from the mobile agent to here for easier management.

This is just the state as it was in the mobile agent repo. @jakubkoci You'll probably have opinions on this, and I'm interested to hear it. 

I'd like to merge first so we can use the package without manually packing every time, and then discuss maybe at the AFJ WG call.

Fixes hyperledger/aries-mobile-agent-react-native#64
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-16 09:28:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/387" class=".btn">#387</a>
            </td>
            <td>
                <b>
                    ci: fetch all commits for correct versioning
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Placed it in the wrong job.. Need it in the release
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-16 09:22:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/386" class=".btn">#386</a>
            </td>
            <td>
                <b>
                    fix: monorepo release issues
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Some issues that I encountered using the new packages in our projects.

Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-16 08:46:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/375" class=".btn">#375</a>
            </td>
            <td>
                <b>
                    renamed RecipientService to MediationRecipientService
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Adam Burdett <burdettadam@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-13 17:52:50 +0000 UTC
    </div>
</div>

