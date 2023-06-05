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
                PR <a href="https://github.com/hyperledger/fabric/pull/4262" class=".btn">#4262</a>
            </td>
            <td>
                <b>
                    WIP: Raft WAL deadlock test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                WAL deadlock recreation

#### Type of change

- Bug fix
- Test update

#### Description

Please look at #4199, and PR #4201 .
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-05 09:32:01 +0000 UTC
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4257" class=".btn">#4257</a>
            </td>
            <td>
                <b>
                    Update CouchDB doc references to 'stable' (backport #4256)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4256 done by [Mergify](https://mergify.com).


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
        Created At 2023-06-02 17:36:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4256" class=".btn">#4256</a>
            </td>
            <td>
                <b>
                    Update CouchDB doc references to 'stable'
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Instead of maintaining the exact version of CouchDB docs and risk getting outdated, it is safe to reference the 'stable' version of the CouchDB docs since the doc content in these topics has indeed been stable.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-02 15:10:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4255" class=".btn">#4255</a>
            </td>
            <td>
                <b>
                    Release commit for v2.2.12
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update docs and release notes for v2.2.12.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-02 15:03:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4254" class=".btn">#4254</a>
            </td>
            <td>
                <b>
                    Bump CouchDB to 3.3.2 (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump CouchDB to 3.3.2.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-02 14:17:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4253" class=".btn">#4253</a>
            </td>
            <td>
                <b>
                    Release commit for v2.5.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add docs and release notes for v2.5.2 release.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-02 13:38:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4248" class=".btn">#4248</a>
            </td>
            <td>
                <b>
                    Make AmMemberOf to use only the mspIDs in collection policy (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Make AmMemberOf to use only the mspIDs in collection policy.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-31 14:41:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4246" class=".btn">#4246</a>
            </td>
            <td>
                <b>
                    Make AmMemberOf to use only the mspIDs in collection policy (backport #4244)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4244 done by [Mergify](https://mergify.com).


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
        Created At 2023-05-31 12:51:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4244" class=".btn">#4244</a>
            </td>
            <td>
                <b>
                    Make AmMemberOf to use only the mspIDs in collection policy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description

https://github.com/hyperledger/fabric/issues/4229

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

<!--- Include a link to any associated issues, e.g. Jira issue or approved rfc. -->

<!---
#### Release Note
If change impacts current users, uncomment Release Note heading and provide
release note text.
Also, copy release note text into the release specific /release_notes file.
-->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-30 18:25:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4242" class=".btn">#4242</a>
            </td>
            <td>
                <b>
                    BFT Block Puller: verify attestation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change-Id: Ia34ff4536453581895c4f13b2d73f0e7066ce125

#### Type of change

- New feature

#### Description

BFT Block Puller: verify attestation. 
Verify a block attestation, which is a block with block.Data=nil.
Verification is the same as verifying a regular block, except computing the data hash and comparing it to the hash in the header, and extracting the channel ID.

#### Related issues
#4240 
#4243 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-30 09:06:47 +0000 UTC
    </div>
</div>

