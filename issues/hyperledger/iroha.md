---
layout: default
title: iroha
parent: Hyperledger
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger/iroha
---

# iroha <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/1315" class=".btn">1315</a>
            </td>
            <td>
                <b>
                    Peer responded with QueryResult instead of VersionedQueryResult
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">good first issue</span><span class="chip">iroha2</span>
            </td>
            <td>
                When client sends request to endpoint /query, it expects as result `VersionedQueryResult`, but the peer returns `QueryResult`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-05 06:33:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/1237" class=".btn">1237</a>
            </td>
            <td>
                <b>
                    Place all configs in a separate folder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span>
            </td>
            <td>
                

We have a lot of configuration files:

    for peers and clients
    for tests and production
    for docker and local deployments

It's better to:

    Create `configurations` folder with examples of every typical configuration
    Use these configurations in tests, benchmarks and for base docker images


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-15 20:04:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/1185" class=".btn">1185</a>
            </td>
            <td>
                <b>
                    Rename iroha lib and bin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span>
            </td>
            <td>
                

Egor Ivkov, [11.06.21 11:32]
Ok, so I guess the points on which we agreed:
1. Call iroha library - iroha_core
2. Call iroha binary - iroha

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-15 18:48:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/1150" class=".btn">1150</a>
            </td>
            <td>
                <b>
                    Group 1000 blocks into each block file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span>
            </td>
            <td>
                Files in the block store should contain a configurable amount of blocks, with the default being 1000. This same number should be the number of blocks that new nodes on the network sync with other peers per syncing request.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-13 08:55:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/1149" class=".btn">1149</a>
            </td>
            <td>
                <b>
                    Limit Block Files to 1 million Per Folder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span>
            </td>
            <td>
                Block files in the blocks storage should be limited to 1 million blocks. If more than 1 million files are in a block storage folder, new folders should be created so the 1 million file limit is not violated.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-13 08:34:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/1139" class=".btn">1139</a>
            </td>
            <td>
                <b>
                    Set mintability of assets on asset creation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span>
            </td>
            <td>
                When assets are created, they should be able to be set as mintable or unmintable when creating the asset.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-12 11:42:31 +0000 UTC
    </div>
</div>

