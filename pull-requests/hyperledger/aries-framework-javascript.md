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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/364" class=".btn">#364</a>
            </td>
            <td>
                <b>
                    fix: Remove apostrophe from connection request message type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jakub Koci <jakub.koci@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-05 14:26:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/362" class=".btn">#362</a>
            </td>
            <td>
                <b>
                    feat: Use session to send outbound message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR contains the following changes:
* A session object is saved only if there is a `return_route` param in an inbound message. 
* An outbound message is sent via session object, and the dispatcher doesn't return the message to the caller. It works for both HTTP and WebSocket.
* The session object also contains the inbound message. The reason for this is that we can decide if we want to use the session to send a message later in MessageSender. We don't try to send a message via session if there is no `return_route` set for a given session.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-04 15:27:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/361" class=".btn">#361</a>
            </td>
            <td>
                <b>
                    refactor: use inline message types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #200 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-03 22:56:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/360" class=".btn">#360</a>
            </td>
            <td>
                <b>
                    refactor: only use ready connection for inbound
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR became a bit bigger than anticipated, but one change led to another and so on. However I do think this PR packs some nice improvements.

### validation on incoming messages

Fixes #68

Although used a lot, we weren't putting the validation decorators to good use yet (`@IsString`, etc...). I've enabled them and made updates where needed to make them valid. Already found some bugs. I think once we update the AFJ backchannel for AATH we'll probably find some more interop issues with ACA-Py.

### Only attach connection to inbound message context if sender and receiver match and connection is ready

Fixes #76

We were attaching the connection before it was ready and didn't do all necessary checks to make sure we're actually in the context of this connection. The connection is now only attached if the connection is ready to be used and fully matches with the incoming recipient and sender key.

### Break out indy wallet

Fixes #330

It didn't make a lot of sense to me that the indy wallet was handling indy storage and ledger stuff. I think it belongs more in the ledger and storage services. This is also more in line with where we're headed with the shared components libraries

- Rename `LedgerService` to `IndyLedgerService`. It's very indy focussed now.
- move storage related methods to `IndyStorageService`
- move ledger related methods to `IndyLedgerService`

### Better indy message handling

Sometimes you would get very cryptic errors such as `CommonInvalidParam` without a stack trace or anything that would help you get a sense of what's erroring out. I've wrapped all indy calls with a try catch and added a new `IndySdkError`. This will take the indy error as input, but with very nice stack tracing so you know exactly where things went wrong, without losing information from the indy error

---

Also fixed a bug where the mediator would terminate on unhandled promise

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-03 22:30:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/359" class=".btn">#359</a>
            </td>
            <td>
                <b>
                    feat: support connection-less issuance and verification
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds connection-less issuance and verification.

- `Agent.credentials.createOutOfBandOffer` - to create credential offer not bound to connection
- `Agent.proofs.createOutOfBandRequest` - to create presentation request not bound to connection
- Add `~service` decorator

Required more changes than initially thought because I had to remove the required `connection` parameter everywhere.

Fixes #347 
Fixes #346
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-03 15:15:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/342" class=".btn">#342</a>
            </td>
            <td>
                <b>
                    fix: add error message to log
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds error message to error log.

@jakubkoci this is what you get when you don't include the error message specifically. I think we need to fix this in rn-indy-sdk. I'll try to look at it in the near future. For now this fix helps

![image](https://user-images.githubusercontent.com/23165168/124268369-b3bc1a00-db39-11eb-8c28-d34f69ae6387.png)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-02 11:31:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/340" class=".btn">#340</a>
            </td>
            <td>
                <b>
                    build: docker containers are compatible with m1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds support for Apple silicon M1. Just specifies the platforms for which the containers were build and with Rosetta it should be possible to start the test ledger and mediators now.

Signed-off-by: Berend Sliedrecht <berend@animo.id>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-30 10:23:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/339" class=".btn">#339</a>
            </td>
            <td>
                <b>
                    feat: add inbound message queue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #259
Fixes #337
Fixes hyperledger/aries-mobile-agent-react-native#59

Adds inbound message queue with serial processing. The `agent.receiveMessage` does not yet use this queue as receiving messages directly on the agent seems separate and I think it won't interfere with the internal processing of messages. 

We can add it later, but we'd need to make the queue a bit more complex to be able to await `receiveMessage`. For now it should fix the race conditions as encountered by @MosCD3 and @pabloromeu
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-30 08:34:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/336" class=".btn">#336</a>
            </td>
            <td>
                <b>
                    feat: negotiation and auto accept credentials
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This allows for negotiation between the holder and the issuer via the `negotiateOffer` and `negotiateProposal` functions on `agent.credentials`. 

It also allows for auto accept of credentials. the `autoAcceptCredentials` can be set on the `agent` itself or on a specific `credentialRecord` where the `credentialRecord` has priority.

The `autoAcceptCredential` has three states: `always`, `contentApproved` and `never` where `never` is the default.

`always`: This means that any credential, no matter from who is automatically accepted (even if the attributes or `credentialDefinitionId` changed).
`contentApproved`: This means that when a credential is received it has to be accepted once and the attributes and `credentialDefinitionId` did not change. If something did change it will not automate the flow.
`never`: This simply means that no credentials are automatically accepted.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-29 14:34:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/335" class=".btn">#335</a>
            </td>
            <td>
                <b>
                    feature/0211-route-coordination
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This pull request provides support for [rfc 0211](https://github.com/hyperledger/aries-rfcs/tree/master/features/0211-route-coordination) mediation coordination. The implementation was inspired from [aca-py](https://github.com/hyperledger/aries-cloudagent-python) mediator and tested with. 
Flow is intended to follow after a connection has been established, request -> grant -> keylistUpdate. A lot of support code was added for mediation with new methods exposed on the agent. Some of the noteworthy changes include:
- Agent Config:
  - removed `mediatorUrl`, `establishInbound`, `getRoutingKeys` 
  - added `myPort`, `mediatorConnectionsInvite`, `autoAcceptMediationRequests`, `defaultMediatorId `
, `clearDefaultMediator`
  - the configurations are used in mediation modules and services to initialize state
- route module:
 - removed provision and consumer modules/services
 - added mediation and recipient modules
- transport:
 - added WebSocket POC for inbound transport with the mediator
 
Signed-off-by: Adam Burdett <burdettadam@gmail.com>
Co-authored-by: David Clawson <david.clawson@gmail.com>
Co-authored-by: Ariel Gentile <gentilester@gmail.com>
Co-authored-by: Daniel Bluhm <dbluhm@pm.me>
Co-authored-by: Patrick Kenyon <treek.kenyon@gmail.com>
Co-authored-by: James Ebert <jamesebert.k@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-28 21:28:54 +0000 UTC
    </div>
</div>

