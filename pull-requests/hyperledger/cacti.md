---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2638" class=".btn">#2638</a>
            </td>
            <td>
                <b>
                    feat(weaver-corda): support array of remote views, consequent user fl…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …ow call
Closes #2470 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-24 12:13:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2637" class=".btn">#2637</a>
            </td>
            <td>
                <b>
                    ci(actionlint): add linting of GitHub action workflow files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2634

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-24 07:02:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2636" class=".btn">#2636</a>
            </td>
            <td>
                <b>
                    test(connector-quorum): fix flaky v2.3.0-deploy-contract-from-json-private.test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added an extra wait for the member 2 contract invocation
where we first obtain the receipt thereby forcing
the execution to wait until it has been mined on
member 2 as well.

Fixes #2635

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-24 06:46:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2633" class=".btn">#2633</a>
            </td>
            <td>
                <b>
                    ci(codegen)!: fix the yarn codegen job in ci.yaml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                BREAKING CHANGES:
1. Fabric connector endpoints are using base64 encoding instead of JSON
when needing to transfer otherwise binary data (UInt8Array)
2. Same as the above for the Iroha 1 and Iroha 2 connectors.

Primary changes:
-----------------
1. Removed the `"identifier": "Apache-2.0",` section from all OpenAPI
specification documents (./**/openapi.json) project-wide because the
OpenAPI generator is not yet compatible with it and because of that the
new property just makes it crash with a false-negative validation error.
2. Downgraded all OpenAPI specification documents version from `v3.1.0` to
`v3.0.3` (which is how it used to be) because the generator is not yet
compatible with it and it had caused types to be mangled.
3. Eliminated incorrect usage of the "format": "binary" declarations in
the OpenAPI specifications where the format was declared as binary but
the data was still traveling as JSON strings despite it (divergence
between our spec .json files and the implementation under the hood)
4. Updated the tests and their related endpoints to use base64 encoding
instead of JSON serializing UInt8Array instances: It is more efficient
this way and also has the benefit of honoring the specification. The
reason why it's more efficient is because JSON serializing a typed UInt8Array
results in an object literal that maps every single byte to a property
of said object, roughly tripling the size of the network transfer. It
probably also is slower to serialize/deserialize but I haven't actually
measured this.
5. All of the packages are now using the OpenAPI generator v6.6.0 instead
of some being stuck on v5.2.1. This might cause build issues in kotlin
API clients but because we don't have a freeze on breaking changes right
now (leading up to v2.0.0) it is the right time to make drastic changes
like this.

Fixes #2618

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-23 22:50:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2632" class=".btn">#2632</a>
            </td>
            <td>
                <b>
                    build(tools): fix tooling globs where cactus is hardcoded
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2576
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-23 05:51:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2631" class=".btn">#2631</a>
            </td>
            <td>
                <b>
                    feat(cactus-plugin-ledger-connector-ethereum): refactor connector API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Refactor to single `invokeContract` endpoint that can accept multiple methods of 
    supplying contract definition (directly, from keychain, etc..).
- Same for `deployContract` method.
- Update cactus-common `safeStringifyException` function to better handle axios errors
    (and other custom exceptions that support `toJSON()` method.).
- Use common error handling in all connector endpoints (except prometheus).
- Fix the tests.
- Switch to `Cacti` work in entire connector (except for package name)

Depends on: #2630

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-22 08:50:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2630" class=".btn">#2630</a>
            </td>
            <td>
                <b>
                    feat(cactus-plugin-ledger-connector-ethereum): support London fork gas prices
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add legacy and EIP1559 gas configuration options to transaction requests.
- Legacy gas configuration is updated to EIP1559 using the same logic as web3 libraries.
- Update the tests to work with new API.
- Added test suite to test new features - `geth-transact-and-gas-fees.test.ts`

Depends on: #2581

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-21 15:38:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2629" class=".btn">#2629</a>
            </td>
            <td>
                <b>
                    build(deps): overall minor upgrade of npm dependencies - 2023-08-18
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2627

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-20 09:45:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2628" class=".btn">#2628</a>
            </td>
            <td>
                <b>
                    test(connector-fabric): fix flaky test 2.2.x deploy-cc-from-javascript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary changes:
---------------

1. Added robust debug logging to the express middleware of the API server
so that problems like this are easier to debug in the future (e.g.
trouble with the Open API spec documents themselves)
2. Refactored the ci.yaml document so that there are separate jobs for
each tape based Fabric connector integration test. This has reduced
(or potentially eliminated) the presence of the flake that we were
encountering during the contract deployment test cases. It also has the
upside of faster CI because of more parallelism in the CI jobs.
3. Updated the assertions in a couple of test cases where the newer Fabric
versions were causing the assertions to fail because the returned JSON
response in the example asset transfer chaincode is now referring to the
asset owner via a property named "Owner" not "owner" (casing difference)

Fixes #1471

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-20 06:32:42 +0000 UTC
    </div>
</div>

