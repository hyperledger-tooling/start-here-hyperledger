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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1578" class=".btn">#1578</a>
            </td>
            <td>
                <b>
                    fix(core): remove node-fetch dependency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Our good friend @dependabot with its #1565 made me remember we had this dependency on core that shouldn't be there. Didn't go further in order to not deal with breaking changes. I think we can move to node-fetch v3 (and see how to deal `AgentDependencies` types) in a next major release.

Fixes #1492
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-18 22:34:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1576" class=".btn">#1576</a>
            </td>
            <td>
                <b>
                    feat: Discover Features V2 over DIDComm V2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Discover Features 2.0 is one of those protocols that are suitable for both DIDComm V1 and V2. However, this becomes a bit complicated because current AFJ model considers that a given message type is defined for either V1 or V2.

So after an interesting discussion in a previous AFJ WG Call, we found out that we can leave each protocol determine which versions it supports and register both models into the `MessageHandlerRegistry`, which will now allow to filter not only by message type (PIURI) but also by DIDComm version.

In this PR we have:
- Different fixes and adaptations for DIDComm V2 (like attachment transformers, message handling, etc.) found during the work of other PRs (#1546 and #1560). This would make this PR to be the basis of those, which will hopefully only add new protocols and make their review easier
- New handling of received messages in `MessageReceiver` and `Dispatcher` to figure out whether it is a DIDComm V1 or V2 message and find the right class and handler
- Updates in Discover Features module to add DIDComm V2 modeling for Query and Disclosure messages, and register/process both in a single handler and service
- There are some slight API changes, like the return types and events, due to messages can be now either be DIDComm V1 or V2. I think in the next major release (before merging DIDComm V2 to main) we can remove the complete message object from the event, as the relevant fields are sent as separate properties (and in case we want to go low level and get the complete message we can subscribe  to `AgentMessageProcessedEvent`)
- Discover Features V2 E2E test has been updated to work in both DIDComm V1 and V2. This makes it to require Askar. As we'll switch soon our tests to node 18 + shared components I guess there is no problem on that


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-16 18:39:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1575" class=".btn">#1575</a>
            </td>
            <td>
                <b>
                    fix: service validation in OOB invitation objects
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I'm not an expert (neither a fan 😝) of `class-validator` but I recently found an issue when creating an `OutOfBandInvitation` instance whose `service` field contains a plain string. It works and allows to do a `toUrl()` and so on, but when it passes through the MessageValidator it threw an error saying:

```
OutOfBandInvitation: Failed to validate class.
    An instance of OutOfBandInvitation has failed the validation:
     - property services[0] has failed the following constraints: each value in nested property services must be either object or array·
```

I found that services field has both `@IsStringOrInstance` and `@ValidateNested` decorators. The first one seems to be doing the correct check on every element of the array, while the latter (which is the one  throwing the error) seems to me redundant in this case. If I remove it, class validation passes (as expected). 

So here I'm removing `@ValidateNested` decorator. Not sure if it's the best approach, but of course happy to change it if there is a more appropriate way.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-15 14:48:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1574" class=".btn">#1574</a>
            </td>
            <td>
                <b>
                    fix(cheqd): Changed the name formatting to a encoded hex value
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                For more information about these changes, see: https://cheqd-community.slack.com/archives/C02AQ9UK4HY/p1693916571308369
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-15 10:30:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1573" class=".btn">#1573</a>
            </td>
            <td>
                <b>
                    fix: improve logging
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
        Created At 2023-09-13 10:12:51 +0000 UTC
    </div>
</div>

