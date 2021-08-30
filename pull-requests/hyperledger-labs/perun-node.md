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
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/226" class=".btn">#226</a>
            </td>
            <td>
                <b>
                    Bump github.com/ethereum/go-ethereum from 1.10.1 to 1.10.8
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/ethereum/go-ethereum](https://github.com/ethereum/go-ethereum) from 1.10.1 to 1.10.8.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/ethereum/go-ethereum/releases">github.com/ethereum/go-ethereum's releases</a>.</em></p>
<blockquote>
<h2>Hades Gamma (v1.10.8)</h2>
<p>Geth v1.10.8 is a pre-announced <em><strong>hotfix release to patch a vulnerability in the EVM</strong></em> (<code>CVE-2021-39137</code>).</p>
<p>The exact attack vector will be provided at a later date to give node operators and dependent downstream projects time to update their nodes and software. All Geth versions supporting the London hard fork are vulnerable (the bug is older than London), so all users should update.</p>
<p>Credits for the discovery go to <a href="https://github.com/guidovranken"><code>@​guidovranken</code></a> (working for <a href="https://sentnl.io/">Sentnl</a> during an audit of the <a href="https://www.telos.net/evm">Telos EVM</a>) and reported via <a href="mailto:bounty@ethereum.org">bounty@ethereum.org</a>.</p>
<p>Beside the fix, we're merged in a few tiny polishes and fixes. For a rundown, please consult the Geth 1.10.8 <a href="https://github.com/ethereum/go-ethereum/milestone/120?closed=1">release milestone</a>.</p>
<hr />
<p>As with all our previous releases, you can find the:</p>
<ul>
<li>Pre-built binaries for all platforms on our <a href="https://geth.ethereum.org/downloads/">downloads page</a>.</li>
<li>Docker images published under <a href="https://cloud.docker.com/u/ethereum/repository/docker/ethereum/client-go"><code>ethereum/client-go</code></a>.</li>
<li>Ubuntu packages in our <a href="https://launchpad.net/~ethereum/+archive/ubuntu/ethereum">Launchpad PPA repository</a>.</li>
<li>OSX packages in our <a href="https://github.com/ethereum/homebrew-ethereum">Homebrew Tap repository</a>.</li>
</ul>
<h2>Styx Theta (v1.10.7)</h2>
<p>Geth v1.10.7 is a maintenance release, mostly focusing on a few post-London polishes.</p>
<p><strong>A few important notes to keep in mind:</strong></p>
<ul>
<li><strong>The return type for <code>oldestBlock</code> in <code>eth_feeHistory</code> was changed from decimal to hex.</strong> This is to conform to the updated spec that was released after Geth's London hard-fork release was already made. The input <code>blockCount</code> parameter was also updated, but there Geth will accept both hex and decimal to keep backward compatibility.</li>
<li><strong>The <code>-miner.gastarget</code> CLI flag was deprecated and is a noop.</strong> This flag is already a noop for networks running the London hard-fork, since it London miners only take into account the <code>-miner.gaslimit</code> flag. For non-London private networks and Geth forks, this might result in a gas bump depending on how the miners are configured.</li>
<li>Docker builds were changed from DockerHub Automated Builds to offsite builds and manual pushes to DockerHub. At the same time, we've added support for multi-arch images, the original tags being the metadata image, linking a <code>-amd64</code> and a <code>-arm64</code> tags together. No changes are needed for docker users, but keep us posted if something strange happens. On the upside, Geth now has official <code>arm64</code> docker images too.</li>
</ul>
<p>Changes made:</p>
<ul>
<li>Change the <code>oldestBlock</code> return type in <code>eth_feeHistory</code> to hex, accept both decimal and hex as the block count (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23239">#23239</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23363">#23363</a>).</li>
<li>Cap max usable gas in <code>eth_estimateGas</code> better for 1559 transactions (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23309">#23309</a>).</li>
<li>When deploying multiple contracts via abigen, only parse the ABI once (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/22583">#22583</a>).</li>
<li>Return <code>maxFeePerGas</code> for the <code>gasPrice</code> of pending transactions (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23345">#23345</a>).</li>
<li>Check cached blocks too when attempting to retrieve a header (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23299">#23299</a>).</li>
<li>Reject transactions imitated from non EOA accounts (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23303">#23303</a>).</li>
<li>Reduce allocations a bit while CPU mining ethash (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23199">#23199</a>).</li>
<li>Deprecate the <code>-miner.gastarget</code> CLI flag (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23213">#23213</a>).</li>
<li>Switch over to manual docker pushes (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23373">#23373</a>).</li>
</ul>
<p>Bugs fixed:</p>
<ul>
<li>Fix a <code>nil</code> pointer panic for certain abigen generated code due to missing context initialization (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23188">#23188</a>).</li>
<li>Fix <code> nil</code> pointer panic in certain automatic access list generation RPC API calls (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23225">#23225</a>).</li>
<li>Fix a regression that prevented <code>clef</code> from signing a legacy transaction (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23274">#23274</a>).</li>
<li>Fix a permission error during snapshot based pruning on Windows (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23370">#23370</a>).</li>
<li>Fix the marshaling of errors from the tracers (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/23292">#23292</a>).</li>
</ul>
<p>For a full rundown of the changes please consult the Geth 1.10.7 <a href="https://github.com/ethereum/go-ethereum/milestone/119?closed=1">release milestone</a>.</p>
<hr />
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ethereum/go-ethereum/commit/26675454bf93bf904be7a43cce6b3f550115ff90"><code>2667545</code></a> params: release Geth v1.10.8</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/1d995731923ca899964371ddb213d40b7e773818"><code>1d99573</code></a> core/vm: faster code analysis (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/23381">#23381</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/f38abc55f135587ce3cf60c9d574ec2a4ebb8197"><code>f38abc5</code></a> eth/gasprice: feeHistory improvements (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/23422">#23422</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/dfeb2f7e8001aef1005a8d5e1605bae1de0b4f12"><code>dfeb2f7</code></a> go.mod: upgrade golang.org/x/sys for go1.17 support (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/23406">#23406</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/bb1f7ebf203f40dae714a3b8445918cfcfc9a7db"><code>bb1f7eb</code></a> signer/core/apitypes: remove dependency on internal/ethapi (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/23362">#23362</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/d02c60536799698888d21f093f7c379acdad3147"><code>d02c605</code></a> core: only check sendernoeoa in non fake mode (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/23424">#23424</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/c368f728c19e7fd7a9613513edda68ffcb503af0"><code>c368f72</code></a> Revert &quot;eth: drop eth/65, the last non-reqid protocol version&quot; (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/23426">#23426</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/5566e5d152c490e5e533f3bc7735dddd57a428eb"><code>5566e5d</code></a> eth/downloader: fix typo in comment (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/23413">#23413</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/57feabea663496109e59df669238398239438fb1"><code>57feabe</code></a> eth, internal/ethapi: make RPC block miner field show block sealer correctly ...</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/16ecdd583984162923256e563320b8b381da7f46"><code>16ecdd5</code></a> cmd/utils: add --nousb to the list of deprecated flags (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/23388">#23388</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/ethereum/go-ethereum/compare/v1.10.1...v1.10.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/ethereum/go-ethereum&package-manager=go_modules&previous-version=1.10.1&new-version=1.10.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-08-30 16:36:38 +0000 UTC
    </div>
</div>

