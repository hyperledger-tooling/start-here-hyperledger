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
                PR <a href="https://github.com/hyperledger/cactus/pull/1349" class=".btn">#1349</a>
            </td>
            <td>
                <b>
                    refactor (core-api): make schema names consistent in openapi spec 
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
        Created At 2021-09-17 16:24:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1348" class=".btn">#1348</a>
            </td>
            <td>
                <b>
                    docs(API-table): update API table and description
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - updated API table for socket.io verifier and validator.
- names are changed for consistency

This PR corresponds to issue #1320

Signed-off-by: Izuru Sato <sato.izuru@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-17 14:02:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1347" class=".btn">#1347</a>
            </td>
            <td>
                <b>
                    fix: endpoints implementation in corda plugin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #1346

Signed-off-by: Elena Izaguirre <e.izaguirre.equiza@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-17 08:18:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1345" class=".btn">#1345</a>
            </td>
            <td>
                <b>
                    build(deps): upgrade axios to latest to fix CVE
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">Security</span><span class="chip">dependent</span>
            </td>
            <td>
                Depends on #1344


Details
CVE-2021-3749
high severity
Vulnerable versions: <= 0.21.1
Patched version: 0.21.2
axios is vulnerable to Inefficient Regular Expression Complexity

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-17 00:45:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1344" class=".btn">#1344</a>
            </td>
            <td>
                <b>
                    build: downgrade to yarn v1.18.0 due to upgrade-interactive bug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">dependent</span>
            </td>
            <td>
                Depends on #1343

See: https://github.com/yarnpkg/yarn/issues/7807 for the root cause
and https://classic.yarnpkg.com/en/docs/cli/upgrade-interactive/
for more information about what yarn upgrade-interactive does.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-17 00:28:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1343" class=".btn">#1343</a>
            </td>
            <td>
                <b>
                    build(yarn): reset script now wipes node modules, yarn lock
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                Found myself in need of this when strange errors started occurring
between branch switches where the gRPC tooling was not installed
properly despite the configure script running successfully.
Now the reset is script is much more robust and it closer
resembles the outcome of a fresh clone.

Also: Ran the reset script and it updated the lock file, including
that in the commit as well to see if in the future othe reset runs
will also generate these/similar changes to the lock file or not.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-16 23:32:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1342" class=".btn">#1342</a>
            </td>
            <td>
                <b>
                    ci: set the swap file size to 10 GB for GitHub runners
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                This will hopefully alleviate the issue of some tests causing
out of memory crashes on the 7.5GB RAM GitHub Action Runners.

Could of course have a domino effect where the swap kicks in
and slows everything down so much that the tests just start
timing out instead of crashing with OOM ¯\_(ツ)_/¯

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-16 23:21:55 +0000 UTC
    </div>
</div>

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

