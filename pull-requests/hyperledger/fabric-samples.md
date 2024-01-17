---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1173" class=".btn">#1173</a>
            </td>
            <td>
                <b>
                    	new file:   LandContract/application-typescript/package.json
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                	new file:   LandContract/application-typescript/src/Admin.js
	new file:   LandContract/application-typescript/src/app.ts
	new file:   LandContract/application-typescript/src/registerEnrollUser.js
	new file:   LandContract/application-typescript/src/utils/AppUtil.ts
	new file:   LandContract/application-typescript/src/utils/CAUtil.ts
	new file:   LandContract/application-typescript/tsconfig.json
	new file:   LandContract/application-typescript/tslint.json
	new file:   chaincode-typescript/Dockerfile
	new file:   chaincode-typescript/dist/Contract/landAsset.d.ts
	new file:   chaincode-typescript/dist/Contract/landAsset.js
	new file:   chaincode-typescript/dist/Contract/landAsset.js.map
	new file:   chaincode-typescript/dist/Contract/landTransaction.d.ts
	new file:   chaincode-typescript/dist/Contract/landTransaction.js
	new file:   chaincode-typescript/dist/Contract/landTransaction.js.map
	new file:   chaincode-typescript/dist/asset.d.ts
	new file:   chaincode-typescript/dist/asset.js
	new file:   chaincode-typescript/dist/asset.js.map
	new file:   chaincode-typescript/dist/assetTransfer.d.ts
	new file:   chaincode-typescript/dist/assetTransfer.js
	new file:   chaincode-typescript/dist/assetTransfer.js.map
	new file:   chaincode-typescript/dist/index.d.ts
	new file:   chaincode-typescript/dist/index.js
	new file:   chaincode-typescript/dist/index.js.map
	new file:   chaincode-typescript/docker/docker-entrypoint.sh
	new file:   chaincode-typescript/npm-shrinkwrap.json
	new file:   chaincode-typescript/package.json
	new file:   chaincode-typescript/src/Contract/Admin.js
	new file:   chaincode-typescript/src/Contract/landAsset.ts
	new file:   chaincode-typescript/src/Contract/landTransaction.ts
	new file:   chaincode-typescript/src/Contract/registerEnrollUser.js
	new file:   chaincode-typescript/src/Contract/userRequest.ts
	new file:   chaincode-typescript/src/Contract/wallet/admin.id
	new file:   chaincode-typescript/src/Contract/wallet/user123.id
	new file:   chaincode-typescript/src/asset.ts
	new file:   chaincode-typescript/src/assetTransfer.ts
	new file:   chaincode-typescript/src/index.ts
	new file:   chaincode-typescript/tsconfig.json
	new file:   chaincode-typescript/tslint.json
	modified:   test-network/compose/compose-ca.yaml
	modified:   test-network/compose/compose-test-net.yaml
	modified:   test-network/compose/docker/docker-compose-bft-test-net.yaml
	modified:   test-network/compose/docker/docker-compose-test-net.yaml
	modified:   test-network/configtx/configtx.yaml
	modified:   test-network/network.sh
	modified:   test-network/organizations/ccp-generate.sh
	modified:   test-network/organizations/cryptogen/crypto-config-org2.yaml
	new file:   test-network/organizations/cryptogen/crypto-config-org3.yaml
	new file:   test-network/organizations/cryptogen/crypto-config-org4.yaml
	modified:   test-network/organizations/fabric-ca/registerEnroll.sh
	new file:   test-network_org4.zip
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-17 11:31:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1169" class=".btn">#1169</a>
            </td>
            <td>
                <b>
                    Fix certPath in assetTransfer.go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Following the latest tutorial, the current version of network.sh does not generate `cert.pem` as filename under `msp/signcerts` but instead created `User1@org1.example.com-cert.pem`. I have edited the application file to reflect such difference.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-15 01:32:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1167" class=".btn">#1167</a>
            </td>
            <td>
                <b>
                    Bump follow-redirects from 1.15.2 to 1.15.4 in /asset-transfer-basic/rest-api-typescript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [follow-redirects](https://github.com/follow-redirects/follow-redirects) from 1.15.2 to 1.15.4.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/65858205e59f1e23c9bf173348a7a7cbb8ac47f5"><code>6585820</code></a> Release version 1.15.4 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/7a6567e16dfa9ad18a70bfe91784c28653fbf19d"><code>7a6567e</code></a> Disallow bracketed hostnames.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/05629af696588b90d64e738bc2e809a97a5f92fc"><code>05629af</code></a> Prefer native URL instead of deprecated url.parse.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/1cba8e85fa73f563a439fe460cf028688e4358df"><code>1cba8e8</code></a> Prefer native URL instead of legacy url.resolve.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/72bc2a4229bc18dc9fbd57c60579713e6264cb92"><code>72bc2a4</code></a> Simplify _processResponse error handling.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/3d42aecdca39b144a0a2f27ea134b4cf67dd796a"><code>3d42aec</code></a> Add bracket tests.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/bcbb096b32686ecad6cd34235358ed6f2217d4f0"><code>bcbb096</code></a> Do not directly set Error properties.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/192dbe7ce671ecad813c074bffe3b3f5d3680fee"><code>192dbe7</code></a> Release version 1.15.3 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/bd8c81e4f32d12f28a35d265f88b1716703687c6"><code>bd8c81e</code></a> Fix resource leak on destroy.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/9c728c314b06f9595dcd7f245d40731e8a27d79f"><code>9c728c3</code></a> Split linting and testing.</li>
<li>Additional commits viewable in <a href="https://github.com/follow-redirects/follow-redirects/compare/v1.15.2...v1.15.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=follow-redirects&package-manager=npm_and_yarn&previous-version=1.15.2&new-version=1.15.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-11 00:23:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1166" class=".btn">#1166</a>
            </td>
            <td>
                <b>
                    Bump github.com/quic-go/quic-go from 0.38.1 to 0.38.2 in /token-sdk/auditor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/quic-go/quic-go](https://github.com/quic-go/quic-go) from 0.38.1 to 0.38.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/quic-go/quic-go/releases">github.com/quic-go/quic-go's releases</a>.</em></p>
<blockquote>
<h2>v0.38.2</h2>
<p>This release contains fixes for a resource exhaustion attack on QUIC's path validation logic (CVE-2023-49295), see <a href="https://seemann.io/posts/2023-12-18-exploiting-quics-path-validation">https://seemann.io/posts/2023-12-18-exploiting-quics-path-validation</a> for details:</p>
<ul>
<li>limit the number of queued PATH_RESPONSE frames to 256 (<a href="https://redirect.github.com/quic-go/quic-go/pull/4199">quic-go/quic-go#4199</a>)</li>
<li>don't retransmit PATH_CHALLENGE and PATH_RESPONSE frames (<a href="https://redirect.github.com/quic-go/quic-go/pull/4200">quic-go/quic-go#4200</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/quic-go/quic-go/compare/v0.38.1...v0.38.2">https://github.com/quic-go/quic-go/compare/v0.38.1...v0.38.2</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/quic-go/quic-go/commit/9aaefe19fc3dc8c8917cc87e6128bb56d9e9e6cc"><code>9aaefe1</code></a> don't retransmit PATH_CHALLENGE and PATH_RESPONSE frames (<a href="https://redirect.github.com/quic-go/quic-go/issues/4200">#4200</a>)</li>
<li><a href="https://github.com/quic-go/quic-go/commit/17fc98c2d81dbe685c19702dc694a9d606ac56dc"><code>17fc98c</code></a> limit the number of queued PATH_RESPONSE frames to 256 (<a href="https://redirect.github.com/quic-go/quic-go/issues/4199">#4199</a>)</li>
<li>See full diff in <a href="https://github.com/quic-go/quic-go/compare/v0.38.1...v0.38.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/quic-go/quic-go&package-manager=go_modules&previous-version=0.38.1&new-version=0.38.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-10 15:11:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1165" class=".btn">#1165</a>
            </td>
            <td>
                <b>
                    Bump github.com/quic-go/quic-go from 0.38.1 to 0.38.2 in /token-sdk/issuer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/quic-go/quic-go](https://github.com/quic-go/quic-go) from 0.38.1 to 0.38.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/quic-go/quic-go/releases">github.com/quic-go/quic-go's releases</a>.</em></p>
<blockquote>
<h2>v0.38.2</h2>
<p>This release contains fixes for a resource exhaustion attack on QUIC's path validation logic (CVE-2023-49295), see <a href="https://seemann.io/posts/2023-12-18-exploiting-quics-path-validation">https://seemann.io/posts/2023-12-18-exploiting-quics-path-validation</a> for details:</p>
<ul>
<li>limit the number of queued PATH_RESPONSE frames to 256 (<a href="https://redirect.github.com/quic-go/quic-go/pull/4199">quic-go/quic-go#4199</a>)</li>
<li>don't retransmit PATH_CHALLENGE and PATH_RESPONSE frames (<a href="https://redirect.github.com/quic-go/quic-go/pull/4200">quic-go/quic-go#4200</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/quic-go/quic-go/compare/v0.38.1...v0.38.2">https://github.com/quic-go/quic-go/compare/v0.38.1...v0.38.2</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/quic-go/quic-go/commit/9aaefe19fc3dc8c8917cc87e6128bb56d9e9e6cc"><code>9aaefe1</code></a> don't retransmit PATH_CHALLENGE and PATH_RESPONSE frames (<a href="https://redirect.github.com/quic-go/quic-go/issues/4200">#4200</a>)</li>
<li><a href="https://github.com/quic-go/quic-go/commit/17fc98c2d81dbe685c19702dc694a9d606ac56dc"><code>17fc98c</code></a> limit the number of queued PATH_RESPONSE frames to 256 (<a href="https://redirect.github.com/quic-go/quic-go/issues/4199">#4199</a>)</li>
<li>See full diff in <a href="https://github.com/quic-go/quic-go/compare/v0.38.1...v0.38.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/quic-go/quic-go&package-manager=go_modules&previous-version=0.38.1&new-version=0.38.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-10 15:11:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1164" class=".btn">#1164</a>
            </td>
            <td>
                <b>
                    Bump github.com/quic-go/quic-go from 0.38.1 to 0.38.2 in /token-sdk/owner
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/quic-go/quic-go](https://github.com/quic-go/quic-go) from 0.38.1 to 0.38.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/quic-go/quic-go/releases">github.com/quic-go/quic-go's releases</a>.</em></p>
<blockquote>
<h2>v0.38.2</h2>
<p>This release contains fixes for a resource exhaustion attack on QUIC's path validation logic (CVE-2023-49295), see <a href="https://seemann.io/posts/2023-12-18-exploiting-quics-path-validation">https://seemann.io/posts/2023-12-18-exploiting-quics-path-validation</a> for details:</p>
<ul>
<li>limit the number of queued PATH_RESPONSE frames to 256 (<a href="https://redirect.github.com/quic-go/quic-go/pull/4199">quic-go/quic-go#4199</a>)</li>
<li>don't retransmit PATH_CHALLENGE and PATH_RESPONSE frames (<a href="https://redirect.github.com/quic-go/quic-go/pull/4200">quic-go/quic-go#4200</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/quic-go/quic-go/compare/v0.38.1...v0.38.2">https://github.com/quic-go/quic-go/compare/v0.38.1...v0.38.2</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/quic-go/quic-go/commit/9aaefe19fc3dc8c8917cc87e6128bb56d9e9e6cc"><code>9aaefe1</code></a> don't retransmit PATH_CHALLENGE and PATH_RESPONSE frames (<a href="https://redirect.github.com/quic-go/quic-go/issues/4200">#4200</a>)</li>
<li><a href="https://github.com/quic-go/quic-go/commit/17fc98c2d81dbe685c19702dc694a9d606ac56dc"><code>17fc98c</code></a> limit the number of queued PATH_RESPONSE frames to 256 (<a href="https://redirect.github.com/quic-go/quic-go/issues/4199">#4199</a>)</li>
<li>See full diff in <a href="https://github.com/quic-go/quic-go/compare/v0.38.1...v0.38.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/quic-go/quic-go&package-manager=go_modules&previous-version=0.38.1&new-version=0.38.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-10 15:10:56 +0000 UTC
    </div>
</div>

