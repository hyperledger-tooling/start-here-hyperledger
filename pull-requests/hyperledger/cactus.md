---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1041" class=".btn">#1041</a>
            </td>
            <td>
                <b>
                    feat(core-api): discontinue dedicated HTTP listeners for web service plugins
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: TonyRowntree <33454202+TonyRowntree@users.noreply.github.com>

Draft PR will amend when changed

resolves #358 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-15 13:33:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1038" class=".btn">#1038</a>
            </td>
            <td>
                <b>
                    docs(examples): fix typos and backend build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Fixed Typos with logLevel
- Fixed fabric chaincode deployment error

Signed-off-by: Pritam Singh <pkspritam16@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-15 04:45:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1037" class=".btn">#1037</a>
            </td>
            <td>
                <b>
                    test: add logLevel parameter to Fabric AIO ctor calls
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span><span class="chip">SPIKE</span>
            </td>
            <td>
                This is another step taken to win the epic battle that we have been
waging against a particularly nasty test flake that is plaguing the
Fabric tests that use the AIO ledger.

This will make the test output much more verbose, but there's no other
way around to making sure that we can narrow down the root cause of the
flake to a specific issue.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-15 02:55:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1033" class=".btn">#1033</a>
            </td>
            <td>
                <b>
                    feat(test-tooling): go-ipfs test container
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span><span class="chip">enhancement</span>
            </td>
            <td>
                New utility class that can manage the life-cycle of a go-ipfs container.
It uses the official go-ipfs container image under the hood not a
custom one like the AIO images.

The purpose of this is to help authoring test cases in the future
related to IPFS of which a good example will be the IPFS
object-store plugin's implementation.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-14 20:10:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1032" class=".btn">#1032</a>
            </td>
            <td>
                <b>
                    feat(core-api): add plugin object store interface definition
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Core_API</span><span class="chip">enhancement</span>
            </td>
            <td>
                This will be implemented by object store plugins so as to
have guarantee that at runtime the plugins can be used the
way the caller expects them to.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-14 20:06:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1031" class=".btn">#1031</a>
            </td>
            <td>
                <b>
                    docs(contributing.md): explicit recommendation for avoiding global dependencies #585
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span>
            </td>
            <td>
                docs(contributing.md): explicit recommendation for avoiding global dependencies #585

Signed-off-by: Zachary Villanueva <Zachary.Villanueva@ibm.com>

Fixes #585 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-14 19:08:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1030" class=".btn">#1030</a>
            </td>
            <td>
                <b>
                    style(corda): linter fix deploy contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Youngone Lee <youngone.lee@accenture.com>

pinged @petermetz because I don't have review section 😢 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-14 14:09:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1024" class=".btn">#1024</a>
            </td>
            <td>
                <b>
                    feat(iroha-testnet): Add REJECT check for transactions to setup-iroha-wallet.sh script in iroha-testnet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                feat(iroha-testnet): Add REJECT check for transactions to setup-iroha-wallet.sh script in iroha-testnet

Signed-off-by: Takeshi Yonezu <tkyonezu@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-12 14:26:49 +0000 UTC
    </div>
</div>

