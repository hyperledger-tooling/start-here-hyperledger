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
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/279" class=".btn">#279</a>
            </td>
            <td>
                <b>
                    Bump github.com/cometbft/cometbft from 0.38.7 to 0.38.8
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/cometbft/cometbft](https://github.com/cometbft/cometbft) from 0.38.7 to 0.38.8.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/cometbft/cometbft/releases">github.com/cometbft/cometbft's releases</a>.</em></p>
<blockquote>
<h2>v0.38.8</h2>
<p>See the <a href="https://github.com/cometbft/cometbft/blob/v0.38.8/CHANGELOG.md#v0388">CHANGELOG</a> for this release.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/cometbft/cometbft/blob/v0.38.8/CHANGELOG.md">github.com/cometbft/cometbft's changelog</a>.</em></p>
<blockquote>
<h2>v0.38.8</h2>
<p><em>June 27, 2024</em></p>
<p>This release contains a few bug fixes and performance improvements.</p>
<h3>BREAKING CHANGES</h3>
<ul>
<li><code>[mempool]</code> Add to the <code>Mempool</code> interface a new method <code>PreUpdate()</code>. This method should be
called before acquiring the mempool lock, to signal that a new update is coming. Also add to
<code>ErrMempoolIsFull</code> a new field <code>RecheckFull</code>.
(<a href="https://redirect.github.com/cometbft/cometbft/pull/3314">#3314</a>)</li>
</ul>
<h3>BUG FIXES</h3>
<ul>
<li>[<code>mempool</code>] Fix data race when rechecking with async ABCI client
(<a href="https://redirect.github.com/cometbft/cometbft/issues/1827">#1827</a>)</li>
<li><code>[consensus]</code> Fix a race condition in the consensus timeout ticker. Race is caused by two timeouts being scheduled at the same time.
(<a href="https://redirect.github.com/cometbft/cometbft/pull/2136">#3092</a>)</li>
<li><code>[types]</code> Do not batch verify a commit if the validator set keys have different
types. (<a href="https://redirect.github.com/cometbft/cometbft/issues/3195">#3195</a></li>
</ul>
<h3>IMPROVEMENTS</h3>
<ul>
<li><code>[blockstore]</code> Added peer banning in blockstore
(<a href="https://github.com/cometbft/cometbft/security/advisories/GHSA-hg58-rf2h-6rr7">#ABC-0013</a>)</li>
<li><code>[blockstore]</code> Send correct error message when vote extensions do not align with received packet
(<a href="https://github.com/cometbft/cometbft/security/advisories/GHSA-hg58-rf2h-6rr7">#ABC-0014</a>)</li>
<li><code>[config]</code> Added <code>recheck_timeout</code> mempool parameter to set how much time to wait for recheck
responses from the app (only applies to non-local ABCI clients).
(<a href="https://redirect.github.com/cometbft/cometbft/issues/1827/">#1827</a>)</li>
<li><code>[rpc]</code> Add a configurable maximum batch size for RPC requests.
(<a href="https://redirect.github.com/cometbft/cometbft/pull/2867">#2867</a>).</li>
<li><code>[event-bus]</code> Remove the debug logs in PublishEventTx, which were noticed production slowdowns.
(<a href="https://redirect.github.com/cometbft/cometbft/pull/2911">#2911</a>)</li>
<li><code>[state/execution]</code> Cache the block hash computation inside of the Block Type, so we only compute it once.
(<a href="https://redirect.github.com/cometbft/cometbft/pull/2924">#2924</a>)</li>
<li><code>[consensus/state]</code> Remove a redundant <code>VerifyBlock</code> call in <code>FinalizeCommit</code>
(<a href="https://redirect.github.com/cometbft/cometbft/pull/2928">#2928</a>)</li>
<li><code>[p2p/channel]</code> Speedup <code>ProtoIO</code> writer creation time, and thereby speedup channel writing by 5%.
(<a href="https://redirect.github.com/cometbft/cometbft/pull/2949">#2949</a>)</li>
<li><code>[p2p/conn]</code> Minor speedup (3%) to connection.WritePacketMsgTo, by removing MinInt calls.
(<a href="https://redirect.github.com/cometbft/cometbft/pull/2952">#2952</a>)</li>
<li><code>[internal/bits]</code> 10x speedup creating initialized bitArrays, which speedsup extendedCommit.BitArray(). This is used in consensus vote gossip.
(<a href="https://redirect.github.com/cometbft/cometbft/pull/2841">#2959</a>).</li>
<li><code>[blockstore]</code> Remove a redundant <code>Header.ValidateBasic</code> call in <code>LoadBlockMeta</code>, 75% reducing this time.
(<a href="https://redirect.github.com/cometbft/cometbft/pull/2964">#2964</a>)</li>
<li><code>[p2p/conn]</code> Speedup connection.WritePacketMsgTo, by reusing internal buffers rather than re-allocating.
(<a href="https://redirect.github.com/cometbft/cometbft/pull/2986">#2986</a>)</li>
<li>[<code>blockstore</code>] Use LRU caches in blockstore, significiantly improving consensus gossip routine performance</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/cometbft/cometbft/commit/69592051835d9e534e567943c895cc7f0ba7d8c2"><code>6959205</code></a> Release/v0.38.8 (<a href="https://redirect.github.com/cometbft/cometbft/issues/3350">#3350</a>)</li>
<li><a href="https://github.com/cometbft/cometbft/commit/8ba2e4f52d5e626e019501ba6420cc86d5de7857"><code>8ba2e4f</code></a> Merge pull request from GHSA-hg58-rf2h-6rr7</li>
<li><a href="https://github.com/cometbft/cometbft/commit/0a89ec13a557a9554f65b9d6c90de96ca0ff06da"><code>0a89ec1</code></a> Update blocksync/pool_test.go</li>
<li><a href="https://github.com/cometbft/cometbft/commit/065810cdc25878cdf500a8adad07b58a6c974ea2"><code>065810c</code></a> Readded good peer to test</li>
<li><a href="https://github.com/cometbft/cometbft/commit/007efd72981a97a9a8170478bad15f5b22281f8a"><code>007efd7</code></a> Removed defers from test</li>
<li><a href="https://github.com/cometbft/cometbft/commit/4199f274cadab9f1ec775c2541a7785d04ff070c"><code>4199f27</code></a> Remove one thread to make test more compact</li>
<li><a href="https://github.com/cometbft/cometbft/commit/8a473ca9c1710f177a02cb22f0b027a4af98ec9d"><code>8a473ca</code></a> Update blocksync/pool_test.go</li>
<li><a href="https://github.com/cometbft/cometbft/commit/872210cb1f8a608961bdf3d04c2746c64d17e2d8"><code>872210c</code></a> Update blocksync/pool_test.go</li>
<li><a href="https://github.com/cometbft/cometbft/commit/4cb0df8321feee9343a5da6db3e3f128787a28ac"><code>4cb0df8</code></a> Update blocksync/pool_test.go</li>
<li><a href="https://github.com/cometbft/cometbft/commit/26bda8b7ffb3647d6f6ca37d1a3117798e98e060"><code>26bda8b</code></a> Test assertions have more detail</li>
<li>Additional commits viewable in <a href="https://github.com/cometbft/cometbft/compare/v0.38.7...v0.38.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/cometbft/cometbft&package-manager=go_modules&previous-version=0.38.7&new-version=0.38.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-ibc-solidity/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-28 14:35:29 +0000 UTC
    </div>
</div>

