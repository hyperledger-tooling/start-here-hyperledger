---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/927" class=".btn">#927</a>
            </td>
            <td>
                <b>
                    Use credx anoncreds in napi wrapper
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
        Created At 2023-08-09 22:47:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/925" class=".btn">#925</a>
            </td>
            <td>
                <b>
                    Remove init_issuer_config function
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
        Created At 2023-08-05 18:00:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/924" class=".btn">#924</a>
            </td>
            <td>
                <b>
                    fix(aries-vcx): fixed dependency listing in README for `Cargo.toml`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Using path does not work and crates from git sources need be specified through `git=...`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-04 17:38:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/923" class=".btn">#923</a>
            </td>
            <td>
                <b>
                    Draft: issue 922 Prover revocation states fix up
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #922 

TODO
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-04 10:15:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/921" class=".btn">#921</a>
            </td>
            <td>
                <b>
                    Refactor test setup, add interface to write DIDs on ledger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add interface to write endorser DIDs on Indy ledger `write_endorser_did`
- In order to reasonably implement its test `test_pool_write_new_endorser_did` I have refactored code related to test setup - mainly separating building "Profiles" from building and setting up wallet. This the mentioned test to create one instance of "Faber agent" with known trusteee DID, and one instance of "Faber agent" with a random did in its wallet.
- Change `libvcx` function `wallet_create_pairwise_did` to `wallet_create_and_store_did(seed: Option<&str>)` - the original name is bit deceiving, sometimes you just want to generate a key even when and you are not dealing with any pairwise relationship. So this name is more general and also provide option to pass in seed for did/verkey generation.
- Minor CI improvements - making `needs` declaration bit simpler and consistent
- Added some integration tests directly to `node` wrapper, rather than propagating the APIs to `vcxagent-core`.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-03 19:01:52 +0000 UTC
    </div>
</div>

