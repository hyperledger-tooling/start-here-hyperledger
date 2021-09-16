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
                PR <a href="https://github.com/hyperledger/cactus/pull/1340" class=".btn">#1340</a>
            </td>
            <td>
                <b>
                    style(js-object-signer): removed all "unexpected any" types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Made all "any" types either explicit or unknown (where possible)
Allowed for private keys to be passed as either byte arrays (Buffer falls under this too) or strings

Resolves #1338
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-16 16:22:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1339" class=".btn">#1339</a>
            </td>
            <td>
                <b>
                    ci: add DCI-Lint GitHub action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Depends on #1334 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-15 20:08:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1337" class=".btn">#1337</a>
            </td>
            <td>
                <b>
                    Quorum private transaction
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #951 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-15 14:05:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1336" class=".btn">#1336</a>
            </td>
            <td>
                <b>
                    feat(ci): skip check when only documentation files #1014
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolve #1014 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-15 08:14:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1335" class=".btn">#1335</a>
            </td>
            <td>
                <b>
                    ci: re-enable image caching, skip flaky tests #1334
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                1. Disables the coverage check of tap.
2. Starts skipping failing tests
3. Re-enables container image caching

Fixes #1334

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-15 02:25:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1333" class=".btn">#1333</a>
            </td>
            <td>
                <b>
                    feat(connector-fabric): support FabricSigningCredentialType.WsX509
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                New feature for fabric connector. identity provider for external clients using a web-socket connection.
    - Connect external clients to a fabric ca server
        (1) setup FabricSocketServer on ca host
        (2) create external web-socket client with pub/priv key pair
        (3) pass pubkey hex to socket server to issue unique web-socket sessionId
        (4) open authenticated sessionId including signed sessionId in url parameters of initial web-socket connection request
    - Use fabric plugin with FabricSigningCredentialType.WsX509 to
        - enroll registrar with admin password and admin's external pkey
        - register new user with admins external pkey and secret
        - enroll new user with user external pkey and secret
        - submit transactions
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 21:55:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1332" class=".btn">#1332</a>
            </td>
            <td>
                <b>
                    fix: openapi validation test for iroha plugin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Iroha</span>
            </td>
            <td>
                Includes test for endpoint runTransactionV1
with test cases:
  - Right request
  - Request including an invalid parameter
  - Request without a required parameter

Closes #1331

Related with #847

Signed-off-by: Elena Izaguirre <e.izaguirre.equiza@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 11:45:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1330" class=".btn">#1330</a>
            </td>
            <td>
                <b>
                    fix: openapi validation test for keychain-vault plugin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Includes tests for endpoints setKeychainEntryV1,
getKeychainEntryV1, deleteKeychainEntryV1 and
hasKeychainEntryV1, each of them, when appropiate,
with test cases:
  - Right request
  - Request including an invalid parameter
  - Request without a required parameter

Closes #1329

Relationed with #847

Signed-off-by: Elena Izaguirre <e.izaguirre.equiza@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 09:01:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1327" class=".btn">#1327</a>
            </td>
            <td>
                <b>
                    feat(validator): Iroha validator using python
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Hyperledger Iroha Validator
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 05:18:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1323" class=".btn">#1323</a>
            </td>
            <td>
                <b>
                    chore(deps): upgrade Web3 to v1.5.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">Security</span><span class="chip">dependent</span>
            </td>
            <td>
                Hoping that this will fix a good chunk of the outstanding
security vulnerabilities that we have.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

Depends on #1335 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-12 04:02:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1318" class=".btn">#1318</a>
            </td>
            <td>
                <b>
                    docs(dev-container): fix Unable to access jarfile openapi-generator-c…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">documentation</span>
            </td>
            <td>
                …li/versions/5.2.0.jar #1317

The OpenAPI generator versions were out of sync, unified it on 5.2.0 and now the dev container
does not have any issue configuring itself upon a successful boot.

Fixes #1317

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 22:03:30 +0000 UTC
    </div>
</div>

