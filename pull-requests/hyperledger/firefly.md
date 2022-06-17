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
                PR <a href="https://github.com/hyperledger/firefly/pull/865" class=".btn">#865</a>
            </td>
            <td>
                <b>
                    Create firefly subscription per namespace
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Each namespace now has a unique firefly contract subscription

To support a subscription per namespace, the `fireflyContract` config section has been replaced with the `contracts` array section under the `multiparty` config.

Example:
```
blockchain:
- name: blockchain0
  type: ethereum
  ethereum:
    ethconnect:
      url: http://ethconnect_0:8080
      topic: "0"
      
namespaces:
  default: default
  predefined:
  - name: default
    remoteName: default
    description: Default predefined namespace
    plugins: [database0, blockchain0, dataexchange0, sharedstorage0, erc20_erc721]
    multiparty:
      enabled: true
      org:
        name: org0
        description: org0
        key: 0x123456
      contract:
        - location:
            address: 0x4ae50189462b0e5d52285f59929d037f790771a6 
          firstEvent: oldest
```

 * location is a yaml object containing blockchain plugin configuration
 * `firstEvent` is replacing `fromBlock`, supporting values of newest or oldest

This PR also introduces a new component, multiparty manager, that is responsible for managing the active firefly contract and interfacing with the blockchain plugin on behalf of that contract.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 21:00:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/864" class=".btn">#864</a>
            </td>
            <td>
                <b>
                    Further cleanup of namespace params to managers and database plugin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Part of [FIR-12](https://github.com/hyperledger/firefly-fir/pull/12)
In a chain with #862

Each manager is specific to a namespace, which should be received and stored during init. All operations conducted by that manager should use that namespace, and therefore no manager methods should accept a namespace as a parameter.

The database plugin, on the other hand, may potentially service multiple namespaces. Therefore, all query operations should take a namespace parameter to ensure that only results from a single namespace are returned.

This PR makes these true for many cases, but others are still to be addressed with a follow-up PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 15:24:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/863" class=".btn">#863</a>
            </td>
            <td>
                <b>
                    Move event plugin init to namespace manager
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Part of [FIR-12](https://github.com/hyperledger/firefly-fir/pull/12)

The event plugins should be singletons, but subscription manager is initialized once per namespace. A single websocket connection may facilitate listeners to multiple subscriptions (and therefore multiple namespaces), and the events need to be delivered to the correct subscription manager.

Current tests should pass, but additional unit test coverage is still pending.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 15:19:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/862" class=".btn">#862</a>
            </td>
            <td>
                <b>
                    Remove namespace from identity manager, network map, and group manager calls
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Part of [FIR-12](https://github.com/hyperledger/firefly-fir/pull/12)

Each manager is initialized for a single namespace and can assume all calls are scoped within that namespace This PR tackles identity manager, network manager, and group manager so they store and use that single namespace.

The one exception is for "network version 1", where identities may have been registered on the legacy "ff_system" namespace. In this case, the identity manager will query "ff_system" instead of its assigned namespace (noting that this will only work if "ff_system" shares a database with that namespace).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-14 19:06:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/861" class=".btn">#861</a>
            </td>
            <td>
                <b>
                    Push namespace info to token connector, handle batch events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ~~This is in a PR chain with the (massive) #855, so that should be reviewed and merged first. Only the last 2 commits are new.~~

Part of [FIR-12](https://github.com/hyperledger/firefly-fir/pull/12)

This is the counterpart to https://github.com/hyperledger/firefly-tokens-erc1155/pull/78 and https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/59.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-14 16:07:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/860" class=".btn">#860</a>
            </td>
            <td>
                <b>
                    Updating Create Listener Docs to Use eventPath
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: hfuss <haydenfuss@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-14 14:25:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/858" class=".btn">#858</a>
            </td>
            <td>
                <b>
                    Remove redundant payloadRef field on Batch Pin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This field is not used by any code.

There was a vision that storing the `payloadRef` on broadcast batches for reference, but this was never implementing. Meaning this field is cruft.

Currently the right way to find the payload reference, is to look at the upload/download operations for the batch.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-13 15:29:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/857" class=".btn">#857</a>
            </td>
            <td>
                <b>
                    FAQ and FireFly Tutorial Updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Two main changes in this PR:
1- FAQ updates. Added some FAQs related to deploying smart contracts, connecting to Metamask, and how FireFly enables multi-chain applications
2- FireFly tutorial updates. Fixed some links to swagger pages that were outdated, updated some instructions, added instructions and screenshots on using the FireFly sandbox in order to follow along some of the examples given in the tutorials
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-10 17:19:37 +0000 UTC
    </div>
</div>

