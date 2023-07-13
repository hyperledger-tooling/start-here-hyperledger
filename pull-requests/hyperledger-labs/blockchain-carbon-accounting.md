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

