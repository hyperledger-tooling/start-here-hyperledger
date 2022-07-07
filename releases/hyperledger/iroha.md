---
layout: default
title: iroha
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/iroha
---

# iroha <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    Hyperledger Iroha 2.0.0-pre.rc.6-lts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v2.0.0-pre.rc.6
                </span>
            </td>
            <td>
                Long term-supported release candidate. We have reached a level of feature completeness, but want to ensure that things are working properly. This is the first major development milestone and we expect a lot of feedback with the option to re-architect some bits later down the line.

## What's Changed
* [refactor]: encapsulate access to data model structures by @mversic in https://github.com/hyperledger/iroha/pull/1984
* [feature] #2048: Add toolchain file by @Arjentix in https://github.com/hyperledger/iroha/pull/2049
* [feature] #1890: Introduce integration tests based on Orillion use-cases by @Arjentix in https://github.com/hyperledger/iroha/pull/2038
* [fix] #1917: Added easy_from_str_impl macro for use with AssetValueType by @SamHSmith in https://github.com/hyperledger/iroha/pull/2054
* [refactor]: Remove unnecessary `&mut` from the API. by @appetrosyan in https://github.com/hyperledger/iroha/pull/2057
* [feature] #2040: Add integration test with transaction execution limit by @Arjentix in https://github.com/hyperledger/iroha/pull/2051
* [feature] #1952: Add a TPS benchmark as a standard for optimizations by @s8sato in https://github.com/hyperledger/iroha/pull/1963
* [fix] #1623: Create a RawGenesisBlockBuilder by @SamHSmith in https://github.com/hyperledger/iroha/pull/2076
* [fix] #2005: Fix `Client::listen_for_events()` not closing WebSocket stream by @Arjentix in https://github.com/hyperledger/iroha/pull/2095
* DOPS-1722: CI for iroha2-longevity-load-rs by @BAStos525 in https://github.com/hyperledger/iroha/pull/2071
* DOPS-1722: CI for iroha2-longevity-load-rs by @BAStos525 in https://github.com/hyperledger/iroha/pull/2070
* [fix] #1845: Non-mintable assets can be minted once only. by @appetrosyan in https://github.com/hyperledger/iroha/pull/2044
* [feature] #2003: Introduce Parity Scale Decoder tool (stable implementation) by @Arjentix in https://github.com/hyperledger/iroha/pull/2080
* [refactor] #1982: encapsulate access to `iroha_crypto` structures by @mversic in https://github.com/hyperledger/iroha/pull/2077
* [refactor] #2109: Make `integration::events::pipeline` test stable by @s8sato in https://github.com/hyperledger/iroha/pull/2110
* [schema] #2108: Add pagination by @appetrosyan in https://github.com/hyperledger/iroha/pull/2107
* [schema] #2114: Sorted collections support in schemas by @mversic in https://github.com/hyperledger/iroha/pull/2115
* [ci]: Bump rust, mold and nightly to 1.60, 1.2.0 and 1.62 respectively. by @appetrosyan in https://github.com/hyperledger/iroha/pull/2129
* [documentation] Add samhsmith to codeowners file by @SamHSmith in https://github.com/hyperledger/iroha/pull/2131
* [fix] #2111: Remove `roles` feature by @Arjentix in https://github.com/hyperledger/iroha/pull/2134
* [fix] #1716: Fix consensus failure with f=0 cases by @s8sato in https://github.com/hyperledger/iroha/pull/2124
* [documentation]: Add QuentinI to codeowners file by @QuentinI in https://github.com/hyperledger/iroha/pull/2138
* [feature] #2099: Add WASM integration test based on Orillion use-case by @Arjentix in https://github.com/hyperledger/iroha/pull/2122
* [feature] #2121: Check keypair is valid when constructed by @mversic in https://github.com/hyperledger/iroha/pull/2130
* [fix] #1640: Generate `genesis.json` and consolidate generation into one tool by @appetrosyan in https://github.com/hyperledger/iroha/pull/2104
* [refactor] #2144: redesign client's http workflow, expose internal api by @0x009922 in https://github.com/hyperledger/iroha/pull/2147
* [documentation] #1991: Add readme to Kura inspector by @outoftardis in https://github.com/hyperledger/iroha/pull/2162
* [ci] #2153: Fix coverage by @s8sato in https://github.com/hyperledger/iroha/pull/2154
* [ci]: Fix deploy pipeline. by @appetrosyan in https://github.com/hyperledger/iroha/pull/2168
* [documentation]: Add Ekaterina to the list of codeowners by @outoftardis in https://github.com/hyperledger/iroha/pull/2171
* [feature]: #1572: Specialized permission tokens by @QuentinI in https://github.com/hyperledger/iroha/pull/2156
* [ci]: Version bump all of the crates. by @appetrosyan in https://github.com/hyperledger/iroha/pull/2174
* [documentation] #2177: Clean up gitchangelog output by @outoftardis in https://github.com/hyperledger/iroha/pull/2178
* [ci] #2153: Fix #2154 by @s8sato in https://github.com/hyperledger/iroha/pull/2166
* [feature] #2050: Add role-related queries. by @appetrosyan in https://github.com/hyperledger/iroha/pull/2126
* [feature] #2105: handle query errors in client by @0x009922 in https://github.com/hyperledger/iroha/pull/2160
* [feature] #2004: Forbid `isize` and `usize` from becoming `IntoSchema`. by @appetrosyan in https://github.com/hyperledger/iroha/pull/2173
* [documentation] #2113: Document features in Cargo.toml files by @outoftardis in https://github.com/hyperledger/iroha/pull/2180
* [feature] #1883: Remove embedded configuration files. by @appetrosyan in https://github.com/hyperledger/iroha/pull/2183
* [fix] #2150: Use `rustfmt` instead of `cargo fmt` in `client/build.rs` by @Arjentix in https://github.com/hyperledger/iroha/pull/2187
* [fix] #2159: Improve `parity_scale_decoder` tests by @Arjentix in https://github.com/hyperledger/iroha/pull/2184
* [documentation] #2181: Review README by @outoftardis in https://github.com/hyperledger/iroha/pull/2190
* [feature] #2179: Optimise trigger execution by @Arjentix in https://github.com/hyperledger/iroha/pull/2157
* [fix] #1990: Enable peer startup via env vars in the absence of `config.json` by @ilchu in https://github.com/hyperledger/iroha/pull/2188
* [documentation] #2119: Add guidance on how to hot reload Iroha in a Docker container by @outoftardis in https://github.com/hyperledger/iroha/pull/2196
* [feature] #2100: Add query to find all accounts with asset by @Arjentix in https://github.com/hyperledger/iroha/pull/2197
* I2 dco by @appetrosyan in https://github.com/hyperledger/iroha/pull/2209
* [feature] #2056: Add a derive proc macro crate for AssetValueType enum by @ilchu in https://github.com/hyperledger/iroha/pull/2213
* [fix] #2215: Make nightly optional for building Iroha. by @appetrosyan in https://github.com/hyperledger/iroha/pull/2217
* [documentation] #1280: Document Iroha metrics by @outoftardis in https://github.com/hyperledger/iroha/pull/2195
* [feature] #2186: Add transfer instructions for all asset types by @appetrosyan in https://github.com/hyperledger/iroha/pull/2185
* [documentation] #2192: Review contributing guidelines by @outoftardis in https://github.com/hyperledger/iroha/pull/2219
* [documentation] #2193: Update benchmarks documentation by @outoftardis in https://github.com/hyperledger/iroha/pull/2230
* [refactor] #2145: refactor client's `WebSocket` side, extract pure data logic by @0x009922 in https://github.com/hyperledger/iroha/pull/2146
* [documentation] #2193: Update Kagami documentation by @outoftardis in https://github.com/hyperledger/iroha/pull/2220
* [fix] #2170: Fixes build in docker container on M1 machines by @pesterev in https://github.com/hyperledger/iroha/pull/2237
* [feature] #2103: support querying for blocks and transactions by @QuentinI in https://github.com/hyperledger/iroha/pull/2210
* [feature] #1413: Add API version endpoint by @ilchu in https://github.com/hyperledger/iroha/pull/2235
* [refactor]: Move `TriggerSet` to `data_model` by @Arjentix in https://github.com/hyperledger/iroha/pull/2229
* [ci] #2222: Split tests by whether it involves coverage or not by @s8sato in https://github.com/hyperledger/iroha/pull/2223
* [documentation] #2193: Update Parity Scale Decoder Tool documentation by @outoftardis in https://github.com/hyperledger/iroha/pull/2224
* [fix] #2232: Make Iroha print meaningful message when genesis has too many isi by @Arjentix in https://github.com/hyperledger/iroha/pull/2239
* [feature] #1149: Restrict block number to 1 million per dir by @SamHSmith in https://github.com/hyperledger/iroha/pull/2194
* [documentation] #2193: Update README for wasm crate by @outoftardis in https://github.com/hyperledger/iroha/pull/2240
* [documentation] #2193: Update README for macro crate by @outoftardis in https://github.com/hyperledger/iroha/pull/2236
* [fix] #1149: Remove nocheckin code by @SamHSmith in https://github.com/hyperledger/iroha/pull/2248
* [documentation] #2193: Update Iroha CLI documentation by @outoftardis in https://github.com/hyperledger/iroha/pull/2244
* [documentation] #2193: Update Iroha Client and Iroha CLI Client documentation by @outoftardis in https://github.com/hyperledger/iroha/pull/2234
* [documentation]: Flakyness report by @appetrosyan in https://github.com/hyperledger/iroha/pull/2246
* [feature] #2161: generate FFI functions for `data_model` by @mversic in https://github.com/hyperledger/iroha/pull/2211
* [documentation]: Update information on git hooks by @outoftardis in https://github.com/hyperledger/iroha/pull/2254
* [feature] #1926: Add signal handling and graceful shutdown by @pesterev in https://github.com/hyperledger/iroha/pull/2251
* [feature] #2125: Add FindAssetDefinitionById query by @pesterev in https://github.com/hyperledger/iroha/pull/2265
* [test] #2272: Add tests for 'FindAssetDefinitionById' query by @pesterev in https://github.com/hyperledger/iroha/pull/2273
* [feature] #2257: Revoke<Role> emits RoleRevoked event by @omkar-mohanty in https://github.com/hyperledger/iroha/pull/2264
* [ci]: Remove unnecessary coverage reporting. by @appetrosyan in https://github.com/hyperledger/iroha/pull/2271
* [feature] #2132: Add `endpointN` proc macro by @ilchu in https://github.com/hyperledger/iroha/pull/2258
* [fix] #2282: improve FFI derives from getset implementation by @mversic in https://github.com/hyperledger/iroha/pull/2283
* [feature] #1638: `configuration` return doc subtree by @ilchu in https://github.com/hyperledger/iroha/pull/2291
* [ci]: Add @ilchu to codeowners by @ilchu in https://github.com/hyperledger/iroha/pull/2298
* [refactor]: Refactor around `QueryError` by @s8sato in https://github.com/hyperledger/iroha/pull/2281
* [fix] #2295: Fix unregister trigger bug by @Arjentix in https://github.com/hyperledger/iroha/pull/2297
* [feature] #2161: Handle id and shared FFI fns by @mversic in https://github.com/hyperledger/iroha/pull/2274
* [refactor] #1896: Simplify `produce_event` implementation by @Erigara in https://github.com/hyperledger/iroha/pull/2305
* [fix] #2303: Fix docker-compose' peers doesn't get gracefully shut down by @pesterev in https://github.com/hyperledger/iroha/pull/2311
* [fix] #2017: Fix role unregistration by @Erigara in https://github.com/hyperledger/iroha/pull/2313
* [fix] #2081: Fix the test case to grant the role by @s8sato in https://github.com/hyperledger/iroha/pull/2312
* [refactor] #2011: More descriptive config params by @ilchu in https://github.com/hyperledger/iroha/pull/2319
* [refactor] #2238: Add peer builder for tests by @pesterev in https://github.com/hyperledger/iroha/pull/2304
* [feature] #2276: Include current Block hash into BlockHeaderValue by @omkar-mohanty in https://github.com/hyperledger/iroha/pull/2285
* [refactor] #2323: Enhance kura init error message by @ilchu in https://github.com/hyperledger/iroha/pull/2329
* [ci]: Version bump of crates and remove unused dependencies by @appetrosyan in https://github.com/hyperledger/iroha/pull/2331
* [documentation]: Add links to the tutorial by @outoftardis in https://github.com/hyperledger/iroha/pull/2337
* [documentation]: Updates codeowners by @pesterev in https://github.com/hyperledger/iroha/pull/2341
* [feature] #1998: Add filters to queries by @appetrosyan in https://github.com/hyperledger/iroha/pull/2270
* [documentation]: Add @Erigara to CODEOWNERS by @Erigara in https://github.com/hyperledger/iroha/pull/2348
* [fix] #2202: Fix total field in query response by @Erigara in https://github.com/hyperledger/iroha/pull/2346
* [feature] #2302: Add 'FindTriggersByDomainId' stub-query by @pesterev in https://github.com/hyperledger/iroha/pull/2342
* [fix] #2294: Add flamegraph generation to oneshot.rs by @SamHSmith in https://github.com/hyperledger/iroha/pull/2324
* [documentation] #2344: Generate CHANGELOG for 2.0.0-pre-rc.5-lts by @outoftardis in https://github.com/hyperledger/iroha/pull/2349
* [refactor] #2204: Make Asset-related operations generic by @Erigara in https://github.com/hyperledger/iroha/pull/2328
* [fix] #2358: Add release with debug profile by @SamHSmith in https://github.com/hyperledger/iroha/pull/2359
* [refactor]: Remove generics from `IsAllowedBoxed` by @Arjentix in https://github.com/hyperledger/iroha/pull/2284
* [refactor]: add permission token wrappers for private_blockchain by @QuentinI in https://github.com/hyperledger/iroha/pull/2354
* [feature] #2053: Add tests to 'private_blockchain' by @pesterev in https://github.com/hyperledger/iroha/pull/2332
* [ci] #1658: Add documentation check by @ales-tsurko in https://github.com/hyperledger/iroha/pull/2367
* [feature] #2053: Add tests to the asset-related queries in private blockchain by @pesterev in https://github.com/hyperledger/iroha/pull/2374
* [fix] #2081: Fix role granting bug by @Arjentix in https://github.com/hyperledger/iroha/pull/2371
* [feature] #2053: Add tests to all remaining queries in private blockchain by @pesterev in https://github.com/hyperledger/iroha/pull/2383
* [Release]: Pre-rc.5 by @appetrosyan in https://github.com/hyperledger/iroha/pull/2343
* [fix] #2227: Implement Register and Unregister for Asset by @QuentinI in https://github.com/hyperledger/iroha/pull/2333
* [refactor] #1985: Reduce size of `Name` struct by @Erigara in https://github.com/hyperledger/iroha/pull/2365
* [fix] #2137: Prepare tests for multiprocess context by @ales-tsurko in https://github.com/hyperledger/iroha/pull/2363
* [feature] #2360: Make `genesis.json` optional again by @ilchu in https://github.com/hyperledger/iroha/pull/2390
* [fix] #2128: Fix `MerkleTree` construction and iteration by @s8sato in https://github.com/hyperledger/iroha/pull/2318
* [ci] #2393: Bump the version of the Docker base image by @s8sato in https://github.com/hyperledger/iroha/pull/2394
* [feature] #2127: Add sanity check to ensure that all data decoded by `parity_scale_codec` is consumed by @Arjentix in https://github.com/hyperledger/iroha/pull/2378
* [release]: 2.0.0-pre-rc.6-lts by @appetrosyan in https://github.com/hyperledger/iroha/pull/2423

## New Contributors
* @BAStos525 made their first contribution in https://github.com/hyperledger/iroha/pull/2071
* @outoftardis made their first contribution in https://github.com/hyperledger/iroha/pull/2162
* @pesterev made their first contribution in https://github.com/hyperledger/iroha/pull/2237
* @omkar-mohanty made their first contribution in https://github.com/hyperledger/iroha/pull/2264

**Full Changelog**: https://github.com/hyperledger/iroha/compare/v2.0.0-pre-rc.3...v2.0.0-pre.rc.6
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/iroha/releases/tag/v2.0.0-pre.rc.6" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-07-04 14:31:54 +0000 UTC
    </span>
</div>

