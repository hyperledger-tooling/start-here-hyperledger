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
                PR <a href="https://github.com/hyperledger/cactus/pull/1568" class=".btn">#1568</a>
            </td>
            <td>
                <b>
                    ci(tools): fix iroha AIO image build flake on CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">dependencies</span><span class="chip">Developer_Experience</span><span class="chip">Iroha</span>
            </td>
            <td>
                Related to #1566 but does not actually fix it.
For now I just commented out the build step
of the flaky container image until we figure out
how to remedy the situation properly because
in the meantime I do not want to waste time
having to re-run the CI all the time because of the
flake.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 23:27:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1565" class=".btn">#1565</a>
            </td>
            <td>
                <b>
                    build(deps): bump @openzeppelin/contracts from 4.2.0 to 4.3.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">Security</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts](https://github.com/OpenZeppelin/openzeppelin-contracts)
from 4.2.0 to 4.3.3.

- [Release notes](https://github.com/OpenZeppelin/openzeppelin-contracts/releases)
- [Changelog](https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/CHANGELOG.md)
- [Commits](https://github.com/OpenZeppelin/openzeppelin-contracts/compare/v4.2.0...v4.3.3)

---
updated-dependencies:
- dependency-name: "@openzeppelin/contracts"
  dependency-type: direct:production
...

Signed-off-by: dependabot[bot] <support@github.com>
Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
(cherry picked from commit 8308434b862d9cc4a5d1b345cb09951438ee792d)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 19:20:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1564" class=".btn">#1564</a>
            </td>
            <td>
                <b>
                    fix(cmd-api-server): build occasionally broken - protoc-gen-ts #1563
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">API_Server</span><span class="chip">dependencies</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                Upgrading protoc-gen-ts from 0.4.0 to 0.6.0 instantly fixed the issue
while I had it in a reproduced state (e.g. my build was broken on main)

This is not necessarily evidence that the fix is legit, but it's most likely
a step in the right direction and there's also the possibility that this
is the actual fix. It would take too much time to properly debug if
it really is the fix, so I'll just give it the benefit of the doubt
for now and assume that it is.

Fixes #1563

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 18:25:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1562" class=".btn">#1562</a>
            </td>
            <td>
                <b>
                    fix(connector-corda): add script to remove files before generate them
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                generate-server script calls this new script before call
openapi-generator-cli

Closes: #1559

Signed-off-by: Elena Izaguirre <e.izaguirre.equiza@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 12:57:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1561" class=".btn">#1561</a>
            </td>
            <td>
                <b>
                    feat(connector-corda): enable Flow Database Access CorDapp
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">Corda</span>
            </td>
            <td>
                Added new corda-all-in-one image for flow-database-access sample

Modified Corda main-server image to allow calls to invoke without
executing any transaction.

Modified Corda InvokeContractV1Response to add the new flowId
field to return the flow handle id instead of use the callOutput
field, which now is used for the data returned by the flow. The
transactionId is not required because we can call invoke without
executing any transaction.

Resolves #1493

Signed-off-by: Elena Izaguirre <e.izaguirre.equiza@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 11:21:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1560" class=".btn">#1560</a>
            </td>
            <td>
                <b>
                    feat(docs): upated maintainers list
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span><span class="chip">P1</span>
            </td>
            <td>
                Added Jagpreet Singh Sasan to the list of active maintainers

Signed-off-by: jagpreetsinghsasan <jagpreet.singh.sasan@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 10:45:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1558" class=".btn">#1558</a>
            </td>
            <td>
                <b>
                    build(deps): bump @openzeppelin/contracts-upgradeable from 4.2.0 to 4.3.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts-upgradeable](https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable) from 4.2.0 to 4.3.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/releases"><code>@​openzeppelin/contracts-upgradeable</code>'s releases</a>.</em></p>
<blockquote>
<h2>v4.3.2</h2>
<p>:warning: This is a security patch. For more information visit the <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/security/advisories/GHSA-q4h9-46xg-m3x9">security advisory</a>.</p>
<ul>
<li><code>UUPSUpgradeable</code>: Add modifiers to prevent <code>upgradeTo</code> and <code>upgradeToAndCall</code> being executed on any contract that is not the active ERC1967 proxy. This prevents these functions being called on implementation contracts or minimal ERC1167 clones, in particular.</li>
</ul>
<h2>v4.3.1</h2>
<p>:warning: This is a security patch. For more information visit the <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/security/advisories/GHSA-vrw4-w73r-6mm8">security advisory</a>.</p>
<ul>
<li><code>TimelockController</code>: Add additional isOperationReady check.</li>
</ul>
<h2>v4.3.0</h2>
<p><strong>Visit our blog for the full <a href="https://blog.openzeppelin.com/openzeppelin-contracts-4-3/">4.3 announcement</a> as well as <a href="https://blog.openzeppelin.com/governor-smart-contract//">Governor announcement</a>!</strong></p>
<ul>
<li><code>ERC2771Context</code>: use private variable from storage to store the forwarder address. Fixes issues where <code>_msgSender()</code> was not callable from constructors. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2754">#2754</a>)</li>
<li><code>EnumerableSet</code>: add <code>values()</code> functions that returns an array containing all values in a single call. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2768">#2768</a>)</li>
<li><code>Governor</code>: added a modular system of <code>Governor</code> contracts based on <code>GovernorAlpha</code> and <code>GovernorBravo</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2672">#2672</a>)</li>
<li>Add an <code>interfaces</code> folder containing solidity interfaces to final ERCs. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2517">#2517</a>)</li>
<li><code>ECDSA</code>: add <code>tryRecover</code> functions that will not throw if the signature is invalid, and will return an error flag instead. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2661">#2661</a>)</li>
<li><code>SignatureChecker</code>: Reduce gas usage of the <code>isValidSignatureNow</code> function for the &quot;signature by EOA&quot; case. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2661">#2661</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/blob/master/CHANGELOG.md"><code>@​openzeppelin/contracts-upgradeable</code>'s changelog</a>.</em></p>
<blockquote>
<h2>4.3.3</h2>
<ul>
<li><code>ERC1155Supply</code>: Handle <code>totalSupply</code> changes by hooking into <code>_beforeTokenTransfer</code> to ensure consistency of balances and supply during <code>IERC1155Receiver.onERC1155Received</code> calls.</li>
</ul>
<h2>4.3.2 (2021-09-14)</h2>
<ul>
<li><code>UUPSUpgradeable</code>: Add modifiers to prevent <code>upgradeTo</code> and <code>upgradeToAndCall</code> being executed on any contract that is not the active ERC1967 proxy. This prevents these functions being called on implementation contracts or minimal ERC1167 clones, in particular.</li>
</ul>
<h2>4.3.1 (2021-08-26)</h2>
<ul>
<li><code>TimelockController</code>: Add additional isOperationReady check.</li>
</ul>
<h2>4.3.0 (2021-08-17)</h2>
<ul>
<li><code>ERC2771Context</code>: use private variable from storage to store the forwarder address. Fixes issues where <code>_msgSender()</code> was not callable from constructors. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2754">#2754</a>)</li>
<li><code>EnumerableSet</code>: add <code>values()</code> functions that returns an array containing all values in a single call. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2768">#2768</a>)</li>
<li><code>Governor</code>: added a modular system of <code>Governor</code> contracts based on <code>GovernorAlpha</code> and <code>GovernorBravo</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2672">#2672</a>)</li>
<li>Add an <code>interfaces</code> folder containing solidity interfaces to final ERCs. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2517">#2517</a>)</li>
<li><code>ECDSA</code>: add <code>tryRecover</code> functions that will not throw if the signature is invalid, and will return an error flag instead. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2661">#2661</a>)</li>
<li><code>SignatureChecker</code>: Reduce gas usage of the <code>isValidSignatureNow</code> function for the &quot;signature by EOA&quot; case. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2661">#2661</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/ebf264cc4b812e6557ed7d539e947211acd5670c"><code>ebf264c</code></a> Transpile 5548ce00</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/5c21639dc39b9062310ee3ca30aa2c3a4feccd8f"><code>5c21639</code></a> Transpile 85c278ba</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/0168fdef32db54b418b411afad0dad69b6a11023"><code>0168fde</code></a> Transpile 14df696b</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/5630276cea48dbabac1d890ad637ab2aef339a61"><code>5630276</code></a> Transpile b99f49d3</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/618d129b52c14aea8d37a413e4c8b643439abe73"><code>618d129</code></a> Transpile 482dc4ec</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/227970d3fc78269c12d96464f4e82a31b6826b0e"><code>227970d</code></a> Transpile 1bfeb6b2</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/0cec7b5355a3c39d9d307b8b1c6d3f849f125501"><code>0cec7b5</code></a> Transpile 0577a612</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/23eeb136ae8fb12c78479217a6089b6d1dfe2c08"><code>23eeb13</code></a> Transpile 391ecdc2</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/583ca63a5b267cb33969793f1163bb1bb9fe1eca"><code>583ca63</code></a> Transpile 01a3ef98</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/8deeede090344f970854f6910b776709ffe1add1"><code>8deeede</code></a> Transpile 79d9fcfa</li>
<li>See full diff in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/compare/v4.2.0...v4.3.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@openzeppelin/contracts-upgradeable&package-manager=npm_and_yarn&previous-version=4.2.0&new-version=4.3.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-11-23 04:31:36 +0000 UTC
    </div>
</div>

