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
                PR <a href="https://github.com/hyperledger/cacti/pull/2581" class=".btn">#2581</a>
            </td>
            <td>
                <b>
                    feat(cactus-plugin-ledger-connector-ethereum): update web3js to 4.X
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                - Update web3js packages from 1.10 to 4.0.3 in `cactus-plugin-ledger-connector-ethereum` and
    `cactus-test-plugin-ledger-connector-ethereum`. This allows interacting
    with most recent geth nodes.
- Refactor all ethereum tests. Most of the test cases were duplicated multiple times
    (between different quorum ledger versions test and deployment methods). I've removed all this
    duplication while maintaining similar level of test coverage.
    New tests use Geth test ledger instead of Quorum one.
- Add web3js type conversions methods to minimize impact of poor dynamic typing
    in this early release of 4.X.
- Update API. In 4.X all numeric responses has been converted to BigNum.
    To keep up with this some fields has been changed to string instead of number when necessary.
    Add some missing fields as well.
- Add `estimateMaxFeePerGas` method for estimating current transaction cost.
- Fix invalid `runTransact` response type.
- Add test script for checking integration with Alchemy that must be executed manually
    (it's excluded from CI at the moment) - `geth-alchemy-integration-manual-check.test`.
    Instructions on how to run it has been added to package README.

Future improvements:
- Support London fork gas fees (i.e. EIP-1559)
- Refactor API to allow future extensions.
- Fix several TODO items in this connector.

Closes: https://github.com/hyperledger/cacti/issues/2580

Depends on https://github.com/hyperledger/cacti/pull/2535
Depends on https://github.com/hyperledger/cacti/pull/2578

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-25 12:12:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2578" class=".btn">#2578</a>
            </td>
            <td>
                <b>
                    feat(geth-all-in-one): add ethereum test image and helper class
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add new `geth-all-in-one` test image for running ethereum tests in mainnet-like environment. Image is based on `client-go:v1.12.0` and uses Clique (PoS). There is one coinbase account with publicly available keys like in other, similar packages in cacti.
- New image was introduced because currently used open-ethereum one is deprecated.
- Add `geth-all-in-one-publish` CI for publishing new images.
- Add `@hyperledger/cactus-test-geth-ledger` for using new geth ledger container in the tests. The class has been moved out of `cactus-test-tooling` because of conflicting `web3js` versions. Other than that, it's similar to open-ethereum test class.
- Add basic tests for `@hyperledger/cactus-test-geth-ledger`. More tests are being developed right now, and should be available in subsequent PRs.

Closes: #2577
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-25 09:07:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2575" class=".btn">#2575</a>
            </td>
            <td>
                <b>
                    refactor(cacti-cmd-gui-app): rename to cacti-gui-tx-viewer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2572

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-24 18:35:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2574" class=".btn">#2574</a>
            </td>
            <td>
                <b>
                    build(deps): pin ALL dependency versions in package.json files 2023-07-24
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Replaced all tilde and caret characters in package.json
files with nothing so that all versions are pinned down
for safety and stability of the build/publishing process.

Fixes #2571

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-24 18:14:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2568" class=".btn">#2568</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump word-wrap from 1.2.3 to 1.2.5 in /weaver/common/policy-dsl
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [word-wrap](https://github.com/jonschlinkert/word-wrap) from 1.2.3 to 1.2.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/jonschlinkert/word-wrap/releases">word-wrap's releases</a>.</em></p>
<blockquote>
<h2>1.2.5</h2>
<p><strong>Changes</strong>:</p>
<p>Reverts default value for <code>options.indent</code> to two spaces <code>'  '</code>.</p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/jonschlinkert/word-wrap/compare/1.2.4...1.2.5">https://github.com/jonschlinkert/word-wrap/compare/1.2.4...1.2.5</a></p>
<h2>1.2.4</h2>
<h2>What's Changed</h2>
<ul>
<li>Remove default indent by <a href="https://github.com/mohd-akram"><code>@​mohd-akram</code></a> in <a href="https://redirect.github.com/jonschlinkert/word-wrap/pull/24">jonschlinkert/word-wrap#24</a></li>
<li>🔒fix: CVE 2023 26115 (2) by <a href="https://github.com/OlafConijn"><code>@​OlafConijn</code></a> in <a href="https://redirect.github.com/jonschlinkert/word-wrap/pull/41">jonschlinkert/word-wrap#41</a></li>
<li>:lock: fix: CVE-2023-26115 by <a href="https://github.com/aashutoshrathi"><code>@​aashutoshrathi</code></a> in <a href="https://redirect.github.com/jonschlinkert/word-wrap/pull/33">jonschlinkert/word-wrap#33</a></li>
<li>chore: publish workflow by <a href="https://github.com/OlafConijn"><code>@​OlafConijn</code></a> in <a href="https://redirect.github.com/jonschlinkert/word-wrap/pull/42">jonschlinkert/word-wrap#42</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/mohd-akram"><code>@​mohd-akram</code></a> made their first contribution in <a href="https://redirect.github.com/jonschlinkert/word-wrap/pull/24">jonschlinkert/word-wrap#24</a></li>
<li><a href="https://github.com/OlafConijn"><code>@​OlafConijn</code></a> made their first contribution in <a href="https://redirect.github.com/jonschlinkert/word-wrap/pull/41">jonschlinkert/word-wrap#41</a></li>
<li><a href="https://github.com/aashutoshrathi"><code>@​aashutoshrathi</code></a> made their first contribution in <a href="https://redirect.github.com/jonschlinkert/word-wrap/pull/33">jonschlinkert/word-wrap#33</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/jonschlinkert/word-wrap/compare/1.2.3...1.2.4">https://github.com/jonschlinkert/word-wrap/compare/1.2.3...1.2.4</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jonschlinkert/word-wrap/commit/207044ebda1dd3809d15b6000a48409266536771"><code>207044e</code></a> 1.2.5</li>
<li><a href="https://github.com/jonschlinkert/word-wrap/commit/98943154855b0dd79b707462b9202614990c7f61"><code>9894315</code></a> revert default indent</li>
<li><a href="https://github.com/jonschlinkert/word-wrap/commit/f64b188c7261d26b99e1e2075d6b12f21798e83a"><code>f64b188</code></a> run verb to generate README</li>
<li><a href="https://github.com/jonschlinkert/word-wrap/commit/03ea08256ba0c8e8b02b1b304f0f5bd2b1863207"><code>03ea082</code></a> Merge pull request <a href="https://redirect.github.com/jonschlinkert/word-wrap/issues/42">#42</a> from jonschlinkert/chore/publish-workflow</li>
<li><a href="https://github.com/jonschlinkert/word-wrap/commit/420dce9a2412b21881202b73a3c34f0edc53cb2e"><code>420dce9</code></a> Merge pull request <a href="https://redirect.github.com/jonschlinkert/word-wrap/issues/41">#41</a> from jonschlinkert/fix/CVE-2023-26115-2</li>
<li><a href="https://github.com/jonschlinkert/word-wrap/commit/bfa694edf55bb84ff84512f13da6d68bf7593f06"><code>bfa694e</code></a> Update .github/workflows/publish.yml</li>
<li><a href="https://github.com/jonschlinkert/word-wrap/commit/ace0b3c78f81aaf43040bab3bc91d3c5546d3fd2"><code>ace0b3c</code></a> chore: bump version to 1.2.4</li>
<li><a href="https://github.com/jonschlinkert/word-wrap/commit/6fd727594676f3e1b196b08a320908bec2f4ca02"><code>6fd7275</code></a> chore: add publish workflow</li>
<li><a href="https://github.com/jonschlinkert/word-wrap/commit/30d6daf60fce429f5f559252fa86ee78200652c4"><code>30d6daf</code></a> chore: fix test</li>
<li><a href="https://github.com/jonschlinkert/word-wrap/commit/655929cabea6299dddf3b4a21fc3713fca701b48"><code>655929c</code></a> chore: remove package-lock</li>
<li>Additional commits viewable in <a href="https://github.com/jonschlinkert/word-wrap/compare/1.2.3...1.2.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=word-wrap&package-manager=npm_and_yarn&previous-version=1.2.3&new-version=1.2.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-24 09:07:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2567" class=".btn">#2567</a>
            </td>
            <td>
                <b>
                    build(deps): clean up unused karma browser testing dependencies/files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2539

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-24 08:51:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2566" class=".btn">#2566</a>
            </td>
            <td>
                <b>
                    chore(deps): clean up typescript compiler dependency declarations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Pinned all of the versions to 4.9.5 in all of the packages.

Fixes #2532

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-24 07:48:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2565" class=".btn">#2565</a>
            </td>
            <td>
                <b>
                    fix(keychain-vault-server): address CVEs: CVE-2021-22946, CVE-2022-1304, CVE-2018-12886, CVE-2022-29458, CVE-2019-3843, CVE-2019-3844, CVE-2022-29458, CVE-2020-16156
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes: #2058
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-24 00:29:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2564" class=".btn">#2564</a>
            </td>
            <td>
                <b>
                    feat(weaver/common): add data view protocol buffer spec & RFCs for Besu
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                feat(weaver/common): add data view protocol buffer spec & RFCs for Besu
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-22 15:47:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2563" class=".btn">#2563</a>
            </td>
            <td>
                <b>
                    build(deps): fix npm (grpc) build on NodeJS v20.4.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                WORK IN PROGRESS
--------------

1. Eliminates all uses of the old `grpc` dependency from the codebase.
1.1. Upgraded all outdated fabirc-network, fabric-client and fabric-ca-client
dependencies to the latest stable 2.2.x version which is 2.2.18 at the time.
1.2. Also outrighted swapped `grpc` declarations with `@grpc/grpc-js`.
The rest of the diff is due to the incompatibility of the two mentioned.

Fixes https://github.com/hyperledger/cacti/issues/2562
Fixes https://github.com/hyperledger/cacti/issues/1507

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-22 06:38:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2559" class=".btn">#2559</a>
            </td>
            <td>
                <b>
                    feat(connector-tcs-huawei):Modify the initial version. Add some feature. 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Modify the initial version. Add some feature. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-19 09:47:28 +0000 UTC
    </div>
</div>

