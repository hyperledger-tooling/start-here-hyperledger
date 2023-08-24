---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/955" class=".btn">#955</a>
            </td>
            <td>
                <b>
                    Added 'names' attribute field parsing in credx
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Addresses #948 .
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-24 09:47:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/954" class=".btn">#954</a>
            </td>
            <td>
                <b>
                    Uniffi demo qr scan
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Merge only after #896 
This PR elaborates the Uniffi demo and API.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-24 06:05:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/953" class=".btn">#953</a>
            </td>
            <td>
                <b>
                    Refacotr/ledger trait
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">skip-ci</span>
            </td>
            <td>
                TODO
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-24 05:10:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/952" class=".btn">#952</a>
            </td>
            <td>
                <b>
                    Demo for aries vcx
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - alice & faber demo to establish connection
- modifies `simple_message_relay` to enable its consumption also as library, rather than executable only
- extends `simple_message_relay` with mpsc channels which forward any incoming message to mpsc receiver. This is nice because in the demo, I don't need to call relay's API at all - just await receiver to wait for new incoming message

Having to interact with aries-vcx from scratch from new application, some improvements I've identified:
- https://github.com/hyperledger/aries-vcx/issues/949
- https://github.com/hyperledger/aries-vcx/issues/951

## Note
This can be thought of as temporary solution to demonstrate the APIs and usage. And while far from ideal yet (todos left, issues created), it's a lot easier to understand than pointing someone to integration tests today. Main issue of integration tests is that they are all couploed with vcxagency-node mediator, but also other issues.
After integration tests are in better shape after:
- https://github.com/hyperledger/aries-vcx/pull/945
- https://github.com/hyperledger/aries-vcx/pull/946
- and subsequent removal of IO, and therefore coupling with vcxagency-node mediator
- and some refactoring of "Alice" "Faber" devsetup agents

I believe that integration tests could be in condition to demonstrate the usage (and surface outstanding API issues) equally good as this demo.
But for the time being, this demo is a lot simpler than the existing integration tests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-22 15:33:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/946" class=".btn">#946</a>
            </td>
            <td>
                <b>
                    IO for issuer and holder as opt-in
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">breaking</span>
            </td>
            <td>
                #### Note:
WIP, yet missing completing the work on Holder, but changes so far are meant to be final in scope of this PR and ready for review.

### Changes
##### Issuer: Removed state `OfferSent`
- Remove `OfferSent` state, keep only `OfferSet`; treat `OfferSet` as `OfferSent`
- To keep Issuer dependant works, Issuer still has its original method `send_credential_offer` which unlike before, does not modify state. Hence existing code should still keep working.

##### Issuer: Removed state `CredentialSent`
- Remove state `CredentialSent`, introduce state `CredentialSet` instead
- The semantic reason between them is self-explaining, "set" doesn't imply the message has been sent
- Structural reason between the 2 is `CredentialSet` has additional field `msg_issue_credential: IssueCredential` to decouple construction of credential from sending `issue-credential` msg

#### Holder: Removed state `RequestSent`
- Remove state `RequestSent`, introduce state `RequestSet` instead
- Generally change analogic to the ones above.

### Strategy
- This PR keep SM's ability to "send" messages, which it keeps in SM's state, however, these calls are opt-in, so callers can choose to send the messages on their own instead.
- In the next stage, we will remove `send_*` methods and required callers to assure msg sending on their own.
  - That will mean that tests can run much faster and do not need to establish didcomm connection and interact with mediator
  - State machines will be generally well position for further transition to typestate pattern followin https://github.com/hyperledger/aries-vcx/pull/928 pattern where transitions function include "msg to be sent out" in return type.

### Breaking
- Issuer: state machines in the intermediate `OfferSent` state won't be valid anymore (state removed)
- Issuer: state machines in the intermediate `CredentialSent` state won't be valid anymore (state removed)
- Issuer: If constructing anoncreds credential / issue-credential message fails, the state machine transitions to failed `Finished` state, but doesn't sends the problem report. You have to check the state and send problem report yourself.
- Holder: state machines in the intermediate `RequestSent` state won't be valid anymore (state removed)
- Holder: if construction anoncreds credential-request / request-credential message fails, the state machine transitions to failed `Finished` state, but doesn't sends the problem report. You have to check the state and send problem report yourself.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-20 10:40:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/945" class=".btn">#945</a>
            </td>
            <td>
                <b>
                    Declutter issuance&presentation protocols
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Changes
- No breaking changes
- Remove concept of "Action" as way to trigger actions/process messages from both Holder and Issuer handlers & state machines
- Externalize interactions with mediated connections and related code to files `mediated_holder.rs`, `mediated_issuer.rs` etc. out of state machine/handlers code itself
- Removed disabled unit tests - majority of tests was testing validity of sequence of FSM transitions. These will be irellevant with typestate pattern

### Next steps:
- We can follow this up with changes to states to remove IO - that itself has higher value than transformation to typestate pattern. 
  - After that, we can in parallel boost up testing performance significantly https://github.com/hyperledger/aries-vcx/issues/786
- In last stage we could rewrite thing to typestate + abstracting out & unifying approach for message processing as drafted in https://github.com/hyperledger/aries-vcx/pull/944
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-19 13:48:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/944" class=".btn">#944</a>
            </td>
            <td>
                <b>
                    Proposal/processor
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
        Created At 2023-08-18 16:17:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/943" class=".btn">#943</a>
            </td>
            <td>
                <b>
                    Remove libvcx-c, libvcx java, libvcx ios
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                After ~9 months of deprecation, we remove libvcx-c and associated java and ios wrappers.

However, anyone with strong interest to keep this components "alive" is welcome to take owner their ownership and maintenance. Please contact us if you are interested and we can provide some guidance.

However, recommended strategy for mobile devices is building custom FFI layer on top of aries-vcx crate. There's project in progress https://github.com/hyperledger/aries-vcx/pull/896 demonstrating such approaching using UniFFI library. While not complete, it's great starting point for anyone looking to build native, aries enabled, mobile app.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-18 14:15:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/942" class=".btn">#942</a>
            </td>
            <td>
                <b>
                    Release 0.58.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - First release with removed libvcx-c, libcx java and ios wrappers. See https://github.com/hyperledger/aries-vcx/pull/943
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-18 14:00:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/941" class=".btn">#941</a>
            </td>
            <td>
                <b>
                    Expose public key getter on verification method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Introduces a `public_key::Key` getter in `VerificationMethod` to facilitate easy retrieval of the key representation derived from `VerificationMethod`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-18 06:54:46 +0000 UTC
    </div>
</div>

