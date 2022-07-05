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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/927" class=".btn">#927</a>
            </td>
            <td>
                <b>
                    fix: missing module exports
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ariel Gentile <gentilester@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-03 21:02:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/926" class=".btn">#926</a>
            </td>
            <td>
                <b>
                    feat(oob): allow to append attachments to invitations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds an optional `appendedAttachments` field for OOB invitations (and legacy Connection Invitation messages) that allows to append attachments as per [Aries RFC 0017](https://github.com/hyperledger/aries-rfcs/tree/main/concepts/0017-attachments#appending).

Signed-off-by: Ariel Gentile <gentilester@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-03 20:34:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/924" class=".btn">#924</a>
            </td>
            <td>
                <b>
                    chore: update afj dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Just some housekeeping
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-03 13:38:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/922" class=".btn">#922</a>
            </td>
            <td>
                <b>
                    refactor!: add agent context
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">multitenancy</span>
            </td>
            <td>
                This is the same PR as #919 , but based off the 0.3.0-pre branch instead of main. There's no changes compared to #919 

Dependant on #920 and #921 

Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-03 12:12:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/921" class=".btn">#921</a>
            </td>
            <td>
                <b>
                    feat: add agent context provider
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">multitenancy</span>
            </td>
            <td>
                This is the same PR as #898, but based off the 0.3.0-pre branch instead of main. There's no changes compared to #898

Dependant on #920

Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-03 11:29:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/920" class=".btn">#920</a>
            </td>
            <td>
                <b>
                    refactor!: add agent context
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">multitenancy</span><span class="chip">breaking change</span>
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>

This is the same PR as #881, but based off the 0.3.0-pre branch instead of main. There's no changes compared to #881 except for making it work with this branch (making the new w3c services stateless). Due to the breaking changes we don't want to have this in main just yet. 

BREAKING CHANGE: To make AFJ multi-tenancy ready, all services and repositories have been made stateless. A new `AgentContext` is introduced that holds the current context, which is passed to each method call. The public API hasn't been affected, but due to the large impact of this change it is marked as breaking.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-03 11:12:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/913" class=".btn">#913</a>
            </td>
            <td>
                <b>
                    feat: add method to fetch KeyType by proof type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim <karim@animo.id>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-29 13:32:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/911" class=".btn">#911</a>
            </td>
            <td>
                <b>
                    ci: fix next version bump output
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Last one I hope...
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 08:45:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/910" class=".btn">#910</a>
            </td>
            <td>
                <b>
                    ci: fix next version bump variable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                CI is hard...
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 08:06:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/909" class=".btn">#909</a>
            </td>
            <td>
                <b>
                    feat(routing): add routing service
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">multitenancy</span>
            </td>
            <td>
                Adds a routing service that handles the creating of keys for routing and integrates with the mediation recipient service to add routing for the mediator.

The extraction is just to make sure we don't have to depend on a mediator dependency all across the framework. 

What this also adds is an event for when routing keys are created. This allows the tenant module to listen for created routing keys and can then create a mapping of it in the base wallet. I first started with a middleware approach (As described in the design document: https://hackmd.io/vGLVlxLvQR6jsEEjzNcL8g), but this added _ A LOT_ of complexity and didn't abstract away the mediator functionality as that is a part of the core API. So I went for the less generic but simpler API, that is just fine I think.

Again no changes to the public api, so we can merge this without issues



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 07:46:12 +0000 UTC
    </div>
</div>

