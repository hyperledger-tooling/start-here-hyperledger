---
layout: default
title: yui-ibc-solidity
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/yui-ibc-solidity
---

# yui-ibc-solidity <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/yui-ibc-solidity){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/163" class=".btn">#163</a>
            </td>
            <td>
                <b>
                    go/relay: update relayer version
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
        Created At 2023-03-13 07:58:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/161" class=".btn">#161</a>
            </td>
            <td>
                <b>
                    build(deps): bump github.com/ethereum/go-ethereum from 1.9.25 to 1.10.22
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/ethereum/go-ethereum](https://github.com/ethereum/go-ethereum) from 1.9.25 to 1.10.22.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/ethereum/go-ethereum/releases">github.com/ethereum/go-ethereum's releases</a>.</em></p>
<blockquote>
<h2>Promavess (v1.10.22)</h2>
<h3>WARNING: This release seems to contain a regression that can corrupt the local state. Please hold on with updating while we investigate the issue!</h3>
<hr />
<p>Geth v1.10.22 <strong>enables the Merge for the Ethereum mainnet at a Terminal Total Difficulty of</strong> <code>58_750_000_000_000_000_000_000</code>.</p>
<p>This TTD is expected to be reached on the 15. September 2022.</p>
<h4>Merge EIPs</h4>
<ul>
<li><a href="https://eips.ethereum.org/EIPS/eip-3675">EIP-3676</a>: Upgrade consensus to Proof-of-Stake</li>
<li><a href="https://eips.ethereum.org/EIPS/eip-4399">EIP-4339</a>: Supplant DIFFICULTY opcode with PREVRANDAO</li>
</ul>
<h4>Additional notes about the merge changes</h4>
<ul>
<li>This release configures the Terminal Total Difficulty for mainnet. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25528">#25528</a>)</li>
<li>Many engine API issues found by hive have been fixed for this release. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25552">#25552</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25423">#25423</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25414">#25414</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25416">#25416</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25428">#25428</a>)</li>
<li>The Goerli testnet is now internally configured as 'successfully merged'. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25519">#25519</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24538">#24538</a>)</li>
</ul>
<h4>JSON-RPC API</h4>
<ul>
<li>The log filtering system now uses a LRU cache for block logs, speeding up repeated queries for the same block range. The cache size can be configured using the <code>--cache.blocklogs</code> command-line flag. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25459">#25459</a>)</li>
<li><code>eth_createAccessList</code> is now much faster when no gas limit is provided. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25467">#25467</a>)</li>
<li><code>eth_feeHistory</code> now also works with the <code>finalized</code> block specifier. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25442">#25442</a>)</li>
<li>The built-in callTracer now supports an option <code>onlyTopCall</code>. Enabling this option makes the tracer skip internal calls. We added this option to enable use of the <code>callTracer</code> to get the return data of reverted transactions. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25430">#25430</a>)</li>
</ul>
<h4>Go-library changes</h4>
<ul>
<li>Storage of trie node hash preimages is now disabled by default. You can enable it again using the <code>--cache.preimages</code> flag. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25287">#25287</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25538">#25538</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25533">#25533</a>)</li>
<li>The ethash mining implemenation now removes temporary DAG files, which could be left of disk when geth was interrupted while generating a DAG. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25381">#25381</a>)</li>
<li>ethclient now supports the <code>eth_feeHistory</code> method. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25403">#25403</a>)</li>
<li>The eth wire protocol test suite now supports protocol version eth/67. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25306">#25306</a>)</li>
<li>RLP-decoding of trie nodes is ~33% faster due to reduced allocations in the decoder. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25357">#25357</a>)</li>
<li>The RPC server supports a new option <code>ReadHeaderTimeout</code>. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25338">#25338</a>)</li>
<li>Registering of clef ruleset UIs should now work correctly. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25455">#25455</a>)</li>
</ul>
<h4>Build</h4>
<ul>
<li>Geth binaries in docker are now statically-linked. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25492">#25492</a>)</li>
<li>This release is built using Go 1.18.5. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25461">#25461</a>)</li>
</ul>
<p>For a full rundown of the changes please consult the Geth <a href="https://github.com/ethereum/go-ethereum/milestone/134?closed=1">1.10.22 release milestone</a></p>
<hr />
<p>As with all our previous releases, you can find the:</p>
<ul>
<li>Pre-built binaries for all platforms on our <a href="https://geth.ethereum.org/downloads/">downloads page</a>.</li>
<li>Docker images published under <a href="https://cloud.docker.com/u/ethereum/repository/docker/ethereum/client-go"><code>ethereum/client-go</code></a>.</li>
<li>Ubuntu packages in our <a href="https://launchpad.net/~ethereum/+archive/ubuntu/ethereum">Launchpad PPA repository</a>.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ethereum/go-ethereum/commit/2de49b04e56cf07f011d6d91f9d5c08847aabe8e"><code>2de49b0</code></a> params: release go-ethereum v1.10.22</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/395f3d4bf689c199e93e05af57ebff09b10f1c9a"><code>395f3d4</code></a> eth/catalyst: warn less frequently if no beacon client is available (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/25569">#25569</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/02418c2fa965e61f5bc1e66e1063482eb5293e5d"><code>02418c2</code></a> Revert &quot;eth/fetcher: don't spend too much time on transaction inclusion&quot; (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/25">#25</a>...</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/0ce494b60cd00d70f1f9f2dd0b9bfbd76204168a"><code>0ce494b</code></a> eth/fetcher: don't spend too much time on transaction inclusion (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/25524">#25524</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/ac7ad811b4d2ba0b93f9272e2487253026620b48"><code>ac7ad81</code></a> internal/ethapi: fix build regression (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/25555">#25555</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/08658806268f4c570c682e87681881ac35123fe9"><code>0865880</code></a> accounts/abi: fix set function (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/25477">#25477</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/36874b63a1b56eed2b8e4b47ccea0337920b84b8"><code>36874b6</code></a> eth/filters: add global block logs cache (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/25459">#25459</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/77308cd6fceb99e276c1e2753d92ff82c6f1a962"><code>77308cd</code></a> consensus/beacon: check ttd reached on pos blocks (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/25552">#25552</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/9762ddf8b0e9d471600c99f158479912f4870c52"><code>9762ddf</code></a> cmd/geth: parse uint64 value with ParseUint instead of Atoi (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/25545">#25545</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/656dc8cc0034d3dd57b5e1baecb788d9c4e9929d"><code>656dc8c</code></a> eth, les: unlock downloader peerSet if there's an error (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/25546">#25546</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/ethereum/go-ethereum/compare/v1.9.25...v1.10.22">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/ethereum/go-ethereum&package-manager=go_modules&previous-version=1.9.25&new-version=1.10.22)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-ibc-solidity/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-07 02:19:09 +0000 UTC
    </div>
</div>

