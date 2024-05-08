---
layout: default
title: weaver-dlt-interoperability
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/weaver-dlt-interoperability
---

# weaver-dlt-interoperability <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/weaver-dlt-interoperability){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/456" class=".btn">#456</a>
            </td>
            <td>
                <b>
                    Updates and Cleanup as Preparation for Archival
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added deprecation notes and suggestions for users to migrate to using Hyperledger Cacti.
Deleting unnecessary and obsolete files.
Fixing typos and updating dependencies to avoid vulnerabilities and match what's currently in Hyperledger Cacti.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-08 08:26:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/455" class=".btn">#455</a>
            </td>
            <td>
                <b>
                    build(deps): Bump github.com/ethereum/go-ethereum from 1.11.6 to 1.13.15 in /core/network/fabric-interop-cc/contracts/interop
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/ethereum/go-ethereum](https://github.com/ethereum/go-ethereum) from 1.11.6 to 1.13.15.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/ethereum/go-ethereum/releases">github.com/ethereum/go-ethereum's releases</a>.</em></p>
<blockquote>
<h2>Ontamalca (v1.13.15)</h2>
<p>Geth v1.13.15 is a maintenance-release that contains some fixes mainly to avoid snapsync-related data-corruption.</p>
<p>We recommend all users to upgrade to v1.13.15 as soon as possible.</p>
<hr />
<p>As with all our previous releases, you can find the:</p>
<ul>
<li>Pre-built binaries for all platforms on our <a href="https://geth.ethereum.org/downloads/">downloads page</a>.</li>
<li>Docker images published under <a href="https://cloud.docker.com/u/ethereum/repository/docker/ethereum/client-go"><code>ethereum/client-go</code></a>.</li>
<li>Ubuntu packages in our <a href="https://launchpad.net/~ethereum/+archive/ubuntu/ethereum">Launchpad PPA repository</a>.</li>
<li>OSX packages in our <a href="https://github.com/ethereum/homebrew-ethereum">Homebrew Tap repository</a>.</li>
</ul>
<h2>Altaaya (v1.13.14)</h2>
<p>Geth v1.13.14 is a small maintenance release with a handful of polishes to the blob pool:</p>
<ul>
<li>Disallow blob transactions below the protocol minimum of 1 wei to enter the pool (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/29081">#29081</a>).</li>
<li>Reduce the blob pool's max capacity to 2.5GB for the rollout. (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/29090">#29090</a>).</li>
<li>Fix gas estimation for blob transactions (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/29085">#29085</a>).</li>
</ul>
<p><em><strong>This release is NOT critical for the Cancun fork, but recommended to make Geth lighter in anticipation to unknown blob load.</strong></em></p>
<p>Other fixes:</p>
<ul>
<li>Support overriding the basefee during tracing (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/29051">#29051</a>).</li>
<li>Fix call tracers missing top level logs in top-only mode (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/29068">#29068</a>).</li>
<li>Support unlimited gas for <code>eth_createAccessList</code> if <code>--gascap=0</code> (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/28846">#28846</a>).</li>
</ul>
<p>For a full rundown of the changes please consult the Geth <a href="https://github.com/ethereum/go-ethereum/milestone/162?closed=1">1.13.14 release milestone</a>.</p>
<hr />
<p>As with all our previous releases, you can find the:</p>
<ul>
<li>Pre-built binaries for all platforms on our <a href="https://geth.ethereum.org/downloads/">downloads page</a>.</li>
<li>Docker images published under <a href="https://cloud.docker.com/u/ethereum/repository/docker/ethereum/client-go"><code>ethereum/client-go</code></a>.</li>
<li>Ubuntu packages in our <a href="https://launchpad.net/~ethereum/+archive/ubuntu/ethereum">Launchpad PPA repository</a>.</li>
<li>OSX packages in our <a href="https://github.com/ethereum/homebrew-ethereum">Homebrew Tap repository</a>.</li>
</ul>
<h2>Alsages (v1.13.13)</h2>
<p>This is a minor release with fixes for several issues related to the upcoming Cancun mainnet fork. As such, it is recommended for all mainnet users.</p>
<p>Changes in this release:</p>
<ul>
<li>Block-building performance with blob transactions has been improved a lot. (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/29026">#29026</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/29008">#29008</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/29005">#29005</a>)</li>
<li>A corner case in the EVM related to out-of-order fork scheduling has been fixed. (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/29023">#29023</a>)</li>
<li><code>eth_fillTransaction</code> has seen some bug fixes related to blob transactions as well. (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/28929">#28929</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/29037">#29037</a>)</li>
<li>A rare panic in the ethstats client related to chain reorgs is resolved. (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/29020">#29020</a>)</li>
<li>The blobpool database will now recover from disk corruption faults instead of crashing geth on startup. (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/29001">#29001</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ethereum/go-ethereum/commit/c5ba367eb6232e3eddd7d6226bfd374449c63164"><code>c5ba367</code></a> params: release Geth v 1.13.15</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/35e0525bf47a16eb1deb2a278552707a324b4c23"><code>35e0525</code></a> core, eth/protocols/snap, trie: fix cause for snap-sync corruption, implement...</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/7bcb5532a5c5da3f5ace3abef23c8f807dd9ab79"><code>7bcb553</code></a> eth/filters: enforce topic-limit early on filter criterias (<a href="https://redirect.github.com/ethereum/go-ethereum/issues/29535">#29535</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/e343ddf9eb39a68c12effd1575275c4888c1cbc9"><code>e343ddf</code></a> core/rawdb: add sanity-limit to header accessor (<a href="https://redirect.github.com/ethereum/go-ethereum/issues/29534">#29534</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/5dcf5032b5590e1a74a7bc65f47860cf9ffda5e8"><code>5dcf503</code></a> eth/protocols/snap: skip retrieval for completed storages (<a href="https://redirect.github.com/ethereum/go-ethereum/issues/29378">#29378</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/2bd6bd01d2e8561dd7fc21b631f4a34ac16627a1"><code>2bd6bd0</code></a> Merge branch 'master' into release/1.13</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/9038ba69428a6ecada1f2acace6981854482748b"><code>9038ba6</code></a> params: release Geth v1.13.14</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/51b479e56459d663a12f95fd8eaba82716c0d5ce"><code>51b479e</code></a> core/txpool: elevate the 'already reserved' error into a constant (<a href="https://redirect.github.com/ethereum/go-ethereum/issues/29095">#29095</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/5a0f468f8cb15b939bd85445d33c614a36942a8e"><code>5a0f468</code></a> eth/tracers: Fix callTracer logs on onlyTopCall == true (<a href="https://redirect.github.com/ethereum/go-ethereum/issues/29068">#29068</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/45a272c7b96cb260528bbc2e31d657488f97c4b0"><code>45a272c</code></a> core/txpool: no need to log loud rotate if no local txs (<a href="https://redirect.github.com/ethereum/go-ethereum/issues/29083">#29083</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/ethereum/go-ethereum/compare/v1.11.6...v1.13.15">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/ethereum/go-ethereum&package-manager=go_modules&previous-version=1.11.6&new-version=1.13.15)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-06 14:36:20 +0000 UTC
    </div>
</div>

