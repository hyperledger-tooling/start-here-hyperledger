---
layout: default
title: blockchain-carbon-accounting
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-carbon-accounting
---

# blockchain-carbon-accounting <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-carbon-accounting){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/691" class=".btn">#691</a>
            </td>
            <td>
                <b>
                    Bump semver and nodemon
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [semver](https://github.com/npm/node-semver) to 7.5.4 and updates ancestor dependency [nodemon](https://github.com/remy/nodemon). These dependencies need to be updated together.

Updates `semver` from 7.3.7 to 7.5.4
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/npm/node-semver/releases">semver's releases</a>.</em></p>
<blockquote>
<h2>v7.5.4</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.3...v7.5.4">7.5.4</a> (2023-07-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/cc6fde2d34b95cb600d126649d926901bd2a9703"><code>cc6fde2</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/588">#588</a> trim each range set before parsing (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/99d8287516a1d2abf0286033e2e26eca6b69c09f"><code>99d8287</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/583">#583</a> correctly parse long build ids as valid (<a href="https://redirect.github.com/npm/node-semver/issues/583">#583</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h2>v7.5.3</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.2...v7.5.3">7.5.3</a> (2023-06-22)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/abdd93d55496d22e3c15a454a5cf13f101e48bce"><code>abdd93d</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/571">#571</a> set max lengths in regex for numeric and build identifiers (<a href="https://redirect.github.com/npm/node-semver/issues/571">#571</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/bf53dd8da15a17eb6b8111115d0d8ef341fea5db"><code>bf53dd8</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/569">#569</a> add example for <code>&gt;</code> comparator (<a href="https://redirect.github.com/npm/node-semver/issues/569">#569</a>) (<a href="https://github.com/mbtools"><code>@​mbtools</code></a>)</li>
</ul>
<h2>v7.5.2</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.1...v7.5.2">7.5.2</a> (2023-06-15)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/58c791f40ba8cf4be35a5ca6644353ecd6249edc"><code>58c791f</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/566">#566</a> diff when detecting major change from prerelease (<a href="https://redirect.github.com/npm/node-semver/issues/566">#566</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/5c8efbcb3c6c125af10746d054faff13e8c33fbd"><code>5c8efbc</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/565">#565</a> preserve build in raw after inc (<a href="https://redirect.github.com/npm/node-semver/issues/565">#565</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/717534ee353682f3bcf33e60a8af4292626d4441"><code>717534e</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/564">#564</a> better handling of whitespace (<a href="https://redirect.github.com/npm/node-semver/issues/564">#564</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h2>v7.5.1</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.0...v7.5.1">7.5.1</a> (2023-05-12)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/d30d25a5c1fb963c3cc9178cb1769fe45e4a3cab"><code>d30d25a</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/559">#559</a> show type on invalid semver error (<a href="https://redirect.github.com/npm/node-semver/issues/559">#559</a>) (<a href="https://github.com/tjenkinson"><code>@​tjenkinson</code></a>)</li>
</ul>
<h2>v7.5.0</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.4.0...v7.5.0">7.5.0</a> (2023-04-17)</h2>
<h3>Features</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/503a4e52fe2b1c6ed1400d33149f7733c8361eed"><code>503a4e5</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/548">#548</a> allow identifierBase to be false (<a href="https://redirect.github.com/npm/node-semver/issues/548">#548</a>) (<a href="https://github.com/lsvalina"><code>@​lsvalina</code></a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/e219bb454036a0c23e34407591f921c8edb688e7"><code>e219bb4</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/552">#552</a> throw on bad version with correct error message (<a href="https://redirect.github.com/npm/node-semver/issues/552">#552</a>) (<a href="https://github.com/wraithgar"><code>@​wraithgar</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/fc2f3df0b5d25253b3580607e111a9a280d888ca"><code>fc2f3df</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/546">#546</a> incorrect results from diff sometimes with prerelease versions (<a href="https://redirect.github.com/npm/node-semver/issues/546">#546</a>) (<a href="https://github.com/tjenkinson"><code>@​tjenkinson</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/27817677794f592b592bf6181a80a4824ff762b2"><code>2781767</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/547">#547</a> avoid re-instantiating SemVer during diff compare (<a href="https://redirect.github.com/npm/node-semver/issues/547">#547</a>) (<a href="https://github.com/macno"><code>@​macno</code></a>)</li>
</ul>
<h2>v7.4.0</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.3.8...v7.4.0">7.4.0</a> (2023-04-10)</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/npm/node-semver/blob/main/CHANGELOG.md">semver's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.3...v7.5.4">7.5.4</a> (2023-07-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/cc6fde2d34b95cb600d126649d926901bd2a9703"><code>cc6fde2</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/588">#588</a> trim each range set before parsing (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/99d8287516a1d2abf0286033e2e26eca6b69c09f"><code>99d8287</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/583">#583</a> correctly parse long build ids as valid (<a href="https://redirect.github.com/npm/node-semver/issues/583">#583</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.2...v7.5.3">7.5.3</a> (2023-06-22)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/abdd93d55496d22e3c15a454a5cf13f101e48bce"><code>abdd93d</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/571">#571</a> set max lengths in regex for numeric and build identifiers (<a href="https://redirect.github.com/npm/node-semver/issues/571">#571</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/bf53dd8da15a17eb6b8111115d0d8ef341fea5db"><code>bf53dd8</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/569">#569</a> add example for <code>&gt;</code> comparator (<a href="https://redirect.github.com/npm/node-semver/issues/569">#569</a>) (<a href="https://github.com/mbtools"><code>@​mbtools</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.1...v7.5.2">7.5.2</a> (2023-06-15)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/58c791f40ba8cf4be35a5ca6644353ecd6249edc"><code>58c791f</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/566">#566</a> diff when detecting major change from prerelease (<a href="https://redirect.github.com/npm/node-semver/issues/566">#566</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/5c8efbcb3c6c125af10746d054faff13e8c33fbd"><code>5c8efbc</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/565">#565</a> preserve build in raw after inc (<a href="https://redirect.github.com/npm/node-semver/issues/565">#565</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/717534ee353682f3bcf33e60a8af4292626d4441"><code>717534e</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/564">#564</a> better handling of whitespace (<a href="https://redirect.github.com/npm/node-semver/issues/564">#564</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.0...v7.5.1">7.5.1</a> (2023-05-12)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/d30d25a5c1fb963c3cc9178cb1769fe45e4a3cab"><code>d30d25a</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/559">#559</a> show type on invalid semver error (<a href="https://redirect.github.com/npm/node-semver/issues/559">#559</a>) (<a href="https://github.com/tjenkinson"><code>@​tjenkinson</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.4.0...v7.5.0">7.5.0</a> (2023-04-17)</h2>
<h3>Features</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/503a4e52fe2b1c6ed1400d33149f7733c8361eed"><code>503a4e5</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/548">#548</a> allow identifierBase to be false (<a href="https://redirect.github.com/npm/node-semver/issues/548">#548</a>) (<a href="https://github.com/lsvalina"><code>@​lsvalina</code></a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/e219bb454036a0c23e34407591f921c8edb688e7"><code>e219bb4</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/552">#552</a> throw on bad version with correct error message (<a href="https://redirect.github.com/npm/node-semver/issues/552">#552</a>) (<a href="https://github.com/wraithgar"><code>@​wraithgar</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/fc2f3df0b5d25253b3580607e111a9a280d888ca"><code>fc2f3df</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/546">#546</a> incorrect results from diff sometimes with prerelease versions (<a href="https://redirect.github.com/npm/node-semver/issues/546">#546</a>) (<a href="https://github.com/tjenkinson"><code>@​tjenkinson</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/27817677794f592b592bf6181a80a4824ff762b2"><code>2781767</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/547">#547</a> avoid re-instantiating SemVer during diff compare (<a href="https://redirect.github.com/npm/node-semver/issues/547">#547</a>) (<a href="https://github.com/macno"><code>@​macno</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.3.8...v7.4.0">7.4.0</a> (2023-04-10)</h2>
<h3>Features</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/113f51312a1a6b6aa50d4f9486b4fde21782c1f5"><code>113f513</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/532">#532</a> identifierBase parameter for .inc (<a href="https://redirect.github.com/npm/node-semver/issues/532">#532</a>) (<a href="https://github.com/wraithgar"><code>@​wraithgar</code></a>, <a href="https://github.com/b-bly"><code>@​b-bly</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/48d8f8fa63bf6e35db70ff840b6da1a51596a5a8"><code>48d8f8f</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/530">#530</a> export new RELEASE_TYPES constant (<a href="https://github.com/hcharley"><code>@​hcharley</code></a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/36cd334708ec1f85a71445622fb1864bceee0f4e"><code>36cd334</code></a> chore: release 7.5.4</li>
<li><a href="https://github.com/npm/node-semver/commit/8456d87971a447ce295d9f1a396b37b29a972a63"><code>8456d87</code></a> chore: postinstall for dependabot template-oss PR</li>
<li><a href="https://github.com/npm/node-semver/commit/dde1f002baadf7b4cc45504c4046d13586de11b7"><code>dde1f00</code></a> chore: postinstall for dependabot template-oss PR</li>
<li><a href="https://github.com/npm/node-semver/commit/dffcd1b07ec6a192bc0fb405d30d19da46fdc690"><code>dffcd1b</code></a> chore: bump <code>@​npmcli/template-oss</code> from 4.16.0 to 4.17.0</li>
<li><a href="https://github.com/npm/node-semver/commit/d619f66513a0fa953177882ecee2c365a65efe97"><code>d619f66</code></a> chore: postinstall for dependabot template-oss PR</li>
<li><a href="https://github.com/npm/node-semver/commit/3bc42477d1a69361eb79978851be090e5fb4bc2a"><code>3bc4247</code></a> chore: bump <code>@​npmcli/template-oss</code> from 4.15.1 to 4.16.0</li>
<li><a href="https://github.com/npm/node-semver/commit/cc6fde2d34b95cb600d126649d926901bd2a9703"><code>cc6fde2</code></a> fix: trim each range set before parsing</li>
<li><a href="https://github.com/npm/node-semver/commit/99d8287516a1d2abf0286033e2e26eca6b69c09f"><code>99d8287</code></a> fix: correctly parse long build ids as valid (<a href="https://redirect.github.com/npm/node-semver/issues/583">#583</a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/4f0f6b19a54b1ba7e1c62af2dfba61f7a4fa68d5"><code>4f0f6b1</code></a> chore: fix arguments in whitespace test (<a href="https://redirect.github.com/npm/node-semver/issues/574">#574</a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/6bd1a37f95904512015353a3a5dd726f785c9eb8"><code>6bd1a37</code></a> chore: remove duplicate test in semver class (<a href="https://redirect.github.com/npm/node-semver/issues/575">#575</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/npm/node-semver/compare/v7.3.7...v7.5.4">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~npm-cli-ops">npm-cli-ops</a>, a new releaser for semver since your current version.</p>
</details>
<br />

Updates `nodemon` from 2.0.20 to 3.0.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/remy/nodemon/releases">nodemon's releases</a>.</em></p>
<blockquote>
<h2>v3.0.1</h2>
<h2><a href="https://github.com/remy/nodemon/compare/v3.0.0...v3.0.1">3.0.1</a> (2023-07-09)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>restore default ext watch behaviour (<a href="https://github.com/remy/nodemon/commit/95bee008bfb4eb77d7826f193e9386812652f449">95bee00</a>), closes <a href="https://redirect.github.com/remy/nodemon/issues/2124">#2124</a> <a href="https://redirect.github.com/remy/nodemon/issues/1957">#1957</a></li>
</ul>
<h2>v3.0.0</h2>
<h1><a href="https://github.com/remy/nodemon/compare/v2.0.22...v3.0.0">3.0.0</a> (2023-07-08)</h1>
<h3>Bug Fixes</h3>
<ul>
<li>also watch cjs (<a href="https://github.com/remy/nodemon/commit/86d5f403a3e06e8aed48b37fa854730dc83257be">86d5f40</a>)</li>
<li>node@10 support back in (<a href="https://github.com/remy/nodemon/commit/af3b9e237281beffd92ceee0e2411ef53edcf375">af3b9e2</a>)</li>
<li>semver vuln dep (<a href="https://github.com/remy/nodemon/commit/6bb876666715e16464d48f98cd4bc2cba172a970">6bb8766</a>), closes <a href="https://redirect.github.com/remy/nodemon/issues/2119">#2119</a></li>
</ul>
<h3>Features</h3>
<ul>
<li>always use polling on IBM i (<a href="https://github.com/remy/nodemon/commit/3b5810463e7c39b0a8e2856c996faf454a6ca1f8">3b58104</a>)</li>
</ul>
<h3>BREAKING CHANGES</h3>
<ul>
<li>official support for node@8 dropped.</li>
</ul>
<p>However there's no function being used in semver that breaks node 8,
so it's technically still possible to run with node 8, but it will
no longer be supported (or tested in CI).</p>
<h2>v2.0.22</h2>
<h2><a href="https://github.com/remy/nodemon/compare/v2.0.21...v2.0.22">2.0.22</a> (2023-03-22)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>remove ts mapping if loader present (<a href="https://github.com/remy/nodemon/commit/f7816e445b61e77dd57d5c9ccf5fa0be4f9b18a7">f7816e4</a>), closes <a href="https://redirect.github.com/remy/nodemon/issues/2083">#2083</a></li>
</ul>
<h2>v2.0.21</h2>
<h2><a href="https://github.com/remy/nodemon/compare/v2.0.20...v2.0.21">2.0.21</a> (2023-03-02)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>remove ts mapping if loader present (<a href="https://github.com/remy/nodemon/commit/146839711be58995f88723b29de3007de87d6c3a">1468397</a>), closes <a href="https://redirect.github.com/remy/nodemon/issues/2083">#2083</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/remy/nodemon/commit/e4c163f7f5c8f73f6e42499b53bf0329d14a9895"><code>e4c163f</code></a> Merge branch 'main' of github.com:remy/nodemon</li>
<li><a href="https://github.com/remy/nodemon/commit/95bee008bfb4eb77d7826f193e9386812652f449"><code>95bee00</code></a> fix: restore default ext watch behaviour</li>
<li><a href="https://github.com/remy/nodemon/commit/f219dccbf0ab9a48a3f84edb75d620e3a61a9f36"><code>f219dcc</code></a> test: Update release.yml to use ubuntu-latest (<a href="https://redirect.github.com/remy/nodemon/issues/2123">#2123</a>)</li>
<li><a href="https://github.com/remy/nodemon/commit/af3b9e237281beffd92ceee0e2411ef53edcf375"><code>af3b9e2</code></a> fix: node@10 support back in</li>
<li><a href="https://github.com/remy/nodemon/commit/a3f0e12bd9081cfb30131b536cd5fb914c9b2ded"><code>a3f0e12</code></a> test: package wasn't installing</li>
<li><a href="https://github.com/remy/nodemon/commit/8ded28cd4a4915a55366e8d1565958b9552ca4ea"><code>8ded28c</code></a> docs: update test runners and add TODO</li>
<li><a href="https://github.com/remy/nodemon/commit/83ef51d7b262b0e27050dadb5b4aba6aa4198ac6"><code>83ef51d</code></a> chore: website supporters</li>
<li><a href="https://github.com/remy/nodemon/commit/86d5f403a3e06e8aed48b37fa854730dc83257be"><code>86d5f40</code></a> fix: also watch cjs</li>
<li><a href="https://github.com/remy/nodemon/commit/7881f05d323f197b3662d68c030b64697d0dd5db"><code>7881f05</code></a> chore: remove legacy .nodemon support</li>
<li><a href="https://github.com/remy/nodemon/commit/04302b8e40bd5bc41f7f31de84aebb62312936c4"><code>04302b8</code></a> Merge branch 'Vindeep07-develop'</li>
<li>Additional commits viewable in <a href="https://github.com/remy/nodemon/compare/v2.0.20...v3.0.1">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-11 07:44:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/690" class=".btn">#690</a>
            </td>
            <td>
                <b>
                    Bump protobufjs from 7.2.2 to 7.2.4 in /hardhat/hedera
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [protobufjs](https://github.com/protobufjs/protobuf.js) from 7.2.2 to 7.2.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/protobufjs/protobuf.js/releases">protobufjs's releases</a>.</em></p>
<blockquote>
<h2>protobufjs: v7.2.4</h2>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.2.3...protobufjs-v7.2.4">7.2.4</a> (2023-06-23)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>do not let setProperty change the prototype (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1899">#1899</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/e66379f451b0393c27d87b37fa7d271619e16b0d">e66379f</a>)</li>
</ul>
<h2>protobufjs: v7.2.3</h2>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.2.2...protobufjs-v7.2.3">7.2.3</a> (2023-03-27)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>type names can be split into multiple tokens (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1877">#1877</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/8817ee613dfcf55f7f6fa8704f3fdd3e68c0e1d8">8817ee6</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/protobufjs/protobuf.js/blob/master/CHANGELOG.md">protobufjs's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.2.3...protobufjs-v7.2.4">7.2.4</a> (2023-06-23)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>do not let setProperty change the prototype (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1899">#1899</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/e66379f451b0393c27d87b37fa7d271619e16b0d">e66379f</a>)</li>
</ul>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.2.2...protobufjs-v7.2.3">7.2.3</a> (2023-03-27)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>type names can be split into multiple tokens (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1877">#1877</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/8817ee613dfcf55f7f6fa8704f3fdd3e68c0e1d8">8817ee6</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/42e5a9ca85044800b16e193020e1d4d2e6b4010c"><code>42e5a9c</code></a> chore: release master (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1900">#1900</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/e66379f451b0393c27d87b37fa7d271619e16b0d"><code>e66379f</code></a> fix: do not let setProperty change the prototype (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1899">#1899</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/56b1e64979dae757b67a21d326e16acee39f2267"><code>56b1e64</code></a> chore: release master (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1879">#1879</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/8817ee613dfcf55f7f6fa8704f3fdd3e68c0e1d8"><code>8817ee6</code></a> fix: type names can be split into multiple tokens (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1877">#1877</a>)</li>
<li>See full diff in <a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.2.2...protobufjs-v7.2.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=protobufjs&package-manager=npm_and_yarn&previous-version=7.2.2&new-version=7.2.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-08 01:14:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/689" class=".btn">#689</a>
            </td>
            <td>
                <b>
                    Bump @grpc/grpc-js from 1.7.0 to 1.8.17 in /fabric/chaincode/emissionscontract/typescript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@grpc/grpc-js](https://github.com/grpc/grpc-node) from 1.7.0 to 1.8.17.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-node/releases"><code>@​grpc/grpc-js</code>'s releases</a>.</em></p>
<blockquote>
<h2><code>@​grpc/grpc-js</code> 1.8.17</h2>
<ul>
<li>Disallow <code>pick_first</code> LB policy as the direct child of an <code>outlier_detection</code> LB policy (<a href="https://redirect.github.com/grpc/grpc-node/issues/2476">#2476</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.16</h2>
<ul>
<li>Fix missing <code>transport</code> trace logs (<a href="https://redirect.github.com/grpc/grpc-node/issues/2470">#2470</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.15</h2>
<ul>
<li>Fix a memory leak that could result from a specific pattern of recursive function calls (<a href="https://redirect.github.com/grpc/grpc-node/issues/2456">#2456</a>)</li>
<li>Ensure <code>status</code> and <code>error</code> events are consistently emitted asynchronously (<a href="https://redirect.github.com/grpc/grpc-node/issues/2456">#2456</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.14</h2>
<ul>
<li>Fix sequencing of some events related to connectivity state changes (<a href="https://redirect.github.com/grpc/grpc-node/issues/2421">#2421</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.13</h2>
<ul>
<li>Fix memory leak in channelz socket tracking (<a href="https://redirect.github.com/grpc/grpc-node/issues/2394">#2394</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code><a href="https://github.com/1"><code>@​1</code></a>.8.12</h2>
<ul>
<li>Fix an occasional type error when receiving DNS updates (<a href="https://redirect.github.com/grpc/grpc-node/issues/2380">#2380</a>)</li>
<li>Fix ordering of events when handing requests on the server (<a href="https://redirect.github.com/grpc/grpc-node/issues/2376">#2376</a> contributed by <a href="https://github.com/phoenix741"><code>@​phoenix741</code></a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.11</h2>
<ul>
<li>Avoid accumulating placeholder objects when sending many messages on a long-running stream (<a href="https://redirect.github.com/grpc/grpc-node/issues/2372">#2372</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.10</h2>
<ul>
<li>Fix bugs in &quot;pick first&quot; load balancing policy that caused incorrect reconnection behavior (<a href="https://redirect.github.com/grpc/grpc-node/issues/2369">#2369</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.9</h2>
<ul>
<li>Fix a bug where clients would continue to send pings at the original configured rate after receiving a backoff request from the server (<a href="https://redirect.github.com/grpc/grpc-node/issues/2363">#2363</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.8</h2>
<ul>
<li>Remove <code>progress</code> field in returned status object (<a href="https://redirect.github.com/grpc/grpc-node/issues/2350">#2350</a>)</li>
<li>Export <code>InterceptingListener</code> and <code>NextCall</code> types (<a href="https://redirect.github.com/grpc/grpc-node/issues/2351">#2351</a>)</li>
<li>Fix a bug that could cause a crash when sending messages that exceed the outgoing message buffer size while a retry is in progress (<a href="https://redirect.github.com/grpc/grpc-node/issues/2349">#2349</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.7</h2>
<ul>
<li>Make handling of HTTP2 session references work independent of keepalive settings (<a href="https://redirect.github.com/grpc/grpc-node/issues/2337">#2337</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.6</h2>
<ul>
<li>Hold a reference to transport from call to avoid premature garbage collection (<a href="https://redirect.github.com/grpc/grpc-node/issues/2336">#2336</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.5</h2>
<ul>
<li>Cancel deadline timer when the call ends (<a href="https://redirect.github.com/grpc/grpc-node/issues/2335">#2335</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code><a href="https://github.com/1"><code>@​1</code></a>.8.4</h2>
<ul>
<li>Fix a bug that would sometimes allow the Node process to exit even though a gRPC request is active (<a href="https://redirect.github.com/grpc/grpc-node/issues/2322">#2322</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.3</h2>
<ul>
<li>Fix bug that caused streams to fail early when receiving a GOAWAY (<a href="https://redirect.github.com/grpc/grpc-node/issues/2319">#2319</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code><a href="https://github.com/1"><code>@​1</code></a>.8.2</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-node/commit/409418b103f35c6b89371731e2b1d5084b442318"><code>409418b</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2476">#2476</a> from murgatroid99/grpc-js_prohibit_od_pick_first</li>
<li><a href="https://github.com/grpc/grpc-node/commit/ed70a0b381144b387698f2d57001f5a7bc82cbe9"><code>ed70a0b</code></a> Fix handling of OD policy with no child</li>
<li><a href="https://github.com/grpc/grpc-node/commit/073caf5b83387be8c1c7416477489646060e4942"><code>073caf5</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2478">#2478</a> from murgatroid99/grpc-js-xds_docker_distroless_1.8.x</li>
<li><a href="https://github.com/grpc/grpc-node/commit/d2d17b0b694d7c23e2448d9cde224b9427102fb4"><code>d2d17b0</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2482">#2482</a> from XuanWang-Amos/backport-1.8-file_multiple_url_map</li>
<li><a href="https://github.com/grpc/grpc-node/commit/a6aa7ea43e1458a578cf9ab81ed492a760c43a78"><code>a6aa7ea</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2475">#2475</a> from XuanWang-Amos/file_multiple_url_map</li>
<li><a href="https://github.com/grpc/grpc-node/commit/a62d2b027bf91e5084c9134305e88a645dc5f1c1"><code>a62d2b0</code></a> Use entrypoint /nodejs/bin/node</li>
<li><a href="https://github.com/grpc/grpc-node/commit/9441de78f655ada34ada0dc1a8057122eb21f229"><code>9441de7</code></a> grpc-js-xds: Use distroless Node image for interop Dockerfile</li>
<li><a href="https://github.com/grpc/grpc-node/commit/b53f5882f13a5cb3c599804e96304bf5b8407ea6"><code>b53f588</code></a> grpc-js: Disallow pick_first as child of outlier_detection</li>
<li><a href="https://github.com/grpc/grpc-node/commit/09d74ca43d2fcb63c97405315bd01633322d9b34"><code>09d74ca</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2470">#2470</a> from murgatroid99/grpc-js_transport_trace_fix</li>
<li><a href="https://github.com/grpc/grpc-node/commit/87b5466b1b5e6d269a9750305c5842c9e30e56e8"><code>87b5466</code></a> grpc-js: Implement trace function in Http2SubchannelConnector</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-node/compare/@grpc/grpc-js@1.7.0...@grpc/grpc-js@1.8.17">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@grpc/grpc-js&package-manager=npm_and_yarn&previous-version=1.7.0&new-version=1.8.17)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 23:26:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/688" class=".btn">#688</a>
            </td>
            <td>
                <b>
                    Bump @grpc/grpc-js from 1.6.8 to 1.8.17 in /fabric/docker-compose-setup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@grpc/grpc-js](https://github.com/grpc/grpc-node) from 1.6.8 to 1.8.17.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-node/releases"><code>@​grpc/grpc-js</code>'s releases</a>.</em></p>
<blockquote>
<h2><code>@​grpc/grpc-js</code> 1.8.17</h2>
<ul>
<li>Disallow <code>pick_first</code> LB policy as the direct child of an <code>outlier_detection</code> LB policy (<a href="https://redirect.github.com/grpc/grpc-node/issues/2476">#2476</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.16</h2>
<ul>
<li>Fix missing <code>transport</code> trace logs (<a href="https://redirect.github.com/grpc/grpc-node/issues/2470">#2470</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.15</h2>
<ul>
<li>Fix a memory leak that could result from a specific pattern of recursive function calls (<a href="https://redirect.github.com/grpc/grpc-node/issues/2456">#2456</a>)</li>
<li>Ensure <code>status</code> and <code>error</code> events are consistently emitted asynchronously (<a href="https://redirect.github.com/grpc/grpc-node/issues/2456">#2456</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.14</h2>
<ul>
<li>Fix sequencing of some events related to connectivity state changes (<a href="https://redirect.github.com/grpc/grpc-node/issues/2421">#2421</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.13</h2>
<ul>
<li>Fix memory leak in channelz socket tracking (<a href="https://redirect.github.com/grpc/grpc-node/issues/2394">#2394</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code><a href="https://github.com/1"><code>@​1</code></a>.8.12</h2>
<ul>
<li>Fix an occasional type error when receiving DNS updates (<a href="https://redirect.github.com/grpc/grpc-node/issues/2380">#2380</a>)</li>
<li>Fix ordering of events when handing requests on the server (<a href="https://redirect.github.com/grpc/grpc-node/issues/2376">#2376</a> contributed by <a href="https://github.com/phoenix741"><code>@​phoenix741</code></a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.11</h2>
<ul>
<li>Avoid accumulating placeholder objects when sending many messages on a long-running stream (<a href="https://redirect.github.com/grpc/grpc-node/issues/2372">#2372</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.10</h2>
<ul>
<li>Fix bugs in &quot;pick first&quot; load balancing policy that caused incorrect reconnection behavior (<a href="https://redirect.github.com/grpc/grpc-node/issues/2369">#2369</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.9</h2>
<ul>
<li>Fix a bug where clients would continue to send pings at the original configured rate after receiving a backoff request from the server (<a href="https://redirect.github.com/grpc/grpc-node/issues/2363">#2363</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.8</h2>
<ul>
<li>Remove <code>progress</code> field in returned status object (<a href="https://redirect.github.com/grpc/grpc-node/issues/2350">#2350</a>)</li>
<li>Export <code>InterceptingListener</code> and <code>NextCall</code> types (<a href="https://redirect.github.com/grpc/grpc-node/issues/2351">#2351</a>)</li>
<li>Fix a bug that could cause a crash when sending messages that exceed the outgoing message buffer size while a retry is in progress (<a href="https://redirect.github.com/grpc/grpc-node/issues/2349">#2349</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.7</h2>
<ul>
<li>Make handling of HTTP2 session references work independent of keepalive settings (<a href="https://redirect.github.com/grpc/grpc-node/issues/2337">#2337</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.6</h2>
<ul>
<li>Hold a reference to transport from call to avoid premature garbage collection (<a href="https://redirect.github.com/grpc/grpc-node/issues/2336">#2336</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.5</h2>
<ul>
<li>Cancel deadline timer when the call ends (<a href="https://redirect.github.com/grpc/grpc-node/issues/2335">#2335</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code><a href="https://github.com/1"><code>@​1</code></a>.8.4</h2>
<ul>
<li>Fix a bug that would sometimes allow the Node process to exit even though a gRPC request is active (<a href="https://redirect.github.com/grpc/grpc-node/issues/2322">#2322</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.3</h2>
<ul>
<li>Fix bug that caused streams to fail early when receiving a GOAWAY (<a href="https://redirect.github.com/grpc/grpc-node/issues/2319">#2319</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code><a href="https://github.com/1"><code>@​1</code></a>.8.2</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/grpc/grpc-node/commits/@grpc/grpc-js@1.8.17">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@grpc/grpc-js&package-manager=npm_and_yarn&previous-version=1.6.8&new-version=1.8.17)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 23:22:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/687" class=".btn">#687</a>
            </td>
            <td>
                <b>
                    Bump @grpc/grpc-js from 1.6.7 to 1.8.17
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@grpc/grpc-js](https://github.com/grpc/grpc-node) from 1.6.7 to 1.8.17.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-node/releases"><code>@​grpc/grpc-js</code>'s releases</a>.</em></p>
<blockquote>
<h2><code>@​grpc/grpc-js</code> 1.8.17</h2>
<ul>
<li>Disallow <code>pick_first</code> LB policy as the direct child of an <code>outlier_detection</code> LB policy (<a href="https://redirect.github.com/grpc/grpc-node/issues/2476">#2476</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.16</h2>
<ul>
<li>Fix missing <code>transport</code> trace logs (<a href="https://redirect.github.com/grpc/grpc-node/issues/2470">#2470</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.15</h2>
<ul>
<li>Fix a memory leak that could result from a specific pattern of recursive function calls (<a href="https://redirect.github.com/grpc/grpc-node/issues/2456">#2456</a>)</li>
<li>Ensure <code>status</code> and <code>error</code> events are consistently emitted asynchronously (<a href="https://redirect.github.com/grpc/grpc-node/issues/2456">#2456</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.14</h2>
<ul>
<li>Fix sequencing of some events related to connectivity state changes (<a href="https://redirect.github.com/grpc/grpc-node/issues/2421">#2421</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.13</h2>
<ul>
<li>Fix memory leak in channelz socket tracking (<a href="https://redirect.github.com/grpc/grpc-node/issues/2394">#2394</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code><a href="https://github.com/1"><code>@​1</code></a>.8.12</h2>
<ul>
<li>Fix an occasional type error when receiving DNS updates (<a href="https://redirect.github.com/grpc/grpc-node/issues/2380">#2380</a>)</li>
<li>Fix ordering of events when handing requests on the server (<a href="https://redirect.github.com/grpc/grpc-node/issues/2376">#2376</a> contributed by <a href="https://github.com/phoenix741"><code>@​phoenix741</code></a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.11</h2>
<ul>
<li>Avoid accumulating placeholder objects when sending many messages on a long-running stream (<a href="https://redirect.github.com/grpc/grpc-node/issues/2372">#2372</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.10</h2>
<ul>
<li>Fix bugs in &quot;pick first&quot; load balancing policy that caused incorrect reconnection behavior (<a href="https://redirect.github.com/grpc/grpc-node/issues/2369">#2369</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.9</h2>
<ul>
<li>Fix a bug where clients would continue to send pings at the original configured rate after receiving a backoff request from the server (<a href="https://redirect.github.com/grpc/grpc-node/issues/2363">#2363</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.8</h2>
<ul>
<li>Remove <code>progress</code> field in returned status object (<a href="https://redirect.github.com/grpc/grpc-node/issues/2350">#2350</a>)</li>
<li>Export <code>InterceptingListener</code> and <code>NextCall</code> types (<a href="https://redirect.github.com/grpc/grpc-node/issues/2351">#2351</a>)</li>
<li>Fix a bug that could cause a crash when sending messages that exceed the outgoing message buffer size while a retry is in progress (<a href="https://redirect.github.com/grpc/grpc-node/issues/2349">#2349</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.7</h2>
<ul>
<li>Make handling of HTTP2 session references work independent of keepalive settings (<a href="https://redirect.github.com/grpc/grpc-node/issues/2337">#2337</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.6</h2>
<ul>
<li>Hold a reference to transport from call to avoid premature garbage collection (<a href="https://redirect.github.com/grpc/grpc-node/issues/2336">#2336</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.5</h2>
<ul>
<li>Cancel deadline timer when the call ends (<a href="https://redirect.github.com/grpc/grpc-node/issues/2335">#2335</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code><a href="https://github.com/1"><code>@​1</code></a>.8.4</h2>
<ul>
<li>Fix a bug that would sometimes allow the Node process to exit even though a gRPC request is active (<a href="https://redirect.github.com/grpc/grpc-node/issues/2322">#2322</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.3</h2>
<ul>
<li>Fix bug that caused streams to fail early when receiving a GOAWAY (<a href="https://redirect.github.com/grpc/grpc-node/issues/2319">#2319</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code><a href="https://github.com/1"><code>@​1</code></a>.8.2</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-node/commit/409418b103f35c6b89371731e2b1d5084b442318"><code>409418b</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2476">#2476</a> from murgatroid99/grpc-js_prohibit_od_pick_first</li>
<li><a href="https://github.com/grpc/grpc-node/commit/ed70a0b381144b387698f2d57001f5a7bc82cbe9"><code>ed70a0b</code></a> Fix handling of OD policy with no child</li>
<li><a href="https://github.com/grpc/grpc-node/commit/073caf5b83387be8c1c7416477489646060e4942"><code>073caf5</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2478">#2478</a> from murgatroid99/grpc-js-xds_docker_distroless_1.8.x</li>
<li><a href="https://github.com/grpc/grpc-node/commit/d2d17b0b694d7c23e2448d9cde224b9427102fb4"><code>d2d17b0</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2482">#2482</a> from XuanWang-Amos/backport-1.8-file_multiple_url_map</li>
<li><a href="https://github.com/grpc/grpc-node/commit/a6aa7ea43e1458a578cf9ab81ed492a760c43a78"><code>a6aa7ea</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2475">#2475</a> from XuanWang-Amos/file_multiple_url_map</li>
<li><a href="https://github.com/grpc/grpc-node/commit/a62d2b027bf91e5084c9134305e88a645dc5f1c1"><code>a62d2b0</code></a> Use entrypoint /nodejs/bin/node</li>
<li><a href="https://github.com/grpc/grpc-node/commit/9441de78f655ada34ada0dc1a8057122eb21f229"><code>9441de7</code></a> grpc-js-xds: Use distroless Node image for interop Dockerfile</li>
<li><a href="https://github.com/grpc/grpc-node/commit/b53f5882f13a5cb3c599804e96304bf5b8407ea6"><code>b53f588</code></a> grpc-js: Disallow pick_first as child of outlier_detection</li>
<li><a href="https://github.com/grpc/grpc-node/commit/09d74ca43d2fcb63c97405315bd01633322d9b34"><code>09d74ca</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2470">#2470</a> from murgatroid99/grpc-js_transport_trace_fix</li>
<li><a href="https://github.com/grpc/grpc-node/commit/87b5466b1b5e6d269a9750305c5842c9e30e56e8"><code>87b5466</code></a> grpc-js: Implement trace function in Http2SubchannelConnector</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-node/compare/@grpc/grpc-js@1.6.7...@grpc/grpc-js@1.8.17">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@grpc/grpc-js&package-manager=npm_and_yarn&previous-version=1.6.7&new-version=1.8.17)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 23:02:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/686" class=".btn">#686</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.46.0 to 1.53.0 in /fabric/multi-cloud-deployment/chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.46.0 to 1.53.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
<h2>Release 1.53.0</h2>
<h1>API Changes</h1>
<ul>
<li>balancer: support injection of per-call metadata from LB policies (<a href="https://redirect.github.com/grpc/grpc-go/issues/5853">#5853</a>)</li>
<li>resolver: remove deprecated field <code>resolver.Target.Endpoint</code> and replace with <code>resolver.Target.Endpoint()</code> (<a href="https://redirect.github.com/grpc/grpc-go/issues/5852">#5852</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/kylejb"><code>@​kylejb</code></a></li>
</ul>
</li>
</ul>
<h1>New Features</h1>
<ul>
<li>xds/ringhash: introduce <code>GRPC_RING_HASH_CAP</code> environment variable to override the maximum ring size. (<a href="https://redirect.github.com/grpc/grpc-go/issues/5884">#5884</a>)</li>
<li>rls: propagate headers received in RLS response to backends (<a href="https://redirect.github.com/grpc/grpc-go/issues/5883">#5883</a>)</li>
</ul>
<h1>Bug Fixes</h1>
<ul>
<li>transport: drain client transport when streamID approaches MaxStreamID (<a href="https://redirect.github.com/grpc/grpc-go/issues/5889">#5889</a>)</li>
<li>server: after GracefulStop, ensure connections are closed when final RPC completes (<a href="https://redirect.github.com/grpc/grpc-go/issues/5968">#5968</a>)</li>
<li>server: fix a few issues where grpc server uses RST_STREAM for non-HTTP/2 errors (<a href="https://redirect.github.com/grpc/grpc-go/issues/5893">#5893</a>)</li>
<li>xdsclient: fix race which can happen when multiple load reporting calls are made at the same time. (<a href="https://redirect.github.com/grpc/grpc-go/issues/5927">#5927</a>)</li>
<li>rls: fix a data race involving the LRU cache (<a href="https://redirect.github.com/grpc/grpc-go/issues/5925">#5925</a>)</li>
<li>xds: fix panic involving double close of channel in xDS transport (<a href="https://redirect.github.com/grpc/grpc-go/issues/5959">#5959</a>)</li>
<li>gcp/observability: update method name validation (<a href="https://redirect.github.com/grpc/grpc-go/issues/5951">#5951</a>)</li>
</ul>
<h1>Documentation</h1>
<ul>
<li>credentials/oauth: mark <code>NewOauthAccess</code> as deprecated (<a href="https://redirect.github.com/grpc/grpc-go/issues/5882">#5882</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/buzzsurfr"><code>@​buzzsurfr</code></a></li>
</ul>
</li>
</ul>
<h2>Release 1.52.3</h2>
<h1>Bug Fixes</h1>
<ul>
<li>Fix user-agent version</li>
</ul>
<h2>Release 1.52.2</h2>
<h1>Bug Fixes</h1>
<ul>
<li>xds: fix panic involving double close of channel in xDS transport (<a href="https://redirect.github.com/grpc/grpc-go/issues/5959">#5959</a>)</li>
</ul>
<h2>Release 1.52.1</h2>
<h1>Bug Fixes</h1>
<ul>
<li>grpclb: rename grpclbstate package back to state (<a href="https://redirect.github.com/grpc/grpc-go/issues/5963">#5963</a>)</li>
</ul>
<h2>Release 1.52.0</h2>
<h1>New Features</h1>
<ul>
<li>xdsclient: log node ID with verbosity INFO (<a href="https://redirect.github.com/grpc/grpc-go/issues/5860">#5860</a>)</li>
<li>ringhash: impose cap on <code>max_ring_size</code> to reduce possibility of OOMs (<a href="https://redirect.github.com/grpc/grpc-go/issues/5801">#5801</a>)</li>
</ul>
<h1>Behavior Changes</h1>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/dba26e15a07f43875ccf806a2dd6cbcbc1c12eab"><code>dba26e1</code></a> Change version to 1.53.0 (<a href="https://redirect.github.com/grpc/grpc-go/issues/5983">#5983</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/2a1e9348ff7b5d9f4b5039e84e6c9873b5b3e26e"><code>2a1e934</code></a> server: after GracefulStop, ensure connections are closed when final RPC comp...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/e2d69aa076dd070e3668784c4dc8bcf7131b3f67"><code>e2d69aa</code></a> tests: fix spelling of variable (<a href="https://redirect.github.com/grpc/grpc-go/issues/5966">#5966</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/a6376c9893f56fc3819bee9ef5d71f55cc2d38dd"><code>a6376c9</code></a> xds/resolver: cleanup tests to use real xDS client 3/n (<a href="https://redirect.github.com/grpc/grpc-go/issues/5953">#5953</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/bf8fc46fa6eb913e4ed0f6dee6c6a7b75e85fbf0"><code>bf8fc46</code></a> xds/resolver: cleanup tests to use real xDS client 5/n (<a href="https://redirect.github.com/grpc/grpc-go/issues/5955">#5955</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/3930549b38c0fc4cd94a95efccf7cef5f90515fd"><code>3930549</code></a> resolver: replace resolver.Target.Endpoint field with Endpoint() method (<a href="https://redirect.github.com/grpc/grpc-go/issues/5852">#5852</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/894816c487f8dd48fc971c45a7c5baa4b86ef7de"><code>894816c</code></a> grpclb: rename <code>grpclbstate</code> package back to <code>state</code> (<a href="https://redirect.github.com/grpc/grpc-go/issues/5962">#5962</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/e5a0237a46a5f95fa571624929be10c7afebb180"><code>e5a0237</code></a> encoding: fix duplicate compressor names (<a href="https://redirect.github.com/grpc/grpc-go/issues/5958">#5958</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/4adb2a7a00d8b62df5ea34d520fe3ca13bffd31a"><code>4adb2a7</code></a> xds/resolver: cleanup tests to use real xDS client 2/n (<a href="https://redirect.github.com/grpc/grpc-go/issues/5952">#5952</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/52a8392f374b8cd60e176b67925a7f8c1605d014"><code>52a8392</code></a> gcp/observability: update method name validation (<a href="https://redirect.github.com/grpc/grpc-go/issues/5951">#5951</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-go/compare/v1.46.0...v1.53.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.46.0&new-version=1.53.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 21:20:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/685" class=".btn">#685</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.46.0 to 1.53.0 in /fabric/chaincode/datalock
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.46.0 to 1.53.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
<h2>Release 1.53.0</h2>
<h1>API Changes</h1>
<ul>
<li>balancer: support injection of per-call metadata from LB policies (<a href="https://redirect.github.com/grpc/grpc-go/issues/5853">#5853</a>)</li>
<li>resolver: remove deprecated field <code>resolver.Target.Endpoint</code> and replace with <code>resolver.Target.Endpoint()</code> (<a href="https://redirect.github.com/grpc/grpc-go/issues/5852">#5852</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/kylejb"><code>@​kylejb</code></a></li>
</ul>
</li>
</ul>
<h1>New Features</h1>
<ul>
<li>xds/ringhash: introduce <code>GRPC_RING_HASH_CAP</code> environment variable to override the maximum ring size. (<a href="https://redirect.github.com/grpc/grpc-go/issues/5884">#5884</a>)</li>
<li>rls: propagate headers received in RLS response to backends (<a href="https://redirect.github.com/grpc/grpc-go/issues/5883">#5883</a>)</li>
</ul>
<h1>Bug Fixes</h1>
<ul>
<li>transport: drain client transport when streamID approaches MaxStreamID (<a href="https://redirect.github.com/grpc/grpc-go/issues/5889">#5889</a>)</li>
<li>server: after GracefulStop, ensure connections are closed when final RPC completes (<a href="https://redirect.github.com/grpc/grpc-go/issues/5968">#5968</a>)</li>
<li>server: fix a few issues where grpc server uses RST_STREAM for non-HTTP/2 errors (<a href="https://redirect.github.com/grpc/grpc-go/issues/5893">#5893</a>)</li>
<li>xdsclient: fix race which can happen when multiple load reporting calls are made at the same time. (<a href="https://redirect.github.com/grpc/grpc-go/issues/5927">#5927</a>)</li>
<li>rls: fix a data race involving the LRU cache (<a href="https://redirect.github.com/grpc/grpc-go/issues/5925">#5925</a>)</li>
<li>xds: fix panic involving double close of channel in xDS transport (<a href="https://redirect.github.com/grpc/grpc-go/issues/5959">#5959</a>)</li>
<li>gcp/observability: update method name validation (<a href="https://redirect.github.com/grpc/grpc-go/issues/5951">#5951</a>)</li>
</ul>
<h1>Documentation</h1>
<ul>
<li>credentials/oauth: mark <code>NewOauthAccess</code> as deprecated (<a href="https://redirect.github.com/grpc/grpc-go/issues/5882">#5882</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/buzzsurfr"><code>@​buzzsurfr</code></a></li>
</ul>
</li>
</ul>
<h2>Release 1.52.3</h2>
<h1>Bug Fixes</h1>
<ul>
<li>Fix user-agent version</li>
</ul>
<h2>Release 1.52.2</h2>
<h1>Bug Fixes</h1>
<ul>
<li>xds: fix panic involving double close of channel in xDS transport (<a href="https://redirect.github.com/grpc/grpc-go/issues/5959">#5959</a>)</li>
</ul>
<h2>Release 1.52.1</h2>
<h1>Bug Fixes</h1>
<ul>
<li>grpclb: rename grpclbstate package back to state (<a href="https://redirect.github.com/grpc/grpc-go/issues/5963">#5963</a>)</li>
</ul>
<h2>Release 1.52.0</h2>
<h1>New Features</h1>
<ul>
<li>xdsclient: log node ID with verbosity INFO (<a href="https://redirect.github.com/grpc/grpc-go/issues/5860">#5860</a>)</li>
<li>ringhash: impose cap on <code>max_ring_size</code> to reduce possibility of OOMs (<a href="https://redirect.github.com/grpc/grpc-go/issues/5801">#5801</a>)</li>
</ul>
<h1>Behavior Changes</h1>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/dba26e15a07f43875ccf806a2dd6cbcbc1c12eab"><code>dba26e1</code></a> Change version to 1.53.0 (<a href="https://redirect.github.com/grpc/grpc-go/issues/5983">#5983</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/2a1e9348ff7b5d9f4b5039e84e6c9873b5b3e26e"><code>2a1e934</code></a> server: after GracefulStop, ensure connections are closed when final RPC comp...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/e2d69aa076dd070e3668784c4dc8bcf7131b3f67"><code>e2d69aa</code></a> tests: fix spelling of variable (<a href="https://redirect.github.com/grpc/grpc-go/issues/5966">#5966</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/a6376c9893f56fc3819bee9ef5d71f55cc2d38dd"><code>a6376c9</code></a> xds/resolver: cleanup tests to use real xDS client 3/n (<a href="https://redirect.github.com/grpc/grpc-go/issues/5953">#5953</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/bf8fc46fa6eb913e4ed0f6dee6c6a7b75e85fbf0"><code>bf8fc46</code></a> xds/resolver: cleanup tests to use real xDS client 5/n (<a href="https://redirect.github.com/grpc/grpc-go/issues/5955">#5955</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/3930549b38c0fc4cd94a95efccf7cef5f90515fd"><code>3930549</code></a> resolver: replace resolver.Target.Endpoint field with Endpoint() method (<a href="https://redirect.github.com/grpc/grpc-go/issues/5852">#5852</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/894816c487f8dd48fc971c45a7c5baa4b86ef7de"><code>894816c</code></a> grpclb: rename <code>grpclbstate</code> package back to <code>state</code> (<a href="https://redirect.github.com/grpc/grpc-go/issues/5962">#5962</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/e5a0237a46a5f95fa571624929be10c7afebb180"><code>e5a0237</code></a> encoding: fix duplicate compressor names (<a href="https://redirect.github.com/grpc/grpc-go/issues/5958">#5958</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/4adb2a7a00d8b62df5ea34d520fe3ca13bffd31a"><code>4adb2a7</code></a> xds/resolver: cleanup tests to use real xDS client 2/n (<a href="https://redirect.github.com/grpc/grpc-go/issues/5952">#5952</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/52a8392f374b8cd60e176b67925a7f8c1605d014"><code>52a8392</code></a> gcp/observability: update method name validation (<a href="https://redirect.github.com/grpc/grpc-go/issues/5951">#5951</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-go/compare/v1.46.0...v1.53.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.46.0&new-version=1.53.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 21:19:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/684" class=".btn">#684</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.46.0 to 1.53.0 in /fabric/multi-cloud-deployment/deploy-aws/chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.46.0 to 1.53.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
<h2>Release 1.53.0</h2>
<h1>API Changes</h1>
<ul>
<li>balancer: support injection of per-call metadata from LB policies (<a href="https://redirect.github.com/grpc/grpc-go/issues/5853">#5853</a>)</li>
<li>resolver: remove deprecated field <code>resolver.Target.Endpoint</code> and replace with <code>resolver.Target.Endpoint()</code> (<a href="https://redirect.github.com/grpc/grpc-go/issues/5852">#5852</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/kylejb"><code>@​kylejb</code></a></li>
</ul>
</li>
</ul>
<h1>New Features</h1>
<ul>
<li>xds/ringhash: introduce <code>GRPC_RING_HASH_CAP</code> environment variable to override the maximum ring size. (<a href="https://redirect.github.com/grpc/grpc-go/issues/5884">#5884</a>)</li>
<li>rls: propagate headers received in RLS response to backends (<a href="https://redirect.github.com/grpc/grpc-go/issues/5883">#5883</a>)</li>
</ul>
<h1>Bug Fixes</h1>
<ul>
<li>transport: drain client transport when streamID approaches MaxStreamID (<a href="https://redirect.github.com/grpc/grpc-go/issues/5889">#5889</a>)</li>
<li>server: after GracefulStop, ensure connections are closed when final RPC completes (<a href="https://redirect.github.com/grpc/grpc-go/issues/5968">#5968</a>)</li>
<li>server: fix a few issues where grpc server uses RST_STREAM for non-HTTP/2 errors (<a href="https://redirect.github.com/grpc/grpc-go/issues/5893">#5893</a>)</li>
<li>xdsclient: fix race which can happen when multiple load reporting calls are made at the same time. (<a href="https://redirect.github.com/grpc/grpc-go/issues/5927">#5927</a>)</li>
<li>rls: fix a data race involving the LRU cache (<a href="https://redirect.github.com/grpc/grpc-go/issues/5925">#5925</a>)</li>
<li>xds: fix panic involving double close of channel in xDS transport (<a href="https://redirect.github.com/grpc/grpc-go/issues/5959">#5959</a>)</li>
<li>gcp/observability: update method name validation (<a href="https://redirect.github.com/grpc/grpc-go/issues/5951">#5951</a>)</li>
</ul>
<h1>Documentation</h1>
<ul>
<li>credentials/oauth: mark <code>NewOauthAccess</code> as deprecated (<a href="https://redirect.github.com/grpc/grpc-go/issues/5882">#5882</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/buzzsurfr"><code>@​buzzsurfr</code></a></li>
</ul>
</li>
</ul>
<h2>Release 1.52.3</h2>
<h1>Bug Fixes</h1>
<ul>
<li>Fix user-agent version</li>
</ul>
<h2>Release 1.52.2</h2>
<h1>Bug Fixes</h1>
<ul>
<li>xds: fix panic involving double close of channel in xDS transport (<a href="https://redirect.github.com/grpc/grpc-go/issues/5959">#5959</a>)</li>
</ul>
<h2>Release 1.52.1</h2>
<h1>Bug Fixes</h1>
<ul>
<li>grpclb: rename grpclbstate package back to state (<a href="https://redirect.github.com/grpc/grpc-go/issues/5963">#5963</a>)</li>
</ul>
<h2>Release 1.52.0</h2>
<h1>New Features</h1>
<ul>
<li>xdsclient: log node ID with verbosity INFO (<a href="https://redirect.github.com/grpc/grpc-go/issues/5860">#5860</a>)</li>
<li>ringhash: impose cap on <code>max_ring_size</code> to reduce possibility of OOMs (<a href="https://redirect.github.com/grpc/grpc-go/issues/5801">#5801</a>)</li>
</ul>
<h1>Behavior Changes</h1>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/dba26e15a07f43875ccf806a2dd6cbcbc1c12eab"><code>dba26e1</code></a> Change version to 1.53.0 (<a href="https://redirect.github.com/grpc/grpc-go/issues/5983">#5983</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/2a1e9348ff7b5d9f4b5039e84e6c9873b5b3e26e"><code>2a1e934</code></a> server: after GracefulStop, ensure connections are closed when final RPC comp...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/e2d69aa076dd070e3668784c4dc8bcf7131b3f67"><code>e2d69aa</code></a> tests: fix spelling of variable (<a href="https://redirect.github.com/grpc/grpc-go/issues/5966">#5966</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/a6376c9893f56fc3819bee9ef5d71f55cc2d38dd"><code>a6376c9</code></a> xds/resolver: cleanup tests to use real xDS client 3/n (<a href="https://redirect.github.com/grpc/grpc-go/issues/5953">#5953</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/bf8fc46fa6eb913e4ed0f6dee6c6a7b75e85fbf0"><code>bf8fc46</code></a> xds/resolver: cleanup tests to use real xDS client 5/n (<a href="https://redirect.github.com/grpc/grpc-go/issues/5955">#5955</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/3930549b38c0fc4cd94a95efccf7cef5f90515fd"><code>3930549</code></a> resolver: replace resolver.Target.Endpoint field with Endpoint() method (<a href="https://redirect.github.com/grpc/grpc-go/issues/5852">#5852</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/894816c487f8dd48fc971c45a7c5baa4b86ef7de"><code>894816c</code></a> grpclb: rename <code>grpclbstate</code> package back to <code>state</code> (<a href="https://redirect.github.com/grpc/grpc-go/issues/5962">#5962</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/e5a0237a46a5f95fa571624929be10c7afebb180"><code>e5a0237</code></a> encoding: fix duplicate compressor names (<a href="https://redirect.github.com/grpc/grpc-go/issues/5958">#5958</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/4adb2a7a00d8b62df5ea34d520fe3ca13bffd31a"><code>4adb2a7</code></a> xds/resolver: cleanup tests to use real xDS client 2/n (<a href="https://redirect.github.com/grpc/grpc-go/issues/5952">#5952</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/52a8392f374b8cd60e176b67925a7f8c1605d014"><code>52a8392</code></a> gcp/observability: update method name validation (<a href="https://redirect.github.com/grpc/grpc-go/issues/5951">#5951</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-go/compare/v1.46.0...v1.53.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.46.0&new-version=1.53.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 21:19:19 +0000 UTC
    </div>
</div>

