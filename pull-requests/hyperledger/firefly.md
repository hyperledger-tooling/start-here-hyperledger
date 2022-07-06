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
                PR <a href="https://github.com/hyperledger/firefly/pull/884" class=".btn">#884</a>
            </td>
            <td>
                <b>
                    Stop orchestrator for ff_system when moving to network V2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Part of [FIR-12](https://github.com/hyperledger/firefly-fir/pull/12)
In a chain with #883

Background: The legacy `ff_system` namespace is created (ie an orchestrator and managers are initialized) whenever the default namespace is a V1 multiparty network. The `ff_system` namespace is initialized with an exact duplicate of the default namespace config (same plugins, same contract addresses, etc).

With this PR, if the default namespace (and therefore `ff_system`) migrates to V2 rules, the `ff_system` orchestrator will be stopped and removed, along with all its children.

This should allow legacy networks to cleanly migrate to V2 rules and retire `ff_system`. Notable caveat: once the default namespace is on V2, no other V1 namespaces will be supported.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 01:13:35 +0000 UTC
    </div>
</div>

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
                Part of [FIR-12](https://github.com/hyperledger/firefly-fir/pull/12)

For blockchain batch pin events, direct them to an appropriate namespace:
* If the multiparty contract is V1, the namespace is passed explicitly
* If the multiparty contract is V2+, the namespace is packed into the subscription name (and is not sent in the event)

For blockchain network actions, direct them to an appropriate namespace:
* If the multiparty contract is V1, send them to all handlers (the handler will filter based on whether the contract address matches the active contract)
* If the multiparty contract is V2+, the namespace is packed into the subscription name

Caveat for pre-existing subscriptions: Old subscription names will _not_ have a namespace included, so multiple namespaces will actually be sharing a single subscription. This is OK for V1 networks, as batch pin events always contain a namespace and network actions are sent to all handlers. A V2 network cannot function in this situation, so V2 contracts will be fundamentally incompatible with releases of FireFly prior to 1.1.

Tokens are also subject to the same problem where pre-existing subscriptions will not include namespace information, so they always send events to all handlers if namespace is unset.

Unanswered question: how does ff_system "go away" cleanly when migrating to a V2 contract? There is no entry for ff_system in the namespace config, so migration is weird and probably tied to the default namespace instead. UPDATE - see #884
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-29 19:04:07 +0000 UTC
    </div>
</div>

