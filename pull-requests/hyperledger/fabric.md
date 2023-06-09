---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4267" class=".btn">#4267</a>
            </td>
            <td>
                <b>
                    Restrict WAL usage to node.go (backport #4201)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4201 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-07 15:11:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4266" class=".btn">#4266</a>
            </td>
            <td>
                <b>
                    Fix typo in logger name
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                commmon -> common


#### Type of change

- Bug fix

#### Description

Typo in the word _common_ being written with 3 `m`'s instead of only 2.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-07 06:30:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4265" class=".btn">#4265</a>
            </td>
            <td>
                <b>
                    Follower: check if join block different from fetched block
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change-Id: I7089df4f1bfc200a5f17582df0da7d4172f8f09b


#### Type of change

- Bug fix

#### Description

Follower: revert check of join block different from fetched block

#### Related issues

Addresses #4264 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-06 10:37:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4263" class=".btn">#4263</a>
            </td>
            <td>
                <b>
                    Raft WAL deadlock test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - There was a bug described at issue #4201. 
- The bug caused a deadlock on etcd raft orderer chain apply change on orderer startup.
- Issue #4201 fixed the issue. 
- We wanted to add a test can check this scenario with high probability (because of the multiple go routines, and how the code is built, this can't be 100% test.)
- We simulated the scenario of the deadlock using a test and debug logs (on the unfixed code) in #4262.
- This PR adds the same test but without the debug logs.

#### Type of change

- Bug fix
- Test update

#### Description

Please look at #4199, PR #4201 and PR #4262.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-05 13:12:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4260" class=".btn">#4260</a>
            </td>
            <td>
                <b>
                    BFT BlockPuller: clean redundant map
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

The gossip service:
- It contains a map of channelID -> DeliverService (an interface).
- The DeliveryService is  implemented by a deliveryServiceImpl, which contains blockProviders a map of channelID -> Deliverer.
- The implementation shows that the external and internal maps are always keyed together, with the same channelID, which means that the internal map has always a single entry...

Remove the redundant internal map.

#### Related issues

#4261 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-04 16:16:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4258" class=".btn">#4258</a>
            </td>
            <td>
                <b>
                    BFT Block Puller: block deliverer, connection source
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change-Id: I4c2d9b8f74a4004d55e779438e41e7a80b274504

#### Type of change
- New feature

#### Description

- Introduce an abstraction BlockDeliverer that can CFT/BFT implementations
- Expose ConnectionSource method Endpoints

#### Related issues

Issue #4259 
Story #4240 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-04 14:36:56 +0000 UTC
    </div>
</div>

