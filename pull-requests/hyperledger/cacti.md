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
                PR <a href="https://github.com/hyperledger/cacti/pull/2647" class=".btn">#2647</a>
            </td>
            <td>
                <b>
                    build(deps): bump gopkg.in/yaml.v3 from 3.0.0-20200313102051-9f266ea9e77c to 3.0.0 in /weaver/sdks/fabric/go-sdk
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps gopkg.in/yaml.v3 from 3.0.0-20200313102051-9f266ea9e77c to 3.0.0.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=gopkg.in/yaml.v3&package-manager=go_modules&previous-version=3.0.0-20200313102051-9f266ea9e77c&new-version=3.0.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

Dependabot will resolve any conflicts with this PR as long as you don't alter it yourself. You can also trigger a rebase manually by commenting `@dependabot rebase`.

[//]: # (dependabot-automerge-start)
[//]: # (dependabot-automerge-end)

---

<details>
<summary>Dependabot commands and options</summary>
<br />

You can trigger Dependabot actions by commenting on this PR:
- `@dependabot rebase` will rebase this PR
- `@dependabot recreate` will recreate this PR, overwriting any edits that have been made to it
- `@dependabot merge` will merge this PR after your CI passes on it
- `@dependabot squash and merge` will squash and merge this PR after your CI passes on it
- `@dependabot cancel merge` will cancel a previously requested merge and block automerging
- `@dependabot reopen` will reopen this PR if it is closed
- `@dependabot close` will close this PR and stop Dependabot recreating it. You can achieve the same result by closing it manually
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-30 13:59:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2646" class=".btn">#2646</a>
            </td>
            <td>
                <b>
                    chore(besu): remove web3-eea typings file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1218

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-30 06:16:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2645" class=".btn">#2645</a>
            </td>
            <td>
                <b>
                    feat(cactus-plugin-ledger-connector-fabric-socketio): remove fabric-socketio connector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Remove cactus-plugin-ledger-connector-fabric-socketio connector.
- Refactor discounted cartrade sample to use openapi fabric connector instead of fabric-socketio.
    Sample app will use delegated signing, similar to offline signing in old connector.
- Remove dead code from cmd-socketio-server
- Update fabric SDK to 2.X in all cacti projects, refactor code that use it where necessary.
    Only exception is fabric persistence plugin which uses fabric SDK as dev dependency (for tests).
    It can be updated in separate PR later on.

Depends on: #2644

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-29 12:29:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2644" class=".btn">#2644</a>
            </td>
            <td>
                <b>
                    feat(cactus-plugin-ledger-connector-fabric): support delegated (offline) signatures
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add new `RunDelegatedSignTransactionEndpointV1` endpoint for delegated / offline signing.
    Takes `signerCertificate` and `signerMspID`, uses `signCallback` on connector to sign messages.
    Sign must be implemented by a user, can contain any logic 
    (contacting 3'rd party services, reading from secure sources, etc…).
    Interface is similar to transact. Supports private transactions.
- Refactor transact endpoint: Use common logic for handling response format. with delegated transact
- Refactor logic of choosing ednorsers in transact endpoint. Previously both `endorsingPeers`
    and `endorsingParties` were selecting organizations in sligly different way under different
    circumstances. Now `endorsingPeers` selectes peers and `endorsingOrgs` selects orgs for all
    cases (query, send, privatesend) in both transact and transact with delegated sign.
    This is more consistent and predictable.
- Add new socketio endpoint `SubscribeDelegatedSign` for monitoring new blocks with delegated sign.
- Use common error handling in getblock, transact and transact delgated endpoints.
- Add functional tests for delegated signing feature.

Depends on: #2598

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-29 10:46:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2643" class=".btn">#2643</a>
            </td>
            <td>
                <b>
                    test(ghcr-rust-compiler): fix image build - anstream v0.5.0 cannot be built
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Upgraded the rust version of the image to v1.72.0 - short term fix
2. The longer term fix is that I locked down the version of wasm-pack to
the current latest stable (v0.12.1) so that the auto-upgrade
doesn't bite is again like this where the newer wasm-pack
starts demanding a newer rust compiler which we don't
have because we are pinning to a specific version through
the image tag that's being used.

Fixes #2641

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-28 22:09:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2642" class=".btn">#2642</a>
            </td>
            <td>
                <b>
                    feat(cbdc-bridging): add frontend code for the CBDC example
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * UI to interact with the CBDC example backend

This PR closes one action pointed out in PR #2185

Signed-off-by: André Augusto <andre.augusto@tecnico.ulisboa.pt>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-28 21:27:33 +0000 UTC
    </div>
</div>

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
Fixes https://github.com/hyperledger/cacti/issues/2299

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-23 22:50:29 +0000 UTC
    </div>
</div>

