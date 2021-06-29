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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/334" class=".btn">#334</a>
            </td>
            <td>
                <b>
                    chore: export wallet interface
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
        Created At 2021-06-28 15:35:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/333" class=".btn">#333</a>
            </td>
            <td>
                <b>
                    chore: export injection symbols
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
        Created At 2021-06-25 19:55:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/331" class=".btn">#331</a>
            </td>
            <td>
                <b>
                    feat: allow for lazy wallet initialization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - remove agent `closeAndDeleteWallet` as it was only used for tests. They now inject the wallet to close and delete
- make `walletConfig` and `walletCredentials` optional in `InitConfig`
- user can now manually initiale the wallet
- If agent is initialized and wallet is not yet initialized and no `walletConfig` and `walletCredentials` are available an error will be thrown
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-24 16:32:26 +0000 UTC
    </div>
</div>

