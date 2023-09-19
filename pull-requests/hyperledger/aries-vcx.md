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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/985" class=".btn">#985</a>
            </td>
            <td>
                <b>
                    Remove agency client from libvcx-core tests and aries-vcx-agent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We are still setting up agency client in libvcx-core test code, although it is not used (in the tests).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-19 11:47:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/984" class=".btn">#984</a>
            </td>
            <td>
                <b>
                    Uniffi android controller
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Credits to @gmulhearn for simplifying the android code by adding a controller. :rocket: 
Merge after #970 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-18 09:18:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/983" class=".btn">#983</a>
            </td>
            <td>
                <b>
                    Integration test refactoring
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">refactoring</span>
            </td>
            <td>
                * Splits test helper functions doing multiple distinct operations and returning many-valued tuples into small, reusable functions returning objects
* Moves ledger tests from `aries_vcx/src/common/primitives/mod.rs` and `aries_vcx/src/common/primitives/revocation_registry_delta.rs` to `tests/test_pool.rs`.
* Localizes test helper functions like `create_indy_proof` which ended up used in one test suite.
* Leaves only generic test helpers in `aries_vcx/src/common/test_utils.rs`.
* Issuance and presentation test helpers are strictly accepting concrete message types instead of generic `AriesMessage` (without implementing message-specific methods on issuance and presentation handlers, which can be done separately).

Although further test refactoring is warranted, the aim of this PR is to focus on integration tests (only those in `aries_vcx/tests/`).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-18 06:54:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/982" class=".btn">#982</a>
            </td>
            <td>
                <b>
                    Implement encrypt_message for Connections with counterparty DidDoc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                yet to be polished up 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-15 23:10:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/981" class=".btn">#981</a>
            </td>
            <td>
                <b>
                    Minimize dependency on tokio
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Addressing https://github.com/hyperledger/aries-vcx/issues/947

- In `aries_vcx`, swapped tokio async sleeps for std blocking sleeps. This is okay because the sleep are only in test setup code, and these we run tests in single thread. If we gain capability to run tests in parallel, with a bit of effort, this can easily be update back to tokio sleeps (just need to properly feature flag the test setup code, which isn't the case today)

- in `aries_vcx_core`, swapped Mutex around cache for std lock. There was no need for tokio mutex, as the locks are not held across an await point
- in `aris_vcx_core`, the tokio import dependency is still declared, but limited to `sync` feature (for `upshot` module use by indy client implementations (`indy_vdr` tools internals require passing callbacks, not sure how difficult would those be to convert to async functions instead ) )

There's no changes visible to lock file because we declare dependency on tokio in other workspace projects (like uniffi, libvcx), but in external projects consuming `aries-vcx`, this should trim dependency tree (and likelyhood of dependency conflicts)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-15 22:41:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/980" class=".btn">#980</a>
            </td>
            <td>
                <b>
                    add cargo ndk build script for uniffi
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Credits to @gmulhearn  for simplifying the build process by using cargo-ndk. This PR integrates those changes and adds relevant documentation. 
Note:
The "other" scripts will be untracked once work on CI (UniFFI) is finished.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-15 13:16:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/979" class=".btn">#979</a>
            </td>
            <td>
                <b>
                    Further integration test refactoring
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Groups tests based on tested scenarios.
* Groups helper functions in `tests/scenarios` based on concern (connection, proof presentation, issuance).
* Extracts schema / credential data hardcoded across tests into one place.
* Multiple presentation generation tests (`test_agency_pool_proof_should_be_validated`, `test_agency_pool_generate_self_attested_proof`, `test_agency_pool_generate_proof_with_predicates`) were joined into one (`test_agency_pool_generate_proof`), adds generated proof verification.
* Many smaller tweaks and renames.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-15 09:32:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/978" class=".btn">#978</a>
            </td>
            <td>
                <b>
                    Expose wallet migration to node wrapper
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR exposes the wallet migration API to the node.js wrapper.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-14 10:35:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/977" class=".btn">#977</a>
            </td>
            <td>
                <b>
                    Add simple client implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Has majorly common code with mediator agent.
It's in essence one hybrid, with code organized separately. 
This is in anticipation of splitting client into separate binary.  

Then again, Aries agents are meant to be horizontal (p2p). So perhaps a multifunctional agent isn't all that odd.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-13 23:52:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/976" class=".btn">#976</a>
            </td>
            <td>
                <b>
                    Initial mediator work
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Display an OOB invitation. Also presented as QR!
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-13 16:08:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/975" class=".btn">#975</a>
            </td>
            <td>
                <b>
                    Remove `tokio`, `android_logger` deps from agency_client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - removes tokio dependency at cost of one test (very low value)
- also removed unused `android_logger` dependency
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-12 18:34:04 +0000 UTC
    </div>
</div>

