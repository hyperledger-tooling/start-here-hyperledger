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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1093" class=".btn">#1093</a>
            </td>
            <td>
                <b>
                    fix(routing): async message pickup on init
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently, when initializing the agent using a `MediationPickupStrategy` different from `None` (e.g. `PickupV1` or `PickupV2`), it attempts to start message pickup in a synchronous way, meaning that it might take some more time for startup depending on the . Also, if mediator is not reachable at that moment, it will throw an error and Agent's `_isInitialized` flag will not be set to true even if can connect afterwards (with the polling of PickupV1 or backoff strategy of PickupV2).

In this PR we are starting the message pickup process in an async way and catching any possible initial error, in a similar way as Agent's initialize method for connecting to ledger pools.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-09 13:02:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1092" class=".btn">#1092</a>
            </td>
            <td>
                <b>
                    feat: Issue Credentials V2 (W3C/JSON-LD) with Commits Squashed
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
        Created At 2022-11-09 09:27:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1086" class=".btn">#1086</a>
            </td>
            <td>
                <b>
                    refactor: remove dependency on indy ledger service from sov did resolver/registrar
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                resolves: #1066  and  #1067 
Signed-off-by: Sai Ranjit Tummalapalli <sairanjit5@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-06 07:54:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1085" class=".btn">#1085</a>
            </td>
            <td>
                <b>
                    fix(connections): do not log AgentContext object
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In last [Aries Framework JS call](https://wiki.hyperledger.org/display/ARIES/2022-11-03+Aries+Framework+JS+Meeting+notes) @niall-shaw reported performance issues when accepting multi-use invitations. 

I've experienced the same issue after migrating to 0.3.0-alpha.x and it turns out that it was happening because some methods in `DidExchangeProtocol` were logging the whole messageContext object, which now includes agentContext and blocks the console for several seconds. This can be avoided by either logging in INFO mode or customizing the logger being in use to only output a certain depth level of objects.

This PR makes a quick-fix of this issue by logging only messageContext.message, to be consistent with other methods from `ConnectionService`. Not sure if it's really useful though, but that's another subject to discuss 😄 .
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-04 22:42:51 +0000 UTC
    </div>
</div>

