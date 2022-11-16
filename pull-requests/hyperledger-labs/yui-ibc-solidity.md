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
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/124" class=".btn">#124</a>
            </td>
            <td>
                <b>
                    Fix missing updates in generated go code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jun Kimura <jun.kimura@datachain.jp>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-16 09:14:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/123" class=".btn">#123</a>
            </td>
            <td>
                <b>
                    build(deps): bump minimatch and truffle
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [minimatch](https://github.com/isaacs/minimatch) to 3.1.2 and updates ancestor dependency [truffle](https://github.com/trufflesuite/truffle/tree/HEAD/packages/truffle). These dependencies need to be updated together.

Updates `minimatch` from 3.0.4 to 3.1.2
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/isaacs/minimatch/commit/699c459443a6bd98f5b28197978f76e7f71467ac"><code>699c459</code></a> 3.1.2</li>
<li><a href="https://github.com/isaacs/minimatch/commit/2f2b5ff1bb1b6a01f4404f7e475f0a2cba578ab7"><code>2f2b5ff</code></a> fix: trim pattern</li>
<li><a href="https://github.com/isaacs/minimatch/commit/25d7c0d09c47063c9b0d2ace17ef8e951d90eccc"><code>25d7c0d</code></a> 3.1.1</li>
<li><a href="https://github.com/isaacs/minimatch/commit/55dda291dfb595bd11b4edb19b45dd98eda76de0"><code>55dda29</code></a> fix: treat nocase:true as always having magic</li>
<li><a href="https://github.com/isaacs/minimatch/commit/5e1fb8dd2bb78c0ae22101b9229fac4c76ef039e"><code>5e1fb8d</code></a> 3.1.0</li>
<li><a href="https://github.com/isaacs/minimatch/commit/f8145c54f34075069f4a23cb214d871da4cd4006"><code>f8145c5</code></a> Add 'allowWindowsEscape' option</li>
<li><a href="https://github.com/isaacs/minimatch/commit/570e8b1aef6c9e823a824aa0b9be10db43857cd7"><code>570e8b1</code></a> add publishConfig for v3 publishes</li>
<li><a href="https://github.com/isaacs/minimatch/commit/5b7cd3372be253759fb4d865eb3f38f189a5fcdf"><code>5b7cd33</code></a> 3.0.6</li>
<li><a href="https://github.com/isaacs/minimatch/commit/20b4b562830680867feb75f9c635aca08e5c86ff"><code>20b4b56</code></a> [fix] revert all breaking syntax changes</li>
<li><a href="https://github.com/isaacs/minimatch/commit/2ff038852ec03e85e60e0eb333005c680ac8a543"><code>2ff0388</code></a> document, expose, and test 'partial:true' option</li>
<li>Additional commits viewable in <a href="https://github.com/isaacs/minimatch/compare/v3.0.4...v3.1.2">compare view</a></li>
</ul>
</details>
<br />

Updates `truffle` from 5.1.58 to 5.6.5
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/trufflesuite/truffle/releases">truffle's releases</a>.</em></p>
<blockquote>
<h2>v5.6.5 — Slurping noodles in the woods</h2>
<p>If a wild Truffle release runs by unnoticed in the woods 🦌, do its legs make a sound? Er, or I mean if it falls on a tree does it makes sound? 🌳 Or something?</p>
<p>Fall cools things down, turns the leaves brown and red, and makes us a bit quieter and introspective. Just a bit like here in the Truffle camp where we've been directing focus inward, deep into the internals of Truffle to make improvements. It's getting better all the time!</p>
<p>Aside from this mass of improvements, there was a bug fixed with the <code>config</code> command. Some problem with a logger was causing it to crash when fetching a value. &quot;Well&quot;, we thought, &quot;crashing is no fun!&quot;. And because we love fun so much 👻, we fixed it!</p>
<p>One other thing to mention, is that there are some more sourcify networks that got added to the source-fetcher. I suppose this is now a monthly thing for us to grow this list of networks. It is a well-known fact, of course, that &quot;more networks&quot; = &quot;more fun&quot;, and you already know how we feel about fun...👯🏼‍♀️</p>
<p>Welp, as mentioned there are also a bunch of improvements to the internals of Truffle. An unnecessary dependency got removed here and some updates were made to the test suite. Some dead code was removed and a README had some improvements made to it. README improvements are fun, right?</p>
<p>So we hope you add some soy sauce, get a forkful, and slurp it down with some noodles. 🍜 Happy Truffling!</p>
<h2>How to upgrade</h2>
<p>We recommend upgrading to the latest version of Truffle by running:</p>
<pre><code>npm uninstall -g truffle
npm install -g truffle
</code></pre>
<h2>Changelog</h2>
<h3>Enhancement</h3>
<ul>
<li>add some more sourcify networks (<a href="https://github-redirect.dependabot.com/trufflesuite/truffle/pull/5689">#5689</a> by <a href="https://github.com/haltman-at"><code>@​haltman-at</code></a>)</li>
</ul>
<h3>Bug fix</h3>
<ul>
<li>fix Truffle Config's logger (<a href="https://github-redirect.dependabot.com/trufflesuite/truffle/pull/5685">#5685</a> by <a href="https://github.com/cds-amal"><code>@​cds-amal</code></a>)</li>
</ul>
<h3>Internal improvements</h3>
<ul>
<li>remove spinners package from compile-solidity and log in events (<a href="https://github-redirect.dependabot.com/trufflesuite/truffle/pull/5672">#5672</a> by <a href="https://github.com/eggplantzzz"><code>@​eggplantzzz</code></a>)</li>
<li>add <code>.prettierignore</code> (<a href="https://github-redirect.dependabot.com/trufflesuite/truffle/pull/5678">#5678</a> by <a href="https://github.com/sukanyaparashar"><code>@​sukanyaparashar</code></a>)</li>
<li>improve the readme for fetch-and-compile (<a href="https://github-redirect.dependabot.com/trufflesuite/truffle/pull/5660">#5660</a> by <a href="https://github.com/eggplantzzz"><code>@​eggplantzzz</code></a>)</li>
<li>remove ethpm-v1 concerns (<a href="https://github-redirect.dependabot.com/trufflesuite/truffle/pull/5665">#5665</a> by <a href="https://github.com/cds-amal"><code>@​cds-amal</code></a>)</li>
<li>return cleanup callback from sandbox test utility and update tests (<a href="https://github-redirect.dependabot.com/trufflesuite/truffle/pull/5641">#5641</a> by <a href="https://github.com/eggplantzzz"><code>@​eggplantzzz</code></a>)</li>
<li>add two more reminders to PR template (<a href="https://github-redirect.dependabot.com/trufflesuite/truffle/pull/5666">#5666</a> by <a href="https://github.com/haltman-at"><code>@​haltman-at</code></a>)</li>
</ul>
<h3>Dependency updates</h3>
<ul>
<li>bump babel-loader to 9.1.0 (<a href="https://github-redirect.dependabot.com/trufflesuite/truffle/pull/5683">#5683</a> by <a href="https://github.com/haltman-at"><code>@​haltman-at</code></a>)</li>
<li>bump loader-utils to 1.4.1 (<a href="https://github-redirect.dependabot.com/trufflesuite/truffle/pull/5682">#5682</a> by <a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
<li>bump apollo-server to ^3.11.0 (<a href="https://github-redirect.dependabot.com/trufflesuite/truffle/pull/5669">#5669</a> by <a href="https://github.com/haltman-at"><code>@​haltman-at</code></a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/trufflesuite/truffle/commit/275115e1ce358aad3050a7583c034e5d19d885a1"><code>275115e</code></a> Publish</li>
<li><a href="https://github.com/trufflesuite/truffle/commit/7066f6f65011a8417adfbce66c6bd8ce313adb22"><code>7066f6f</code></a> Merge pull request <a href="https://github.com/trufflesuite/truffle/tree/HEAD/packages/truffle/issues/5665">#5665</a> from trufflesuite/drop/ethpm-v1</li>
<li><a href="https://github.com/trufflesuite/truffle/commit/e36fbbed5a1e1948ad9009f348d8d58a9ae7a91f"><code>e36fbbe</code></a> Merge pull request <a href="https://github.com/trufflesuite/truffle/tree/HEAD/packages/truffle/issues/5641">#5641</a> from trufflesuite/update-sandbox</li>
<li><a href="https://github.com/trufflesuite/truffle/commit/495e923676ca47ff7ff4c32b10c0af89ecadaa3a"><code>495e923</code></a> Publish</li>
<li><a href="https://github.com/trufflesuite/truffle/commit/0a16e1500ce47bc2bcdd3fb40a1ea609e92a6e98"><code>0a16e15</code></a> remove db from dev deps in truffle</li>
<li><a href="https://github.com/trufflesuite/truffle/commit/3a31e15d2137d5564aa91b508c26a385e8964387"><code>3a31e15</code></a> Remove ethpm-v1 concerns</li>
<li><a href="https://github.com/trufflesuite/truffle/commit/4ab767e9c6be7e4a2dd6aef14c2b8aa48c96ca9c"><code>4ab767e</code></a> update call to sandbox method after rebasing</li>
<li><a href="https://github.com/trufflesuite/truffle/commit/c21a610b06bfa96583ee107deb8a50655e45728b"><code>c21a610</code></a> remove console.log</li>
<li><a href="https://github.com/trufflesuite/truffle/commit/48eaffe519e3a343384d2f94e937563583548a04"><code>48eaffe</code></a> correct error in test setup</li>
<li><a href="https://github.com/trufflesuite/truffle/commit/bf7d29a485a393efddc01052d7af519c2569a576"><code>bf7d29a</code></a> correct error in test</li>
<li>Additional commits viewable in <a href="https://github.com/trufflesuite/truffle/commits/truffle@5.6.5/packages/truffle">compare view</a></li>
</ul>
</details>
<br />


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
        Created At 2022-11-16 08:42:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/122" class=".btn">#122</a>
            </td>
            <td>
                <b>
                    build(deps): bump github.com/btcsuite/btcd from 0.22.1 to 0.23.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/btcsuite/btcd](https://github.com/btcsuite/btcd) from 0.22.1 to 0.23.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/btcsuite/btcd/releases">github.com/btcsuite/btcd's releases</a>.</em></p>
<blockquote>
<h2>btcd v0.23.2</h2>
<h2>What's Changed</h2>
<ul>
<li>MuSig2: Catch up to 0.4.0 by <a href="https://github.com/sputn1ck"><code>@​sputn1ck</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1865">btcsuite/btcd#1865</a></li>
<li>Bump btcd version in btcutil package by <a href="https://github.com/darioush"><code>@​darioush</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1866">btcsuite/btcd#1866</a></li>
<li>doc: fix Tor hidden service setup link by <a href="https://github.com/shyba"><code>@​shyba</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1883">btcsuite/btcd#1883</a></li>
<li>build: bump golang base image version to 1.17 by <a href="https://github.com/tochicool"><code>@​tochicool</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1882">btcsuite/btcd#1882</a></li>
<li>wire: remove erroneous witness size check in wire parsing by <a href="https://github.com/Roasbeef"><code>@​Roasbeef</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1896">btcsuite/btcd#1896</a></li>
<li>build: bump version to v0.23.2 by <a href="https://github.com/Roasbeef"><code>@​Roasbeef</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1898">btcsuite/btcd#1898</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/sputn1ck"><code>@​sputn1ck</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1865">btcsuite/btcd#1865</a></li>
<li><a href="https://github.com/darioush"><code>@​darioush</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1866">btcsuite/btcd#1866</a></li>
<li><a href="https://github.com/shyba"><code>@​shyba</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1883">btcsuite/btcd#1883</a></li>
<li><a href="https://github.com/tochicool"><code>@​tochicool</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1882">btcsuite/btcd#1882</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/btcsuite/btcd/compare/v0.23.1...v0.23.2">https://github.com/btcsuite/btcd/compare/v0.23.1...v0.23.2</a></p>
<h2>btcd v0.23.1-beta</h2>
<h2>What's Changed</h2>
<ul>
<li>btcjson: Update WalletCreateFundedPsbtOpts.FeeRate type by <a href="https://github.com/gnasr"><code>@​gnasr</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1729">btcsuite/btcd#1729</a></li>
<li>rpcserverhelp: Remove extra period for gettxout--synopsis by <a href="https://github.com/kcalvinalvin"><code>@​kcalvinalvin</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1733">btcsuite/btcd#1733</a></li>
<li>mempool: export isDust for use in other projects by <a href="https://github.com/Crypt-iQ"><code>@​Crypt-iQ</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1739">btcsuite/btcd#1739</a></li>
<li>Switch irc to libera.chat by <a href="https://github.com/jcvernaleo"><code>@​jcvernaleo</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1725">btcsuite/btcd#1725</a></li>
<li>rpcclient: Export symbols needed for custom commands by <a href="https://github.com/JeremyRand"><code>@​JeremyRand</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1457">btcsuite/btcd#1457</a></li>
<li>btcec: check if recovered pk is at point of infinity by <a href="https://github.com/MariusVanDerWijden"><code>@​MariusVanDerWijden</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1750">btcsuite/btcd#1750</a></li>
<li>mempool: introduce GetDustThreshold to export dust limit calculation by <a href="https://github.com/Crypt-iQ"><code>@​Crypt-iQ</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1742">btcsuite/btcd#1742</a></li>
<li>build: bump min Go version to 1.16.8 add Go 1.17.1 by <a href="https://github.com/Roasbeef"><code>@​Roasbeef</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1753">btcsuite/btcd#1753</a></li>
<li>Upgraded the docker version to 1.16 by <a href="https://github.com/naveensrinivasan"><code>@​naveensrinivasan</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1755">btcsuite/btcd#1755</a></li>
<li>peer+server: add new config option to optionally disable stall detection by <a href="https://github.com/Roasbeef"><code>@​Roasbeef</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1752">btcsuite/btcd#1752</a></li>
<li>addrmgr: make KnownAddress methods thread-safe by <a href="https://github.com/chappjc"><code>@​chappjc</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1763">btcsuite/btcd#1763</a></li>
<li>comment improvement by <a href="https://github.com/pyh4"><code>@​pyh4</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1762">btcsuite/btcd#1762</a></li>
<li>Included permissions for GitHub action by <a href="https://github.com/naveensrinivasan"><code>@​naveensrinivasan</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1756">btcsuite/btcd#1756</a></li>
<li>connmgr: Fix stale comment in TestRemovePendingConnection by <a href="https://github.com/sloorush"><code>@​sloorush</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1749">btcsuite/btcd#1749</a></li>
<li>rpcclient: Add retry with backoffs to HTTP POST requests by <a href="https://github.com/3nprob"><code>@​3nprob</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1743">btcsuite/btcd#1743</a></li>
<li>txscript: backport tokenizer from dcrd by <a href="https://github.com/Roasbeef"><code>@​Roasbeef</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1769">btcsuite/btcd#1769</a></li>
<li>go.mod, go.sum: Update goleveldb by <a href="https://github.com/kcalvinalvin"><code>@​kcalvinalvin</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1770">btcsuite/btcd#1770</a></li>
<li>reduce redundant memory allocation - resolves <a href="https://github-redirect.dependabot.com/btcsuite/btcd/issues/1699">btcsuite/btcd#1699</a> by <a href="https://github.com/ziollek"><code>@​ziollek</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1759">btcsuite/btcd#1759</a></li>
<li>rpcclient+rpcserver+integration: GetNetworkHashPS3 must be float64 by <a href="https://github.com/mattbajorek"><code>@​mattbajorek</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1778">btcsuite/btcd#1778</a></li>
<li>multi: move the btcutil repo into btcd as a sub-module by <a href="https://github.com/Roasbeef"><code>@​Roasbeef</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1785">btcsuite/btcd#1785</a></li>
<li>btcutil: update modules to replace to top-level btcd repo by <a href="https://github.com/Roasbeef"><code>@​Roasbeef</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1788">btcsuite/btcd#1788</a></li>
<li>chaincfg+blockchain: abstract/refactor BIP 9 version bits implementation to work w/ BIP 8 block heights  by <a href="https://github.com/Roasbeef"><code>@​Roasbeef</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1700">btcsuite/btcd#1700</a></li>
<li>btcec: create new btcec/v2 module that type aliases into the dcrec module by <a href="https://github.com/Roasbeef"><code>@​Roasbeef</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1773">btcsuite/btcd#1773</a></li>
<li>btcec/v2: create new schnorr package for BIP-340, move existing ecdsa implementation into new ecdsa package by <a href="https://github.com/Roasbeef"><code>@​Roasbeef</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1777">btcsuite/btcd#1777</a></li>
<li>build: update to btcec v2.1.0 by <a href="https://github.com/Roasbeef"><code>@​Roasbeef</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1801">btcsuite/btcd#1801</a></li>
<li>build: retract bogus tags from btcd fork by <a href="https://github.com/Roasbeef"><code>@​Roasbeef</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1805">btcsuite/btcd#1805</a></li>
<li>mempool/estimatefee: Fix negative index bug by <a href="https://github.com/kcalvinalvin"><code>@​kcalvinalvin</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1813">btcsuite/btcd#1813</a></li>
<li>Replace github.com/btcsuite/goleveldb imports with github.com/syndtr/goleveldb by <a href="https://github.com/anupcshan"><code>@​anupcshan</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1780">btcsuite/btcd#1780</a></li>
<li>Remove circular dependency issue between <code>btcec/v2</code> and main package by <a href="https://github.com/guggero"><code>@​guggero</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1823">btcsuite/btcd#1823</a></li>
<li>Fixes coveralls coverage report by <a href="https://github.com/vpereira01"><code>@​vpereira01</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1814">btcsuite/btcd#1814</a></li>
<li>Update LICENSE by <a href="https://github.com/MarnixCroes"><code>@​MarnixCroes</code></a> in <a href="https://github-redirect.dependabot.com/btcsuite/btcd/pull/1809">btcsuite/btcd#1809</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/btcsuite/btcd/commit/6b5418d5850f5b9977c9b13725d79c5c81d0c1db"><code>6b5418d</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/btcsuite/btcd/issues/1898">#1898</a> from Roasbeef/v0-23-2-branch</li>
<li><a href="https://github.com/btcsuite/btcd/commit/1a4af39ab02a1a4fb1f2a01e12fafccea82aa442"><code>1a4af39</code></a> build: bump version to v0.23.2</li>
<li><a href="https://github.com/btcsuite/btcd/commit/d0aa7473a6b593c807842888dc9fe781a5984a78"><code>d0aa747</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/btcsuite/btcd/issues/1896">#1896</a> from Roasbeef/witness-wire-hot-fix</li>
<li><a href="https://github.com/btcsuite/btcd/commit/f523d4ccaa5f34a2f761f16a05f5d6e6665b1168"><code>f523d4c</code></a> wire: remove erroneous witness size check in wire parsing</li>
<li><a href="https://github.com/btcsuite/btcd/commit/38ee9a41c8f8aa24a079a28f5e8a86faecffdfe1"><code>38ee9a4</code></a> build: bump golang base image version to 1.17</li>
<li><a href="https://github.com/btcsuite/btcd/commit/ef4a8d310b18953718fc99fc536aa39ecf4d8ab7"><code>ef4a8d3</code></a> doc: fix Tor hidden service setup link</li>
<li><a href="https://github.com/btcsuite/btcd/commit/0f49e1000633b0af6d7bbef97d69671f4c99e37e"><code>0f49e10</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/btcsuite/btcd/issues/1866">#1866</a> from darioush/bump-btcutils-versions</li>
<li><a href="https://github.com/btcsuite/btcd/commit/da4b534ed915023ec44e841469df48c2ebe94b2d"><code>da4b534</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/btcsuite/btcd/issues/1865">#1865</a> from sputn1ck/musig2_0.3.0</li>
<li><a href="https://github.com/btcsuite/btcd/commit/06ce9608aa3bd2de895b5c12e545e9e0f2935c42"><code>06ce960</code></a> btcec/schnorr/musig2: add infinity testvectors</li>
<li><a href="https://github.com/btcsuite/btcd/commit/44eb8c64f8d0f0e3a84400e7f93b9eb16ea08873"><code>44eb8c6</code></a> btcec/schnorr/musig2: Allow infinity nonces</li>
<li>Additional commits viewable in <a href="https://github.com/btcsuite/btcd/compare/v0.22.1...v0.23.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/btcsuite/btcd&package-manager=go_modules&previous-version=0.22.1&new-version=0.23.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-11-16 08:38:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/121" class=".btn">#121</a>
            </td>
            <td>
                <b>
                    Introduce code formatting tool and check it on CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix #118 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-16 08:19:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/120" class=".btn">#120</a>
            </td>
            <td>
                <b>
                    Move generated proto codes into contracts/proto
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jun Kimura <jun.kimura@datachain.jp>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-16 07:37:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/117" class=".btn">#117</a>
            </td>
            <td>
                <b>
                    Update tests and follow-up #115
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
        Created At 2022-11-16 06:45:26 +0000 UTC
    </div>
</div>

