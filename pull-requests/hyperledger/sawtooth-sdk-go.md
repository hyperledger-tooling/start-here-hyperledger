---
layout: default
title: sawtooth-sdk-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/sawtooth-sdk-go
---

# sawtooth-sdk-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/sawtooth-sdk-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-sdk-go/pull/56" class=".btn">#56</a>
            </td>
            <td>
                <b>
                    Bump github.com/btcsuite/btcd from 0.22.1 to 0.23.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
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
<li>MuSig2: Catch up to 0.4.0 by <a href="https://github.com/sputn1ck"><code>@​sputn1ck</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1865">btcsuite/btcd#1865</a></li>
<li>Bump btcd version in btcutil package by <a href="https://github.com/darioush"><code>@​darioush</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1866">btcsuite/btcd#1866</a></li>
<li>doc: fix Tor hidden service setup link by <a href="https://github.com/shyba"><code>@​shyba</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1883">btcsuite/btcd#1883</a></li>
<li>build: bump golang base image version to 1.17 by <a href="https://github.com/tochicool"><code>@​tochicool</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1882">btcsuite/btcd#1882</a></li>
<li>wire: remove erroneous witness size check in wire parsing by <a href="https://github.com/Roasbeef"><code>@​Roasbeef</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1896">btcsuite/btcd#1896</a></li>
<li>build: bump version to v0.23.2 by <a href="https://github.com/Roasbeef"><code>@​Roasbeef</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1898">btcsuite/btcd#1898</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/sputn1ck"><code>@​sputn1ck</code></a> made their first contribution in <a href="https://redirect.github.com/btcsuite/btcd/pull/1865">btcsuite/btcd#1865</a></li>
<li><a href="https://github.com/darioush"><code>@​darioush</code></a> made their first contribution in <a href="https://redirect.github.com/btcsuite/btcd/pull/1866">btcsuite/btcd#1866</a></li>
<li><a href="https://github.com/shyba"><code>@​shyba</code></a> made their first contribution in <a href="https://redirect.github.com/btcsuite/btcd/pull/1883">btcsuite/btcd#1883</a></li>
<li><a href="https://github.com/tochicool"><code>@​tochicool</code></a> made their first contribution in <a href="https://redirect.github.com/btcsuite/btcd/pull/1882">btcsuite/btcd#1882</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/btcsuite/btcd/compare/v0.23.1...v0.23.2">https://github.com/btcsuite/btcd/compare/v0.23.1...v0.23.2</a></p>
<h2>btcd v0.23.1-beta</h2>
<h2>What's Changed</h2>
<ul>
<li>btcjson: Update WalletCreateFundedPsbtOpts.FeeRate type by <a href="https://github.com/gnasr"><code>@​gnasr</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1729">btcsuite/btcd#1729</a></li>
<li>rpcserverhelp: Remove extra period for gettxout--synopsis by <a href="https://github.com/kcalvinalvin"><code>@​kcalvinalvin</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1733">btcsuite/btcd#1733</a></li>
<li>mempool: export isDust for use in other projects by <a href="https://github.com/Crypt-iQ"><code>@​Crypt-iQ</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1739">btcsuite/btcd#1739</a></li>
<li>Switch irc to libera.chat by <a href="https://github.com/jcvernaleo"><code>@​jcvernaleo</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1725">btcsuite/btcd#1725</a></li>
<li>rpcclient: Export symbols needed for custom commands by <a href="https://github.com/JeremyRand"><code>@​JeremyRand</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1457">btcsuite/btcd#1457</a></li>
<li>btcec: check if recovered pk is at point of infinity by <a href="https://github.com/MariusVanDerWijden"><code>@​MariusVanDerWijden</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1750">btcsuite/btcd#1750</a></li>
<li>mempool: introduce GetDustThreshold to export dust limit calculation by <a href="https://github.com/Crypt-iQ"><code>@​Crypt-iQ</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1742">btcsuite/btcd#1742</a></li>
<li>build: bump min Go version to 1.16.8 add Go 1.17.1 by <a href="https://github.com/Roasbeef"><code>@​Roasbeef</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1753">btcsuite/btcd#1753</a></li>
<li>Upgraded the docker version to 1.16 by <a href="https://github.com/naveensrinivasan"><code>@​naveensrinivasan</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1755">btcsuite/btcd#1755</a></li>
<li>peer+server: add new config option to optionally disable stall detection by <a href="https://github.com/Roasbeef"><code>@​Roasbeef</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1752">btcsuite/btcd#1752</a></li>
<li>addrmgr: make KnownAddress methods thread-safe by <a href="https://github.com/chappjc"><code>@​chappjc</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1763">btcsuite/btcd#1763</a></li>
<li>comment improvement by <a href="https://github.com/pyh4"><code>@​pyh4</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1762">btcsuite/btcd#1762</a></li>
<li>Included permissions for GitHub action by <a href="https://github.com/naveensrinivasan"><code>@​naveensrinivasan</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1756">btcsuite/btcd#1756</a></li>
<li>connmgr: Fix stale comment in TestRemovePendingConnection by <a href="https://github.com/sloorush"><code>@​sloorush</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1749">btcsuite/btcd#1749</a></li>
<li>rpcclient: Add retry with backoffs to HTTP POST requests by <a href="https://github.com/3nprob"><code>@​3nprob</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1743">btcsuite/btcd#1743</a></li>
<li>txscript: backport tokenizer from dcrd by <a href="https://github.com/Roasbeef"><code>@​Roasbeef</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1769">btcsuite/btcd#1769</a></li>
<li>go.mod, go.sum: Update goleveldb by <a href="https://github.com/kcalvinalvin"><code>@​kcalvinalvin</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1770">btcsuite/btcd#1770</a></li>
<li>reduce redundant memory allocation - resolves <a href="https://redirect.github.com/btcsuite/btcd/issues/1699">btcsuite/btcd#1699</a> by <a href="https://github.com/ziollek"><code>@​ziollek</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1759">btcsuite/btcd#1759</a></li>
<li>rpcclient+rpcserver+integration: GetNetworkHashPS3 must be float64 by <a href="https://github.com/mattbajorek"><code>@​mattbajorek</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1778">btcsuite/btcd#1778</a></li>
<li>multi: move the btcutil repo into btcd as a sub-module by <a href="https://github.com/Roasbeef"><code>@​Roasbeef</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1785">btcsuite/btcd#1785</a></li>
<li>btcutil: update modules to replace to top-level btcd repo by <a href="https://github.com/Roasbeef"><code>@​Roasbeef</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1788">btcsuite/btcd#1788</a></li>
<li>chaincfg+blockchain: abstract/refactor BIP 9 version bits implementation to work w/ BIP 8 block heights  by <a href="https://github.com/Roasbeef"><code>@​Roasbeef</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1700">btcsuite/btcd#1700</a></li>
<li>btcec: create new btcec/v2 module that type aliases into the dcrec module by <a href="https://github.com/Roasbeef"><code>@​Roasbeef</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1773">btcsuite/btcd#1773</a></li>
<li>btcec/v2: create new schnorr package for BIP-340, move existing ecdsa implementation into new ecdsa package by <a href="https://github.com/Roasbeef"><code>@​Roasbeef</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1777">btcsuite/btcd#1777</a></li>
<li>build: update to btcec v2.1.0 by <a href="https://github.com/Roasbeef"><code>@​Roasbeef</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1801">btcsuite/btcd#1801</a></li>
<li>build: retract bogus tags from btcd fork by <a href="https://github.com/Roasbeef"><code>@​Roasbeef</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1805">btcsuite/btcd#1805</a></li>
<li>mempool/estimatefee: Fix negative index bug by <a href="https://github.com/kcalvinalvin"><code>@​kcalvinalvin</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1813">btcsuite/btcd#1813</a></li>
<li>Replace github.com/btcsuite/goleveldb imports with github.com/syndtr/goleveldb by <a href="https://github.com/anupcshan"><code>@​anupcshan</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1780">btcsuite/btcd#1780</a></li>
<li>Remove circular dependency issue between <code>btcec/v2</code> and main package by <a href="https://github.com/guggero"><code>@​guggero</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1823">btcsuite/btcd#1823</a></li>
<li>Fixes coveralls coverage report by <a href="https://github.com/vpereira01"><code>@​vpereira01</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1814">btcsuite/btcd#1814</a></li>
<li>Update LICENSE by <a href="https://github.com/MarnixCroes"><code>@​MarnixCroes</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1809">btcsuite/btcd#1809</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/btcsuite/btcd/commit/6b5418d5850f5b9977c9b13725d79c5c81d0c1db"><code>6b5418d</code></a> Merge pull request <a href="https://redirect.github.com/btcsuite/btcd/issues/1898">#1898</a> from Roasbeef/v0-23-2-branch</li>
<li><a href="https://github.com/btcsuite/btcd/commit/1a4af39ab02a1a4fb1f2a01e12fafccea82aa442"><code>1a4af39</code></a> build: bump version to v0.23.2</li>
<li><a href="https://github.com/btcsuite/btcd/commit/d0aa7473a6b593c807842888dc9fe781a5984a78"><code>d0aa747</code></a> Merge pull request <a href="https://redirect.github.com/btcsuite/btcd/issues/1896">#1896</a> from Roasbeef/witness-wire-hot-fix</li>
<li><a href="https://github.com/btcsuite/btcd/commit/f523d4ccaa5f34a2f761f16a05f5d6e6665b1168"><code>f523d4c</code></a> wire: remove erroneous witness size check in wire parsing</li>
<li><a href="https://github.com/btcsuite/btcd/commit/38ee9a41c8f8aa24a079a28f5e8a86faecffdfe1"><code>38ee9a4</code></a> build: bump golang base image version to 1.17</li>
<li><a href="https://github.com/btcsuite/btcd/commit/ef4a8d310b18953718fc99fc536aa39ecf4d8ab7"><code>ef4a8d3</code></a> doc: fix Tor hidden service setup link</li>
<li><a href="https://github.com/btcsuite/btcd/commit/0f49e1000633b0af6d7bbef97d69671f4c99e37e"><code>0f49e10</code></a> Merge pull request <a href="https://redirect.github.com/btcsuite/btcd/issues/1866">#1866</a> from darioush/bump-btcutils-versions</li>
<li><a href="https://github.com/btcsuite/btcd/commit/da4b534ed915023ec44e841469df48c2ebe94b2d"><code>da4b534</code></a> Merge pull request <a href="https://redirect.github.com/btcsuite/btcd/issues/1865">#1865</a> from sputn1ck/musig2_0.3.0</li>
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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/sawtooth-sdk-go/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-02 11:11:07 +0000 UTC
    </div>
</div>

