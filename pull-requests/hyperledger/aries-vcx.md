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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/673" class=".btn">#673</a>
            </td>
            <td>
                <b>
                    Create integration test on top of aries-vcx-agent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Create integration test on top of aries-vcx-agent
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-29 18:00:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/672" class=".btn">#672</a>
            </td>
            <td>
                <b>
                    get_service was modified, to first retrieve the attrib endpoint, in c…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …ase it does not find a search for service.

A new add_service_public method was added, which generates information in the ledger with this structure

    "endpoint": {
        "endpoint": "https://example.com",
        "types": [ "endpoint", "did-communication", "DIDComm"],
        "routingKeys": [ "did:key12345", "did:key12345" ]
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-28 22:46:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/671" class=".btn">#671</a>
            </td>
            <td>
                <b>
                    Implement Storage trait for agent's ObjectCache
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">agents</span>
            </td>
            <td>
                Adds a Storage trait and implements it for Rust agent's ObjectCache. This may eventually allow for multiple storage implementations.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-28 20:15:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/670" class=".btn">#670</a>
            </td>
            <td>
                <b>
                    Remove ios wrapper indysdk
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
        Created At 2022-11-28 16:20:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/668" class=".btn">#668</a>
            </td>
            <td>
                <b>
                    revealed parameter in prover building proof
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Pompeo Faruolo <pompeo.faruolo@etuitus.it>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-28 07:45:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/667" class=".btn">#667</a>
            </td>
            <td>
                <b>
                    Validated some parameters passed as a JSON string.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Remove of the FFI layer also removed some validations of parameters passed as a JSON strings. This PR restore missed validations.

Signed-off-by: Artem Mironov <artem.mironov@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-27 21:14:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/666" class=".btn">#666</a>
            </td>
            <td>
                <b>
                    Set indy wallet master secret
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Set indy wallet master secret
master_secret parameter has been added to wallet config
Master secret is used in some methods where the wallet config is not there,
then has been added a global access to master secret of each wallet
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-27 05:52:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/665" class=".btn">#665</a>
            </td>
            <td>
                <b>
                    Generate node bindings using napi-rs - separate crate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">wrappers</span>
            </td>
            <td>
                Based on approach taken by #661, but moving node API to a separate crate in order to minimize impact of NAPI boilerplate on libvcx.

Signed-off-by: Miroslav Kovar <miroslav.kovar@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-25 14:28:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/664" class=".btn">#664</a>
            </td>
            <td>
                <b>
                    Do not try to publish libvcx image from fork PRs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">skip-ios</span><span class="chip">skip-android</span>
            </td>
            <td>
                If PR is made from a repo fork, it currently always fails on attempt to publish to docker registry. This PR makes the step conditional

Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-24 22:16:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/663" class=".btn">#663</a>
            </td>
            <td>
                <b>
                    iOS Wrapper
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">skip-android</span>
            </td>
            <td>
                - Renamed ConnectMeVcx to VcxAPI
- Added type to parameters on function setLogger in VcxLogger
- Added/exposed new functions to VcxAPI (equalized like in wrappers/node/src/rustlib.ts) related to OOB, Proof, CredDef, Schema etc.
- Created VcxWrapperCallbacks.(h/m) to organize and reduce the code of VcxAPI (old ConnectMeVcx) file
- Organized some imports and cleaned some code
- Moved some type definitions from VcxAPI (old ConnectMeVcx) to VcxTypes
- Redefined VcxHandle type to be unsigned int
- Redefined type of all handles (connection, proof etc.) parameters on input and completion functions, in VcxAPI, to NSUInteger
- Replaced deprecated function vcx_connection_create_with_connection_request by vcx_connection_create_with_connection_request_v2 in libvcx.h and VcxAPI
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-24 18:45:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/662" class=".btn">#662</a>
            </td>
            <td>
                <b>
                    Add other mime type for attributes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">skip-ios</span><span class="chip">skip-android</span>
            </td>
            <td>
                Handles the receipt of offers and credentials

Signed-off-by: Pompeo Faruolo <pompeo.faruolo@etuitus.it>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-24 06:35:48 +0000 UTC
    </div>
</div>

