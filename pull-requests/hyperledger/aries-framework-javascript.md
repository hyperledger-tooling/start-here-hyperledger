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

