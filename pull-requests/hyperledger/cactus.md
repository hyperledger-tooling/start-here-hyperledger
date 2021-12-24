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
                PR <a href="https://github.com/hyperledger/cactus/pull/1677" class=".btn">#1677</a>
            </td>
            <td>
                <b>
                    refactor: upgrade the version of node in CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is `PR 0` that is the prerequisite for an upcoming PR that will fix issue #1654. 

What this PR does is upgrade the version in the CI from Node `v14.18.0` to Node `v16.0.0`. 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-23 20:19:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1676" class=".btn">#1676</a>
            </td>
            <td>
                <b>
                    fix: add optional parameter token to CactusNode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                add token to apiClient.ofLedger and PluginConsortiumManual
getConsortiumJws method when property is setted

relationed with #1579

Signed-off-by: Elena Izaguirre <e.izaguirre.equiza@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-22 16:17:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1673" class=".btn">#1673</a>
            </td>
            <td>
                <b>
                    test: jestify runtime-plugin-imports test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Migrated test from Tap to Jest.

File Path:
packages/cactus-test-cmd-api-server/src/test/
typescript/integration/runtime-plugin-imports.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: awadhana <awadhana0825@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-21 21:19:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1672" class=".btn">#1672</a>
            </td>
            <td>
                <b>
                    test: jestify plugin-import-with-npm-install test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Migrated test from Tap to Jest.

File Path:
packages/cactus-test-cmd-api-server/src/test/typescript/
integration/plugin-import-with-npm-install.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: awadhana <awadhana0825@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-21 20:50:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1670" class=".btn">#1670</a>
            </td>
            <td>
                <b>
                    build: include cmd-socketio-server and socketio validators in the monorepo setup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span>
            </td>
            <td>
                Multiple changes, but they are tightly related to same issue so I introduced them in single PR, hope it's okay :)

- Added two build steps in common packages.json to facilitate more complex build process of packages related to this PR. I will write another comment in code to this.
- Added standalone projects to the global monorepo setup, namely:
```
./packages/cactus-cmd-socketio-server
./packages/cactus-plugin-ledger-connector-fabric-socketio
./packages/cactus-plugin-ledger-connector-go-ethereum-socketio
./packages/cactus-plugin-ledger-connector-sawtooth-socketio
```
- All changed packages extends `tsconfig.base.json`, but most overwrites strict flag to false. This is the task for another PR. After fixing strict warnings we can merge verifier tests to the main jest config.
    - Related issue - https://github.com/hyperledger/cactus/issues/1671
- All projects builds in typescript 4 set by the root config.
- Updated the README files form connectors and examples to describe new (monorepo) build process. Also converted tabs to spaces.
- I've lost a while trying to debug socketio errors when I forgot to run the init step in example app (I was sure it was my changes that caused that). I don't see for now any benefit of running two separate commands, so I've merged the init-* step to the build process itself so it's always executed.
- Rewritten socketio and go-eheterum dockerfiles. Not strictly necessary for this PR, but now they are much smaller both in dockerfile lines and resulting container size. Tested with electricty-trade - works the same as before.
- **yarn.lock update** - Changes from previous commits (I think it wasn't regenerated for a while) and from removing redundant and duplicated packages in this issue.
- Fixed bug in Verifier that caused cartrade to fail compilation - for now just restored the previous implementation. Will be part of fixes to enable strict flag in this package (another task).
- Examples were not included in monorepo setup, since it'd be tricky at the moment. It's better to containerize them instead of doing some fixes now.
- Projects use `../../.build-cache` like the other ones, so manual `npm run build` in package dir can do nothing. Do builds from root dir or clear the cache.

Closes: #1647
Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-21 15:38:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1669" class=".btn">#1669</a>
            </td>
            <td>
                <b>
                    test: jestify config-service-example-config-validity test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Tests</span><span class="chip">Jestify</span>
            </td>
            <td>
                Migrated test from Tap to Jest.

File Path:
packages/cactus-cmd-api-server/src/test/typescript/
unit/config/config-service-example-config-validity.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: awadhana <awadhana0825@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-19 18:44:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1668" class=".btn">#1668</a>
            </td>
            <td>
                <b>
                    test: jestify v2.3.0-invoke contract test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Tests</span><span class="chip">Jestify</span>
            </td>
            <td>
                Migrated test from Tap to Jest.

File Path:
packages/cactus-plugin-ledger-connector-quorum/src/test/
typescript/integration/plugin-ledger-connector-quorum/
deploy-contract/v2.3.0-invoke-contract.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: awadhana <awadhana0825@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-19 17:29:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1666" class=".btn">#1666</a>
            </td>
            <td>
                <b>
                    test: jestify get-balance test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Migrated test from Tap to Jest.

File Path:
packages/cactus-plugin-ledger-connector-besu/src/test/
typescript/integration/plugin-ledger-connector-besu/
deploy-contract/get-balance.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: awadhana <awadhana0825@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-17 13:04:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1665" class=".btn">#1665</a>
            </td>
            <td>
                <b>
                    build(deps): bump @openzeppelin/contracts-upgradeable from 4.3.3 to 4.4.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">Security</span><span class="chip">P2</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts-upgradeable](https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable) from 4.3.3 to 4.4.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/releases"><code>@​openzeppelin/contracts-upgradeable</code>'s releases</a>.</em></p>
<blockquote>
<h2>v4.4.1</h2>
<p>:warning: This is a patch for a low severity vulnerability. For more information <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-9c22-pwxw-p6hx">visit the security advisory</a>.</p>
<ul>
<li><code>Initializable</code>: change the existing <code>initializer</code> modifier and add a new <code>onlyInitializing</code> modifier to prevent reentrancy risk. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3006">#3006</a>)</li>
</ul>
<h3>Breaking change</h3>
<p>It is no longer possible to call an <code>initializer</code>-protected function from within another <code>initializer</code> function outside the context of a constructor. Projects using OpenZeppelin upgradeable proxies should continue to work as is, since in the common case the initializer is invoked in the constructor directly. If this is not the case for you, the suggested change is to use the new <code>onlyInitializing</code> modifier in the following way:</p>
<pre lang="diff"><code> contract A {
-    function initialize() public   initializer { ... }
+    function initialize() internal onlyInitializing { ... }
 }
 contract B is A {
     function initialize() public initializer {
         A.initialize();
     }
 }
</code></pre>
<h2>v4.4.0</h2>
<p>Check out the first <a href="https://www.youtube.com/watch?v=ed96DWbfliQ"><strong>OpenZeppelin Community Call</strong></a> where the team discussed everything that is included in this release.</p>
<p>And if you missed it, we recently announced an official <strong>bug bounty program</strong> for OpenZeppelin Contracts. <a href="https://forum.openzeppelin.com/t/openzeppelin-contracts-bug-bounty-program-on-immunefi/19279">Check it out!</a></p>
<ul>
<li><code>Ownable</code>: add an internal <code>_transferOwnership(address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2568">#2568</a>)</li>
<li><code>AccessControl</code>: add internal <code>_grantRole(bytes32,address)</code> and <code>_revokeRole(bytes32,address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2568">#2568</a>)</li>
<li><code>AccessControl</code>: mark <code>_setupRole(bytes32,address)</code> as deprecated in favor of <code>_grantRole(bytes32,address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2568">#2568</a>)</li>
<li><code>AccessControlEnumerable</code>: hook into <code>_grantRole(bytes32,address)</code> and <code>_revokeRole(bytes32,address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2946">#2946</a>)</li>
<li><code>EIP712</code>: cache <code>address(this)</code> to immutable storage to avoid potential issues if a vanilla contract is used in a delegatecall context. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2852">#2852</a>)</li>
<li>Add internal <code>_setApprovalForAll</code> to <code>ERC721</code> and <code>ERC1155</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2834">#2834</a>)</li>
<li><code>Governor</code>: shift vote start and end by one block to better match Compound's GovernorBravo and prevent voting at the Governor level if the voting snapshot is not ready. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2892">#2892</a>)</li>
<li><code>GovernorCompatibilityBravo</code>: consider quorum an inclusive rather than exclusive minimum to match Compound's GovernorBravo. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2974">#2974</a>)</li>
<li><code>GovernorSettings</code>: a new governor module that manages voting settings updatable through governance actions. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2904">#2904</a>)</li>
<li><code>PaymentSplitter</code>: now supports ERC20 assets in addition to Ether. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2858">#2858</a>)</li>
<li><code>ECDSA</code>: add a variant of <code>toEthSignedMessageHash</code> for arbitrary length message hashing. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2865">#2865</a>)</li>
<li><code>MerkleProof</code>: add a <code>processProof</code> function that returns the rebuilt root hash given a leaf and a proof. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2841">#2841</a>)</li>
<li><code>VestingWallet</code>: new contract that handles the vesting of Ether and ERC20 tokens following a customizable vesting schedule. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2748">#2748</a>)</li>
<li><code>Governor</code>: enable receiving Ether when a Timelock contract is not used. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2849">#2748</a>)</li>
<li><code>GovernorTimelockCompound</code>: fix ability to use Ether stored in the Timelock contract. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2849">#2748</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/blob/master/CHANGELOG.md"><code>@​openzeppelin/contracts-upgradeable</code>'s changelog</a>.</em></p>
<blockquote>
<h2>4.4.1 (2021-12-10)</h2>
<ul>
<li><code>Initializable</code>: change the existing <code>initializer</code> modifier and add a new <code>onlyInitializing</code> modifier to prevent reentrancy risk. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3006">#3006</a>)</li>
</ul>
<h3>Breaking change</h3>
<p>It is no longer possible to call an <code>initializer</code>-protected function from within another <code>initializer</code> function outside the context of a constructor. Projects using OpenZeppelin upgradeable proxies should continue to work as is, since in the common case the initializer is invoked in the constructor directly. If this is not the case for you, the suggested change is to use the new <code>onlyInitializing</code> modifier in the following way:</p>
<pre lang="diff"><code> contract A {
-    function initialize() public   initializer { ... }
+    function initialize() internal onlyInitializing { ... }
 }
 contract B is A {
     function initialize() public initializer {
         A.initialize();
     }
 }
</code></pre>
<h2>4.4.0 (2021-11-25)</h2>
<ul>
<li><code>Ownable</code>: add an internal <code>_transferOwnership(address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2568">#2568</a>)</li>
<li><code>AccessControl</code>: add internal <code>_grantRole(bytes32,address)</code> and <code>_revokeRole(bytes32,address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2568">#2568</a>)</li>
<li><code>AccessControl</code>: mark <code>_setupRole(bytes32,address)</code> as deprecated in favor of <code>_grantRole(bytes32,address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2568">#2568</a>)</li>
<li><code>AccessControlEnumerable</code>: hook into <code>_grantRole(bytes32,address)</code> and <code>_revokeRole(bytes32,address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2946">#2946</a>)</li>
<li><code>EIP712</code>: cache <code>address(this)</code> to immutable storage to avoid potential issues if a vanilla contract is used in a delegatecall context. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2852">#2852</a>)</li>
<li>Add internal <code>_setApprovalForAll</code> to <code>ERC721</code> and <code>ERC1155</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2834">#2834</a>)</li>
<li><code>Governor</code>: shift vote start and end by one block to better match Compound's GovernorBravo and prevent voting at the Governor level if the voting snapshot is not ready. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2892">#2892</a>)</li>
<li><code>GovernorCompatibilityBravo</code>: consider quorum an inclusive rather than exclusive minimum to match Compound's GovernorBravo. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2974">#2974</a>)</li>
<li><code>GovernorSettings</code>: a new governor module that manages voting settings updatable through governance actions. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2904">#2904</a>)</li>
<li><code>PaymentSplitter</code>: now supports ERC20 assets in addition to Ether. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2858">#2858</a>)</li>
<li><code>ECDSA</code>: add a variant of <code>toEthSignedMessageHash</code> for arbitrary length message hashing. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2865">#2865</a>)</li>
<li><code>MerkleProof</code>: add a <code>processProof</code> function that returns the rebuilt root hash given a leaf and a proof. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2841">#2841</a>)</li>
<li><code>VestingWallet</code>: new contract that handles the vesting of Ether and ERC20 tokens following a customizable vesting schedule. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2748">#2748</a>)</li>
<li><code>Governor</code>: enable receiving Ether when a Timelock contract is not used. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2849">#2748</a>)</li>
<li><code>GovernorTimelockCompound</code>: fix ability to use Ether stored in the Timelock contract. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2849">#2748</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/3ff38d850a4e8bcd377f559f750678734af50450"><code>3ff38d8</code></a> Transpile 5fcb6c72</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/44c52af9ab856ea4f89f2e5a533cc3cdebd2d75b"><code>44c52af</code></a> Transpile 5fcb6c72</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/6e8820d5a421120c11fd125b145d00cf126a38df"><code>6e8820d</code></a> Transpile d6894842</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/835a58a8c2928a0a8e8381684c46289f3822afca"><code>835a58a</code></a> Transpile 2d95a812</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/18f6cb0f50e7fb0107845002f73389b030467080"><code>18f6cb0</code></a> Transpile 8b043070</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/e732caa6950c0ed880992a1c064a165f3f53da12"><code>e732caa</code></a> Transpile 93269dee</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/39a2c938900d2ae242654fac69d3867fc2eb53c4"><code>39a2c93</code></a> Transpile 5b5e3823</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/b9bc5391dacc2c6082b64abe79c06bf624cc7c6d"><code>b9bc539</code></a> Transpile 34c715d8</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/9839feb54203df1f0bf28a1956149515d929bb8a"><code>9839feb</code></a> Transpile 33343101</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/ae47cd6384c7bb88a5e6afce388e3214fd32840d"><code>ae47cd6</code></a> Transpile 27d1de7a</li>
<li>Additional commits viewable in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/compare/v4.3.3...v4.4.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@openzeppelin/contracts-upgradeable&package-manager=npm_and_yarn&previous-version=4.3.3&new-version=4.4.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cactus/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-17 02:34:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1664" class=".btn">#1664</a>
            </td>
            <td>
                <b>
                    build(deps): bump @openzeppelin/contracts from 4.3.3 to 4.4.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts](https://github.com/OpenZeppelin/openzeppelin-contracts) from 4.3.3 to 4.4.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/releases"><code>@​openzeppelin/contracts</code>'s releases</a>.</em></p>
<blockquote>
<h2>v4.4.1</h2>
<p>:warning: This is a patch for a low severity vulnerability. For more information <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-9c22-pwxw-p6hx">visit the security advisory</a>.</p>
<ul>
<li><code>Initializable</code>: change the existing <code>initializer</code> modifier and add a new <code>onlyInitializing</code> modifier to prevent reentrancy risk. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3006">#3006</a>)</li>
</ul>
<h3>Breaking change</h3>
<p>It is no longer possible to call an <code>initializer</code>-protected function from within another <code>initializer</code> function outside the context of a constructor. Projects using OpenZeppelin upgradeable proxies should continue to work as is, since in the common case the initializer is invoked in the constructor directly. If this is not the case for you, the suggested change is to use the new <code>onlyInitializing</code> modifier in the following way:</p>
<pre lang="diff"><code> contract A {
-    function initialize() public   initializer { ... }
+    function initialize() internal onlyInitializing { ... }
 }
 contract B is A {
     function initialize() public initializer {
         A.initialize();
     }
 }
</code></pre>
<h2>v4.4.0</h2>
<p>Check out the first <a href="https://www.youtube.com/watch?v=ed96DWbfliQ"><strong>OpenZeppelin Community Call</strong></a> where the team discussed everything that is included in this release.</p>
<p>And if you missed it, we recently announced an official <strong>bug bounty program</strong> for OpenZeppelin Contracts. <a href="https://forum.openzeppelin.com/t/openzeppelin-contracts-bug-bounty-program-on-immunefi/19279">Check it out!</a></p>
<ul>
<li><code>Ownable</code>: add an internal <code>_transferOwnership(address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2568">#2568</a>)</li>
<li><code>AccessControl</code>: add internal <code>_grantRole(bytes32,address)</code> and <code>_revokeRole(bytes32,address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2568">#2568</a>)</li>
<li><code>AccessControl</code>: mark <code>_setupRole(bytes32,address)</code> as deprecated in favor of <code>_grantRole(bytes32,address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2568">#2568</a>)</li>
<li><code>AccessControlEnumerable</code>: hook into <code>_grantRole(bytes32,address)</code> and <code>_revokeRole(bytes32,address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2946">#2946</a>)</li>
<li><code>EIP712</code>: cache <code>address(this)</code> to immutable storage to avoid potential issues if a vanilla contract is used in a delegatecall context. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2852">#2852</a>)</li>
<li>Add internal <code>_setApprovalForAll</code> to <code>ERC721</code> and <code>ERC1155</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2834">#2834</a>)</li>
<li><code>Governor</code>: shift vote start and end by one block to better match Compound's GovernorBravo and prevent voting at the Governor level if the voting snapshot is not ready. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2892">#2892</a>)</li>
<li><code>GovernorCompatibilityBravo</code>: consider quorum an inclusive rather than exclusive minimum to match Compound's GovernorBravo. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2974">#2974</a>)</li>
<li><code>GovernorSettings</code>: a new governor module that manages voting settings updatable through governance actions. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2904">#2904</a>)</li>
<li><code>PaymentSplitter</code>: now supports ERC20 assets in addition to Ether. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2858">#2858</a>)</li>
<li><code>ECDSA</code>: add a variant of <code>toEthSignedMessageHash</code> for arbitrary length message hashing. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2865">#2865</a>)</li>
<li><code>MerkleProof</code>: add a <code>processProof</code> function that returns the rebuilt root hash given a leaf and a proof. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2841">#2841</a>)</li>
<li><code>VestingWallet</code>: new contract that handles the vesting of Ether and ERC20 tokens following a customizable vesting schedule. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2748">#2748</a>)</li>
<li><code>Governor</code>: enable receiving Ether when a Timelock contract is not used. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2849">#2748</a>)</li>
<li><code>GovernorTimelockCompound</code>: fix ability to use Ether stored in the Timelock contract. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2849">#2748</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/CHANGELOG.md"><code>@​openzeppelin/contracts</code>'s changelog</a>.</em></p>
<blockquote>
<h2>4.4.1 (2021-12-14)</h2>
<ul>
<li><code>Initializable</code>: change the existing <code>initializer</code> modifier and add a new <code>onlyInitializing</code> modifier to prevent reentrancy risk. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3006">#3006</a>)</li>
</ul>
<h3>Breaking change</h3>
<p>It is no longer possible to call an <code>initializer</code>-protected function from within another <code>initializer</code> function outside the context of a constructor. Projects using OpenZeppelin upgradeable proxies should continue to work as is, since in the common case the initializer is invoked in the constructor directly. If this is not the case for you, the suggested change is to use the new <code>onlyInitializing</code> modifier in the following way:</p>
<pre lang="diff"><code> contract A {
-    function initialize() public   initializer { ... }
+    function initialize() internal onlyInitializing { ... }
 }
 contract B is A {
     function initialize() public initializer {
         A.initialize();
     }
 }
</code></pre>
<h2>4.4.0 (2021-11-25)</h2>
<ul>
<li><code>Ownable</code>: add an internal <code>_transferOwnership(address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2568">#2568</a>)</li>
<li><code>AccessControl</code>: add internal <code>_grantRole(bytes32,address)</code> and <code>_revokeRole(bytes32,address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2568">#2568</a>)</li>
<li><code>AccessControl</code>: mark <code>_setupRole(bytes32,address)</code> as deprecated in favor of <code>_grantRole(bytes32,address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2568">#2568</a>)</li>
<li><code>AccessControlEnumerable</code>: hook into <code>_grantRole(bytes32,address)</code> and <code>_revokeRole(bytes32,address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2946">#2946</a>)</li>
<li><code>EIP712</code>: cache <code>address(this)</code> to immutable storage to avoid potential issues if a vanilla contract is used in a delegatecall context. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2852">#2852</a>)</li>
<li>Add internal <code>_setApprovalForAll</code> to <code>ERC721</code> and <code>ERC1155</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2834">#2834</a>)</li>
<li><code>Governor</code>: shift vote start and end by one block to better match Compound's GovernorBravo and prevent voting at the Governor level if the voting snapshot is not ready. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2892">#2892</a>)</li>
<li><code>GovernorCompatibilityBravo</code>: consider quorum an inclusive rather than exclusive minimum to match Compound's GovernorBravo. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2974">#2974</a>)</li>
<li><code>GovernorSettings</code>: a new governor module that manages voting settings updatable through governance actions. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2904">#2904</a>)</li>
<li><code>PaymentSplitter</code>: now supports ERC20 assets in addition to Ether. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2858">#2858</a>)</li>
<li><code>ECDSA</code>: add a variant of <code>toEthSignedMessageHash</code> for arbitrary length message hashing. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2865">#2865</a>)</li>
<li><code>MerkleProof</code>: add a <code>processProof</code> function that returns the rebuilt root hash given a leaf and a proof. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2841">#2841</a>)</li>
<li><code>VestingWallet</code>: new contract that handles the vesting of Ether and ERC20 tokens following a customizable vesting schedule. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2748">#2748</a>)</li>
<li><code>Governor</code>: enable receiving Ether when a Timelock contract is not used. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2849">#2748</a>)</li>
<li><code>GovernorTimelockCompound</code>: fix ability to use Ether stored in the Timelock contract. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2849">#2748</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/6bd6b76d1156e20e45d1016f355d154141c7e5b9"><code>6bd6b76</code></a> 4.4.1</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/13a6ec753a3e9c56a3d9dec845a9b5cbd616b658"><code>13a6ec7</code></a> Remove bad date from changelog</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/553c8fdec708ea10dd5f4a2977364af7a562566f"><code>553c8fd</code></a> Update initializer modifier to prevent reentrancy during initialization (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3006">#3006</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/4961a51cc736c7d4aa9bd2e11e4cbbaff73efee9"><code>4961a51</code></a> 4.4.0</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/94a0b8f573e0033d5338689030d2b721e4a5177a"><code>94a0b8f</code></a> Make VestingWallet token event argument indexed (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/2988">#2988</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/0413d58860e0253f30cd6d18c6caaf20ebb4de33"><code>0413d58</code></a> add bug bounty info</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/a4cee9ed37d5d406c1ae742d1cd4c3122f930ba5"><code>a4cee9e</code></a> make setters in GovernorSettings virtual</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/65ef662a2ba263b62de0f45b062c8942362ba8c8"><code>65ef662</code></a> 4.4.0-rc.1</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/8b8ee57a1a09656d7f10826c1dac7c8720d5b51c"><code>8b8ee57</code></a> Make quorum behavior match GovernorBravo (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/2974">#2974</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/cf6e32fc541b4436de7cec3e87aee684dff18bb5"><code>cf6e32f</code></a> Fix Timelock Controller description typo (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/2960">#2960</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/compare/v4.3.3...v4.4.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@openzeppelin/contracts&package-manager=npm_and_yarn&previous-version=4.3.3&new-version=4.4.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cactus/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-17 02:34:30 +0000 UTC
    </div>
</div>

