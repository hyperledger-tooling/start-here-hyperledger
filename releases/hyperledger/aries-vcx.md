---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    Release 0.58.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.58.0
                </span>
            </td>
            <td>
                # New components
* Modular did:key representation by @mirgee in https://github.com/hyperledger/aries-vcx/pull/912

# Features
* Add interface to write DIDs on ledger by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/921
* Allow parsing unqualified DIDs by @mirgee in https://github.com/hyperledger/aries-vcx/pull/936
* Attempt to convert legacy DID documents to new during deserialization by @mirgee in https://github.com/hyperledger/aries-vcx/pull/938

# Refactoring
* Move PublicKey to a separate crate by @mirgee in https://github.com/hyperledger/aries-vcx/pull/911
* Allow storing resolvers with varying extra fields in the registry by @mirgee in https://github.com/hyperledger/aries-vcx/pull/913
* Eliminate dependence of indy-ledger-response-parser on indy-api-types by @mirgee in https://github.com/hyperledger/aries-vcx/pull/934
* Refactor test setup by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/921
* Extract subset of changes made in #928 by @mirgee in https://github.com/hyperledger/aries-vcx/pull/939
* Expose public key getter on verification method by @mirgee in https://github.com/hyperledger/aries-vcx/pull/941

# Dependencies
* Bump word-wrap from 1.2.3 to 1.2.5 in /wrappers/node by @dependabot in https://github.com/hyperledger/aries-vcx/pull/920
* Updated indy-credx by @bobozaur in https://github.com/hyperledger/aries-vcx/pull/931
* Update indy-vdr by @mirgee in https://github.com/hyperledger/aries-vcx/pull/935
* Try Hide indy-api-types from modular_libs consumers by @gmulhearn in https://github.com/hyperledger/aries-vcx/pull/940

# Changes
* Remove libvcx-c, libvcx java, libvcx ios by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/943
* Replace vdrtool ledger client by indy-vdr client by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/914

# Fixes
* fix(aries-vcx): fixed dependency listing in README for `Cargo.toml` by @arminveres in https://github.com/hyperledger/aries-vcx/pull/924

# Other
* Rebuild cargo.lock, restore indy-vdr-proxy txn submitter by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/932


## New Contributors
* @arminveres made their first contribution in https://github.com/hyperledger/aries-vcx/pull/924

**Full Changelog**: https://github.com/hyperledger/aries-vcx/compare/0.57.1...0.58.0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-vcx/releases/tag/0.58.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-08-21 22:20:22 +0000 UTC
    </span>
</div>

