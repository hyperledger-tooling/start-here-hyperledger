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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1306" class=".btn">#1306</a>
            </td>
            <td>
                <b>
                    feat!: add data, cache and temp dirs to FileSystem
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Files created by the framework have different nature, and in this PR we introduce three categories:

- **data**: intended to be persistent and included in OS backups. For instance, wallet contents (used by default for Askar-based wallets)
- **cache**: files intended to be persistent, but that can be regenerated or re-downloaded. An example of this are the tails files for AnonCreds
- **temp**: temporary files that can be safely deleted by the OS after usage. For instance, the genesis file created from genesisTransactions or wallet backup generated during migration

Another change from current behaviour is that all files created by the framework are contained within `basePath/.afj` directory. This is somewhat similar to indy-sdk, which creates a `homedir/.indy_client`. 

Some remaining questions:

- Will it be necessary to write migration scripts to move files (if existant) to new directories? Probably not, considering that until now all files created by AFJ are either temporary or cache
- Is it OK to use user home directory and Document directory as a base for data in (node and react-native respectively)? This selection and categorization is based on [iOS storage guidelines](https://developer.apple.com/documentation/foundation/optimizing_your_app_s_data_for_icloud_backup/)  
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 02:50:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1303" class=".btn">#1303</a>
            </td>
            <td>
                <b>
                    fix: imports from core
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These are preventing `@aries-framework/anoncreds-rs` and `@aries-framework/askar` from bein properly imported. 

Also removes the outdated `AskarModuleConfig`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-14 21:52:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1301" class=".btn">#1301</a>
            </td>
            <td>
                <b>
                    feat(askar): createKey from secret bytes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is being added to provide a way of creating deterministic keys in a similar way than indy-sdk, as our [current findings](https://github.com/hyperledger/aries-cloudagent-python/blob/467104fab662507e18483abaaf2305bc702bb303/aries_cloudagent/wallet/askar.py#L751) are that it is actually using the seed as a secret key.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-14 16:19:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1298" class=".btn">#1298</a>
            </td>
            <td>
                <b>
                    docs: update readme
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
        Created At 2023-02-14 08:30:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1295" class=".btn">#1295</a>
            </td>
            <td>
                <b>
                    fix(askar): generate nonce suitable for anoncreds
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The one that was returned by `AskarWallet.generateNonce()` is not usable for AnonCreds proofs and credential issuance flow, so it is now adjusted to return something equivalent to what's in IndyWallet or anoncreds-rs.

As part of a further refactor, this functionality will be most likely moved to `anoncreds` package, as it is more related to AnonCreds specification than the Wallet itself.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-13 20:48:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1294" class=".btn">#1294</a>
            </td>
            <td>
                <b>
                    test: add anoncreds restriction test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Some small changes and an extra test to test anoncreds restriction transformation
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-13 17:45:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1293" class=".btn">#1293</a>
            </td>
            <td>
                <b>
                    build(indy-sdk): set private to false
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim Stekelenburg <karim@animo.id>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-13 14:09:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1292" class=".btn">#1292</a>
            </td>
            <td>
                <b>
                    chore: make askar, anoncreds(-rs), indy-vdr packages public
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ariel Gentile <gentilester@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-13 11:44:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1291" class=".btn">#1291</a>
            </td>
            <td>
                <b>
                    fix(indy-vdr): export relevant packages from root
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds missing exports to the `indy-vdr` package's public API.

Signed-off-by: Karim Stekelenburg <karim@animo.id>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-13 11:06:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1290" class=".btn">#1290</a>
            </td>
            <td>
                <b>
                    feat: add fetch indy schema method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements the `fetchIndySchema` method which fetches the actual schema ID for the `getCredentialDefinition` method in the` IndySdkAnonCredsRegistry` and  `IndyVdrAnonCredsRegistry`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-13 08:00:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1289" class=".btn">#1289</a>
            </td>
            <td>
                <b>
                    feat: indy sdk aries askar migration script
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - feat: setup package
- feat: setup some base components

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-12 20:40:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1288" class=".btn">#1288</a>
            </td>
            <td>
                <b>
                    chore(core): remove useless file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: blu3beri <blu3beri@proton.me>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-12 20:02:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1286" class=".btn">#1286</a>
            </td>
            <td>
                <b>
                    refactor!: remove indy from core
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Completely broken at the moment. Not ready yet

Dependant on #1279 and #1283 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-10 15:49:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1285" class=".btn">#1285</a>
            </td>
            <td>
                <b>
                    feat: indy-vdr module registration
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
        Created At 2023-02-10 14:07:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1283" class=".btn">#1283</a>
            </td>
            <td>
                <b>
                    feat(anoncreds): legacy indy proof format service
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds a `LegacyIndyProofFormatService` that can be used with v1 and v2 of the proof protocol.

I've made some improvements to the tails handling and it now verifies the hash after downloading. 

There's some high level tests that use both the legacy indy credential format service and the legacy indy proof format service to do the full flow of issuance and verification. It's a bit hard to test in isolation with the indy-sdk, but we can change that once we have the AnonCredsRs backend.

Dependant on #1279
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-10 02:14:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1282" class=".btn">#1282</a>
            </td>
            <td>
                <b>
                    feat: add devcontainer support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Initial work on adding devcontainer support to make development easier for Mac, Windows and Linux. The [Dockerfile](.devcontainer/Dockerfile) located in the `.devcontainer` directory is used to build the working container.

Fixes #1281

![screenshot](https://user-images.githubusercontent.com/390891/217969554-e7e530dc-fada-40db-bd33-35938b4f1290.jpg)


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-10 00:18:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1280" class=".btn">#1280</a>
            </td>
            <td>
                <b>
                    ci: increase maximum heap memory for node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Attempt to increase maximum heap memory available for node, as CI is consistently failing when reaching around 1.8 GB under node 18.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-09 22:27:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1279" class=".btn">#1279</a>
            </td>
            <td>
                <b>
                    refactor(proofs)!: generalize proofs api and improve consistency with credentials module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This refactors the proofs api to be more generic and allow dynamic registration of formats (which we need for the anoncreds works) in addition with making it consistent with the credentials module. With all the refactoring over the last year, although they followed the same patterns they became somewhat inconsistent.

This is based on the DIF Presentation exchange branch from @NB-MikeRichardson, but doesn't include the Presentation Exchange work yet. I've done this to avoid the need for refactoring in the presentation exchange branch.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-09 14:00:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1278" class=".btn">#1278</a>
            </td>
            <td>
                <b>
                    feat: added endpoint setter to agent InitConfig
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jim Ezesinachi <jim@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-09 13:53:47 +0000 UTC
    </div>
</div>

