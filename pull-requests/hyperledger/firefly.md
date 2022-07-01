---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/883" class=".btn">#883</a>
            </td>
            <td>
                <b>
                    Track blockchain callback handlers per namespace
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                For blockchain batch pin events, direct them to an appropriate namespace:
* If the multiparty contract is V1, the namespace is passed explicitly
* If the multiparty contract is V2+, the namespace is packed into the subscription name (and is not sent in the event)

For blockchain network actions, direct them to an appropriate namespace:
* If the multiparty contract is V1, send them to all handlers (the handler will filter based on whether the contract address matches the active contract)
* If the multiparty contract is V2+, the namespace is packed into the subscription name

Caveat for pre-existing subscriptions: Old subscription names will _not_ have a namespace included, so multiple namespaces will actually be sharing a single subscription. This is OK for V1 networks, as batch pin events always contain a namespace and network actions are sent to all handlers. A V2 network cannot function in this situation, so V2 contracts will be fundamentally incompatible with releases of FireFly prior to 1.1.

Tokens are also subject to the same problem where pre-existing subscriptions will not include namespace information, so they always send events to all handlers if namespace is unset.

Unanswered question: how does ff_system "go away" cleanly when migrating to a V2 contract? There is no entry for ff_system in the namespace config, so migration is weird and probably tied to the default namespace instead.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-29 19:04:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/882" class=".btn">#882</a>
            </td>
            <td>
                <b>
                    Deprecate default value for "ffdx"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This default value will be totally removed in v1.1+ due to #878. Deprecating it on the v1.0.x train will give a cleaner migration path forward.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 19:35:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/881" class=".btn">#881</a>
            </td>
            <td>
                <b>
                    Move SubmitNetworkAction and RootOrg config to Multiparty Manager
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also added new transaction and operation types for network action.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-24 20:17:12 +0000 UTC
    </div>
</div>

