---
layout: default
title: perun-rs
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/perun-rs
---

# perun-rs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/perun-rs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-rs/pull/10" class=".btn">#10</a>
            </td>
            <td>
                <b>
                    build(deps): bump github.com/ethereum/go-ethereum from 1.10.26 to 1.12.1 in /examples/go-integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/ethereum/go-ethereum](https://github.com/ethereum/go-ethereum) from 1.10.26 to 1.12.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/ethereum/go-ethereum/releases">github.com/ethereum/go-ethereum's releases</a>.</em></p>
<blockquote>
<h2>Antibaar (v1.12.1)</h2>
<p>Geth v1.12.1 is a maintenance release, albeit a rather large one, since we haven't put out a version since May.
This release is a recommended upgrade for all users and contains security-related fixes.</p>
<p>Here's the list of changes:</p>
<h4>Cancun fork</h4>
<p>Development for the upcoming Cancun hard fork has been a focus in this release cycle. Do note however, that Geth v1.12.1 is <strong>not yet ready</strong> for Cancun.</p>
<ul>
<li>For EIP-4844 'Shard Blob Transactions', this release contains basic type definitions and state transition logic (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/27356">#27356</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/27382">#27382</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/27392">#27392</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/27393">#27393</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/27470">#27470</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/27721">#27721</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/27736">#27736</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/27743">#27743</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/27767">#27767</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/27789">#27789</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/27791">#27791</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/27793">#27793</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/27796">#27796</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/27797">#27797</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/27825">#27825</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/27874">#27874</a>)</li>
<li>We have also implemented an entirely new mempool -- the blobpool -- for EIP-4844 transactions. The new pool is backed by an on-disk database and has an overall simpler design than the txpool we use for regular transactions. The blobpool is not yet used by p2p networking and is still being tested in the Cancun devnets. (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/26940">#26940</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/27429">#27429</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/27463">#27463</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/27481">#27481</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/27790">#27790</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/27822">#27822</a>)</li>
<li>EIP-6780: 'SELFDESTRUCT only in same transaction' (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/27189">#27189</a>)</li>
<li>EIP-5656: 'MCOPY instruction' (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/26181">#26181</a>)</li>
<li>EIP-1153: 'Transient storage opcodes' was already implemented and is enabled for Cancun (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/27663">#27663</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/27613">#27613</a>)</li>
</ul>
<h4>Geth command changes</h4>
<ul>
<li>The Rinkeby testnet is no longer supported in Geth (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/27406">#27406</a>)</li>
<li><code>geth --dev</code> now simulates a PoS-based chain (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/27327">#27327</a>)</li>
<li><code>evm blocktest</code> can now output structured logs (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/27396">#27396</a>)</li>
<li>Geth will now configure GOMAXPROCS based on CPU quota settings. This should improve efficiency when running in Docker containers with a CPU core limit applied. (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/27506">#27506</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/27814">#27814</a>)</li>
<li>An IPv6 listening address for can now be configured for HTTP/WS (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/27628">#27628</a>) (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/27635">#27635</a>)</li>
</ul>
<h4>RPC/GraphQL API changes</h4>
<ul>
<li>JSON transactions now have a <code>yParity</code> fields, as mandated by the RPC API spec (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/27744">#27744</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/27882">#27882</a>)</li>
<li>Legacy transactions now have a <code>chainID</code> field in RPC responses, like all other transaction types (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/27452">#27452</a>)</li>
<li>Block headers returned by RPC no longer report a non-standard <code>size</code> field (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/27347">#27347</a>)</li>
<li><code>eth_estimateGas</code> now supports state overrides like <code>eth_call</code> (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/27845">#27845</a>)</li>
<li><code>eth_estimateGas</code> now handles internal chain reorgs more correctly (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/27505">#27505</a>)</li>
<li><code>eth_getProof</code> is slight more efficient, and will now return a response in the canonical encoding even for off-spec input parameters (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/27309">#27309</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/27310">#27310</a>)</li>
<li><code>eth_getTransactionReceipt</code> now returns <code>null</code> when the transaction is not available. It used return an error in that case. (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/27712">#27712</a>)</li>
<li><code>debug_storageRangeAt</code> now takes a block hash or number as parameter (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/27328">#27328</a>)</li>
<li>The new <code>debug_getTrieFlushInterval</code> method reports the internal state saving interval (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/27303">#27303</a>)</li>
<li>A crash in the prestate tracer is resolved (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/27691">#27691</a>)</li>
<li>Structured EVM logs returned by tracing now contain the <code>returnData</code> (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/27704">#27704</a>)</li>
<li>GraphQL now supports withdrawals (EIP-4895) (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/27072">#27072</a>)</li>
</ul>
<h4>Go library changes</h4>
<ul>
<li>The RPC server now enforces limits on batch requests and responses. This is a potentially breaking change.
If you use batch requests with geth, and also use the go-ethereum RPC client library, <strong>we strongly recommend updating your go-ethereum library dependency</strong> as well. The new client version handles invalid batch responses way better than before. (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/26681">#26681</a>)</li>
<li>The RPC client has multiple new ways to test whether the transport supports real time subscriptions (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/25942">#25942</a>)</li>
<li>fsync is now enabled for pebble database writes (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/27615">#27615</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/27522">#27522</a>)</li>
<li>Function calls timed by metrics will now run even if metrics are disabled (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/27724">#27724</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/27723">#27723</a>)</li>
<li><code>Node.Attach</code> no longer returns an error. This is a breaking Go API change. (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/27450">#27450</a>)</li>
<li>The keystore has improved verification of keys loaded from disk (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/27432">#27432</a>)</li>
<li>Per-level metrics are now available for LevelDB (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/27643">#27643</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ethereum/go-ethereum/commit/9c216bd6cbd7f0d3ab179700907a53409beeca9b"><code>9c216bd</code></a> params: release go-ethereum v1.12.1</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/67979022aa8ea6a96b618c086f60b49af7d2a568"><code>6797902</code></a> core/state: move UpdateContractCode before the trie hash is computed (<a href="https://redirect.github.com/ethereum/go-ethereum/issues/27853">#27853</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/10d9f9377bae3fc9e0474d4bd49698db5beef579"><code>10d9f93</code></a> graphql: add yParity field for transactions (<a href="https://redirect.github.com/ethereum/go-ethereum/issues/27882">#27882</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/7ec60d5f0c45bc68fd4e814479df065acec95d60"><code>7ec60d5</code></a> p2p: move ping handling into pingLoop goroutine (<a href="https://redirect.github.com/ethereum/go-ethereum/issues/27887">#27887</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/e13fa32cea3497aa311226c62daf21c5847c8e4f"><code>e13fa32</code></a> core/vm: update 4844 - point evaluation precompile address (<a href="https://redirect.github.com/ethereum/go-ethereum/issues/27874">#27874</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/0d772b9f094285227c5d89fb61cb57e206e94199"><code>0d772b9</code></a> graphql: avoid greedy allocation (<a href="https://redirect.github.com/ethereum/go-ethereum/issues/27873">#27873</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/6d2bcb911a85d7d7003a09b7dd029b0af38da377"><code>6d2bcb9</code></a> p2p/simulations/examples: use atomic.Int64 (<a href="https://redirect.github.com/ethereum/go-ethereum/issues/27861">#27861</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/eeebb07c735e0f10ee0945d47fe85591dd9baec8"><code>eeebb07</code></a> internal/ethapi: add state override to estimateGas (<a href="https://redirect.github.com/ethereum/go-ethereum/issues/27845">#27845</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/d14c07d91e565c0d97cfcee3aa84a08ce08d93bf"><code>d14c07d</code></a> accounts: use atomic type (<a href="https://redirect.github.com/ethereum/go-ethereum/issues/27857">#27857</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/857476753dc8a8b3f090c60c08a05b41d42aced9"><code>8574767</code></a> internal: use atomic type (<a href="https://redirect.github.com/ethereum/go-ethereum/issues/27858">#27858</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/ethereum/go-ethereum/compare/v1.10.26...v1.12.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/ethereum/go-ethereum&package-manager=go_modules&previous-version=1.10.26&new-version=1.12.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/perun-rs/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-06 19:54:09 +0000 UTC
    </div>
</div>

