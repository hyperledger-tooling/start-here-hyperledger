---
layout: default
title: perun-node
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/perun-node
---

# perun-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/perun-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/228" class=".btn">#228</a>
            </td>
            <td>
                <b>
                    Bump github.com/ethereum/go-ethereum from 1.10.1 to 1.10.10
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/ethereum/go-ethereum](https://github.com/ethereum/go-ethereum) from 1.10.1 to 1.10.10.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/ethereum/go-ethereum/releases">github.com/ethereum/go-ethereum's releases</a>.</em></p>
<blockquote>
<h2>Sytau (v1.10.10)</h2>
<p>Geth v1.10.10 is another bug fix release.</p>
<h4>Geth changes</h4>
<ul>
<li>Geth is much less likely to crash during shutdown, especially when mining is active. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23435">#23435</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/21992">#21992</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/22853">#22853</a>)</li>
<li>The new <code>--rpc.evmtimeout</code> flag allows setting the internal timeout for <code>eth_call</code>. The default timeout is still 5s. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23645">#23645</a>)</li>
<li>The geth console supports some ECMAScript 6 features like arrow functions, typed arrays and let bindings (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23721">#23721</a>)</li>
<li>The console no longer crashes when trying to complete on properties with value 'null' or 'undefined'. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23701">#23701</a>)</li>
<li>The evm debugging/testing tool now validates transaction gas limits in 't9n' mode. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23694">#23694</a>)</li>
</ul>
<h4>RPC API changes</h4>
<ul>
<li>A regression in the JS-based call tracer is resolved. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23667">#23667</a>)</li>
<li>The new <code>debug_getAccessibleState</code> RPC method finds a block number at which full state is available. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23646">#23646</a>)</li>
<li>The new <code>debug_getHeaderRlp</code> RPC method fetches RLP-encoded headers from the database. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23670">#23670</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23677">#23677</a>)</li>
<li>The sender address is once again returned correctly for very old Frontier-era transactions. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23683">#23683</a>)</li>
</ul>
<h4>Go library changes</h4>
<ul>
<li>For contract calls using accounts/abi/bind, a regression that could lead to incorrect gas estimation is fixed. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23719">#23719</a>)</li>
<li>Package accounts/abi now has basic support for Solidity error types. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23161">#23161</a>)</li>
<li>Miner stress test tools work again (they were broken in the previous release) (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23699">#23699</a>)</li>
<li>The transaction recipient address stored in types.Transaction is now truly independent of the address pointer passed to the constructor. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23376">#23376</a>)</li>
<li>The Receipt type now implements encoding.BinaryMarshaler, like Transaction (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/22806">#22806</a>)</li>
<li>TxPool.Pending no longer returns an error (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23720">#23720</a>)</li>
</ul>
<h4>Build</h4>
<ul>
<li>As a workaround for tracing issues on Alpine Linux, we now set the C stack size to 8MB for release builds. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23676">#23676</a>)</li>
<li>Go module vendoring issues related to github.com/karalable/usb are finally resolved. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23684">#23684</a>)</li>
<li>This release is built with Go 1.17.2. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23698">#23698</a>)</li>
</ul>
<p>For a full rundown of the changes please consult the Geth 1.10.10 <a href="https://github.com/ethereum/go-ethereum/milestone/122?closed=1">release milestone</a>.</p>
<hr />
<p>As with all our previous releases, you can find the:</p>
<ul>
<li>Pre-built binaries for all platforms on our <a href="https://geth.ethereum.org/downloads/">downloads page</a>.</li>
<li>Docker images published under <a href="https://cloud.docker.com/u/ethereum/repository/docker/ethereum/client-go"><code>ethereum/client-go</code></a>.</li>
<li>Ubuntu packages in our <a href="https://launchpad.net/~ethereum/+archive/ubuntu/ethereum">Launchpad PPA repository</a>.</li>
<li>OSX packages in our <a href="https://github.com/ethereum/homebrew-ethereum">Homebrew Tap repository</a>.</li>
</ul>
<h2>Attican Beta (v1.10.9)</h2>
<p>Geth v1.10.9 is a maintenance release containing mostly bug fixes.</p>
<p>Chain tracing has received quite a bit of attention during this release cycle. JS-based tracing now supports additional callbacks for entry and exit of contract calls, improving performance if processing individual opcodes is not needed.</p>
<h4>Geth command changes</h4>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ethereum/go-ethereum/commit/bb74230f2a93057b92bf58aab09c9438ce435f95"><code>bb74230</code></a> params: release go-ethereum v1.10.10 stable</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/f915f6873f725b338dc95f0a8add7875af0de912"><code>f915f68</code></a> core/state/snapshot: fix data race in layer flattening (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/23628">#23628</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/08e782c61ff5eb1f5890238c970c95bc6d19c3a6"><code>08e782c</code></a> accounts/abi: add basic support for error types (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/23161">#23161</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/011fe3eb5e29e246ba14e7c9675c536cf7123305"><code>011fe3e</code></a> core: remove unused error from TxPool.Pending (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/23720">#23720</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/79b727bc8aa19a70c0735141e60da003d3624472"><code>79b727b</code></a> accounts/abi/bind: refactor transact method (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/23719">#23719</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/778ff947944f388e2a0307764a182a5521886081"><code>778ff94</code></a> all: fix some go-critic linter warnings (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/23709">#23709</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/e4f570fcc67aa2df489666cc08568c637024fd3c"><code>e4f570f</code></a> core/types: add MarshalBinary, UnmarshalBinary for Receipt (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/22806">#22806</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/f9d683b07f390080c4898260d9824137e0b62a3f"><code>f9d683b</code></a> go.mod: upgrade goja (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/23721">#23721</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/633e7ef4781453111c4b29e14a65c5335bb9ecac"><code>633e7ef</code></a> eth,rpc: allow for flag configured timeouts for eth_call (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/23645">#23645</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/3d11a22c99d195c8bd8a99f3b41e96745d31c360"><code>3d11a22</code></a> fixed broken web3 methods link in README.md (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/23703">#23703</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/ethereum/go-ethereum/compare/v1.10.1...v1.10.10">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/ethereum/go-ethereum&package-manager=go_modules&previous-version=1.10.1&new-version=1.10.10)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/perun-node/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 18:23:48 +0000 UTC
    </div>
</div>

