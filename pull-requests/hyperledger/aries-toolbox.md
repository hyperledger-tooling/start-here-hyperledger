---
layout: default
title: aries-toolbox
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-toolbox
---

# aries-toolbox <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-toolbox){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-toolbox/pull/318" class=".btn">#318</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump glob-parent and webpack-dev-server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [glob-parent](https://github.com/gulpjs/glob-parent) to 5.1.2 and updates ancestor dependency [webpack-dev-server](https://github.com/webpack/webpack-dev-server). These dependencies need to be updated together.

Updates `glob-parent` from 3.1.0 to 5.1.2
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/gulpjs/glob-parent/releases">glob-parent's releases</a>.</em></p>
<blockquote>
<h2>v5.1.2</h2>
<h3>Bug Fixes</h3>
<ul>
<li>eliminate ReDoS (<a href="https://redirect.github.com/gulpjs/glob-parent/issues/36">#36</a>) (<a href="https://github.com/gulpjs/glob-parent/commit/f9231168b0041fea3f8f954b3cceb56269fc6366">f923116</a>)</li>
</ul>
<h2>v5.1.1</h2>
<h3>Bug Fixes</h3>
<ul>
<li>unescape exclamation mark (<a href="https://redirect.github.com/gulpjs/glob-parent/issues/26">#26</a>) (<a href="https://github.com/gulpjs/glob-parent/commit/a98874f1a59e407f4fb1beb0db4efa8392da60bb">a98874f</a>)</li>
</ul>
<h2>v5.1.0</h2>
<h3>Features</h3>
<ul>
<li>add <code>flipBackslashes</code> option to disable auto conversion of slashes (closes <a href="https://redirect.github.com/gulpjs/glob-parent/issues/24">#24</a>) (<a href="https://redirect.github.com/gulpjs/glob-parent/issues/25">#25</a>) (<a href="https://github.com/gulpjs/glob-parent/commit/eecf91d5e3834ed78aee39c4eaaae654d76b87b3">eecf91d</a>)</li>
</ul>
<h2>v5.0.0</h2>
<h3>⚠ BREAKING CHANGES</h3>
<ul>
<li>Drop support for node &lt;6 &amp; bump dependencies</li>
</ul>
<h3>Miscellaneous Chores</h3>
<ul>
<li>Drop support for node &lt;6 &amp; bump dependencies (<a href="https://github.com/gulpjs/glob-parent/commit/896c0c00b4e7362f60b96e7fc295ae929245255a">896c0c0</a>)</li>
</ul>
<h2>v4.0.0</h2>
<h3>⚠ BREAKING CHANGES</h3>
<ul>
<li>question marks are valid path characters on Windows so avoid flagging as a glob when alone</li>
<li>Update is-glob dependency</li>
</ul>
<h3>Features</h3>
<ul>
<li>hoist regexps and strings for performance gains (<a href="https://github.com/gulpjs/glob-parent/commit/4a80667c69355c76a572a5892b0f133c8e1f457e">4a80667</a>)</li>
<li>question marks are valid path characters on Windows so avoid flagging as a glob when alone (<a href="https://github.com/gulpjs/glob-parent/commit/2a551dd0dc3235e78bf3c94843d4107072d17841">2a551dd</a>)</li>
<li>Update is-glob dependency (<a href="https://github.com/gulpjs/glob-parent/commit/e41fcd895d1f7bc617dba45c9d935a7949b9c281">e41fcd8</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/gulpjs/glob-parent/blob/main/CHANGELOG.md">glob-parent's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/gulpjs/glob-parent/compare/v5.1.1...v5.1.2">5.1.2</a> (2021-03-06)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>eliminate ReDoS (<a href="https://redirect.github.com/gulpjs/glob-parent/issues/36">#36</a>) (<a href="https://github.com/gulpjs/glob-parent/commit/f9231168b0041fea3f8f954b3cceb56269fc6366">f923116</a>)</li>
</ul>
<h3><a href="https://www.github.com/gulpjs/glob-parent/compare/v6.0.1...v6.0.2">6.0.2</a> (2021-09-29)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>Improve performance (<a href="https://redirect.github.com/gulpjs/glob-parent/issues/53">#53</a>) (<a href="https://www.github.com/gulpjs/glob-parent/commit/843f8de1c177e9a5c06c4cfd2349ca5207168e00">843f8de</a>)</li>
</ul>
<h3><a href="https://www.github.com/gulpjs/glob-parent/compare/v6.0.0...v6.0.1">6.0.1</a> (2021-07-20)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>Resolve ReDoS vulnerability from CVE-2021-35065 (<a href="https://redirect.github.com/gulpjs/glob-parent/issues/49">#49</a>) (<a href="https://www.github.com/gulpjs/glob-parent/commit/3e9f04a3b4349db7e1962d87c9a7398cda51f339">3e9f04a</a>)</li>
</ul>
<h2><a href="https://www.github.com/gulpjs/glob-parent/compare/v5.1.2...v6.0.0">6.0.0</a> (2021-05-03)</h2>
<h3>⚠ BREAKING CHANGES</h3>
<ul>
<li>Correct mishandled escaped path separators (<a href="https://redirect.github.com/gulpjs/glob-parent/issues/34">#34</a>)</li>
<li>upgrade scaffold, dropping node &lt;10 support</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>Correct mishandled escaped path separators (<a href="https://redirect.github.com/gulpjs/glob-parent/issues/34">#34</a>) (<a href="https://www.github.com/gulpjs/glob-parent/commit/32f6d52663b7addac38d0dff570d8127edf03f47">32f6d52</a>), closes <a href="https://redirect.github.com/gulpjs/glob-parent/issues/32">#32</a></li>
</ul>
<h3>Miscellaneous Chores</h3>
<ul>
<li>upgrade scaffold, dropping node &lt;10 support (<a href="https://www.github.com/gulpjs/glob-parent/commit/e83d0c5a411947cf69eb58f36349db80439c606f">e83d0c5</a>)</li>
</ul>
<h3><a href="https://github.com/gulpjs/glob-parent/compare/v5.1.0...v5.1.1">5.1.1</a> (2021-01-27)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>unescape exclamation mark (<a href="https://redirect.github.com/gulpjs/glob-parent/issues/26">#26</a>) (<a href="https://github.com/gulpjs/glob-parent/commit/a98874f1a59e407f4fb1beb0db4efa8392da60bb">a98874f</a>)</li>
</ul>
<h2><a href="https://github.com/gulpjs/glob-parent/compare/v5.0.0...v5.1.0">5.1.0</a> (2021-01-27)</h2>
<h3>Features</h3>
<ul>
<li>add <code>flipBackslashes</code> option to disable auto conversion of slashes (closes <a href="https://redirect.github.com/gulpjs/glob-parent/issues/24">#24</a>) (<a href="https://redirect.github.com/gulpjs/glob-parent/issues/25">#25</a>) (<a href="https://github.com/gulpjs/glob-parent/commit/eecf91d5e3834ed78aee39c4eaaae654d76b87b3">eecf91d</a>)</li>
</ul>
<h2><a href="https://github.com/gulpjs/glob-parent/compare/v4.0.0...v5.0.0">5.0.0</a> (2021-01-27)</h2>
<h3>⚠ BREAKING CHANGES</h3>
<ul>
<li>Drop support for node &lt;6 &amp; bump dependencies</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/gulpjs/glob-parent/commit/eb2c439de448c779b450472e591a2bc9e37e9668"><code>eb2c439</code></a> chore: update changelog</li>
<li><a href="https://github.com/gulpjs/glob-parent/commit/12bcb6c45c942e2d05fc1e6ff5402e72555b54b6"><code>12bcb6c</code></a> chore: release 5.1.2</li>
<li><a href="https://github.com/gulpjs/glob-parent/commit/f9231168b0041fea3f8f954b3cceb56269fc6366"><code>f923116</code></a> fix: eliminate ReDoS (<a href="https://redirect.github.com/gulpjs/glob-parent/issues/36">#36</a>)</li>
<li><a href="https://github.com/gulpjs/glob-parent/commit/0b014a7962789b2d8f2cf0b6311f40667aecd62c"><code>0b014a7</code></a> chore: add JSDoc returns information (<a href="https://redirect.github.com/gulpjs/glob-parent/issues/33">#33</a>)</li>
<li><a href="https://github.com/gulpjs/glob-parent/commit/2b24ebd64b2a045aa167c825376335555da139fd"><code>2b24ebd</code></a> chore: generate initial changelog</li>
<li><a href="https://github.com/gulpjs/glob-parent/commit/9b6e8747ddf664c9b1a36fbd2a23e43a35b8a52f"><code>9b6e874</code></a> chore: release 5.1.1</li>
<li><a href="https://github.com/gulpjs/glob-parent/commit/749c35ee084498ebb1ce8cc9cf655f6aa4d623c5"><code>749c35e</code></a> ci: try wrapping the JOB_ID in a string</li>
<li><a href="https://github.com/gulpjs/glob-parent/commit/5d39def48c9e9eaee0ca36dafdf7b6cdcd875b85"><code>5d39def</code></a> ci: attempt to switch to published coveralls</li>
<li><a href="https://github.com/gulpjs/glob-parent/commit/0b5b37f674a7e207457c99cb2f123299e5ab31c9"><code>0b5b37f</code></a> ci: put the npm step back in for only Windows</li>
<li><a href="https://github.com/gulpjs/glob-parent/commit/473f5d87644bf19f32c53de21d2420f03aa02e5a"><code>473f5d8</code></a> ci: update azure build images</li>
<li>Additional commits viewable in <a href="https://github.com/gulpjs/glob-parent/compare/v3.1.0...v5.1.2">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~phated">phated</a>, a new releaser for glob-parent since your current version.</p>
</details>
<br />

Updates `webpack-dev-server` from 3.11.3 to 4.13.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack-dev-server/releases">webpack-dev-server's releases</a>.</em></p>
<blockquote>
<h2>v4.13.1</h2>
<h3><a href="https://github.com/webpack/webpack-dev-server/compare/v4.13.0...v4.13.1">4.13.1</a> (2023-03-18)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>make webpack optional peer dependency (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4778">#4778</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/71be54edcb890f53d2cd900c2801989a17c2c9b1">71be54e</a>)</li>
</ul>
<h2>v4.13.0</h2>
<h2><a href="https://github.com/webpack/webpack-dev-server/compare/v4.12.0...v4.13.0">4.13.0</a> (2023-03-17)</h2>
<h3>Features</h3>
<ul>
<li>added <code>client.overlay.runtimeErrors</code> option to control runtime errors (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4773">#4773</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/dca2366e22a262e6052dae060c8b237f4e6fd26b">dca2366</a>)</li>
</ul>
<h2>v4.12.0</h2>
<h2><a href="https://github.com/webpack/webpack-dev-server/compare/v4.11.1...v4.12.0">4.12.0</a> (2023-03-14)</h2>
<h3>Features</h3>
<ul>
<li>allow to set the <code>sockjs_url</code> option (only <code>sockjs</code>) using the <code>webSocketServer.options.sockjsUrl</code> option (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4586">#4586</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/69a2fba4e915b4814de1c3cb27930a13dc994945">69a2fba</a>)</li>
<li>catch runtime error (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4605">#4605</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/87a26cf4c1fd9ac8140d345a8520a8d5cb059556">87a26cf</a>)</li>
<li>improve styles for overlay (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4576">#4576</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/791fb85931299eea052b3c37d4353d48ea34fa5e">791fb85</a>)</li>
<li>open editor when clicking error on overlay (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4587">#4587</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/efb2cec3f8acbbe5113aad20529e268c01ac29c2">efb2cec</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>compatibility with <code>experiments.buildHttp</code> (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4585">#4585</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/5b846cbe9bfb8444bc7605654fcebf4e87766aa4">5b846cb</a>)</li>
<li>respect <code>NODE_PATH</code> env variable (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4581">#4581</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/b857e6fa3b86facc63811438eef17be92dc36dc6">b857e6f</a>)</li>
</ul>
<h2>v4.11.1</h2>
<h3><a href="https://github.com/webpack/webpack-dev-server/compare/v4.11.0...v4.11.1">4.11.1</a> (2022-09-19)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>respect <code>client.logging</code> option for all logs (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4572">#4572</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/375835c926ec03fdfecae9ab1b54fd43b1ff4b31">375835c</a>)</li>
</ul>
<h2>v4.11.0</h2>
<h2><a href="https://github.com/webpack/webpack-dev-server/compare/v4.10.1...v4.11.0">4.11.0</a> (2022-09-07)</h2>
<h3>Features</h3>
<ul>
<li>make allowedHosts accept localhost subdomains by default (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4357">#4357</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/0a33e6a7529ef20ec8841c3fd501c37da179be3e">0a33e6a</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack-dev-server/blob/master/CHANGELOG.md">webpack-dev-server's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/webpack/webpack-dev-server/compare/v4.13.0...v4.13.1">4.13.1</a> (2023-03-18)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>make webpack optional peer dependency (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4778">#4778</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/71be54edcb890f53d2cd900c2801989a17c2c9b1">71be54e</a>)</li>
</ul>
<h2><a href="https://github.com/webpack/webpack-dev-server/compare/v4.12.0...v4.13.0">4.13.0</a> (2023-03-17)</h2>
<h3>Features</h3>
<ul>
<li>added <code>client.overlay.runtimeErrors</code> option to control runtime errors (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4773">#4773</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/dca2366e22a262e6052dae060c8b237f4e6fd26b">dca2366</a>)</li>
</ul>
<h2><a href="https://github.com/webpack/webpack-dev-server/compare/v4.11.1...v4.12.0">4.12.0</a> (2023-03-14)</h2>
<h3>Features</h3>
<ul>
<li>allow to set the <code>sockjs_url</code> option (only <code>sockjs</code>) using the <code>webSocketServer.options.sockjsUrl</code> option (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4586">#4586</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/69a2fba4e915b4814de1c3cb27930a13dc994945">69a2fba</a>)</li>
<li>catch runtime error (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4605">#4605</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/87a26cf4c1fd9ac8140d345a8520a8d5cb059556">87a26cf</a>)</li>
<li>improve styles for overlay (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4576">#4576</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/791fb85931299eea052b3c37d4353d48ea34fa5e">791fb85</a>)</li>
<li>open editor when clicking error on overlay (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4587">#4587</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/efb2cec3f8acbbe5113aad20529e268c01ac29c2">efb2cec</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>compatibility with <code>experiments.buildHttp</code> (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4585">#4585</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/5b846cbe9bfb8444bc7605654fcebf4e87766aa4">5b846cb</a>)</li>
<li>respect <code>NODE_PATH</code> env variable (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4581">#4581</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/b857e6fa3b86facc63811438eef17be92dc36dc6">b857e6f</a>)</li>
</ul>
<h3><a href="https://github.com/webpack/webpack-dev-server/compare/v4.11.0...v4.11.1">4.11.1</a> (2022-09-19)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>respect <code>client.logging</code> option for all logs (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4572">#4572</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/375835c926ec03fdfecae9ab1b54fd43b1ff4b31">375835c</a>)</li>
</ul>
<h2><a href="https://github.com/webpack/webpack-dev-server/compare/v4.10.1...v4.11.0">4.11.0</a> (2022-09-07)</h2>
<h3>Features</h3>
<ul>
<li>make allowedHosts accept localhost subdomains by default (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4357">#4357</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/0a33e6a7529ef20ec8841c3fd501c37da179be3e">0a33e6a</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>auto reply to OPTIONS requests only when unhandled (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4559">#4559</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/984af026a50f3e77c58abe24475da40a4ed038f1">984af02</a>), closes <a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4551">#4551</a></li>
</ul>
<h3><a href="https://github.com/webpack/webpack-dev-server/compare/v4.10.0...v4.10.1">4.10.1</a> (2022-08-29)</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack-dev-server/commit/ed0ca20af719e553b666ad2a5bc35f0cecef6dd0"><code>ed0ca20</code></a> chore(release): 4.13.1</li>
<li><a href="https://github.com/webpack/webpack-dev-server/commit/71be54edcb890f53d2cd900c2801989a17c2c9b1"><code>71be54e</code></a> fix: make webpack optional peer dependency (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4778">#4778</a>)</li>
<li><a href="https://github.com/webpack/webpack-dev-server/commit/4e846078b3b9befafbc56b1cd6db7778175355c9"><code>4e84607</code></a> chore(release): 4.13.0</li>
<li><a href="https://github.com/webpack/webpack-dev-server/commit/dca2366e22a262e6052dae060c8b237f4e6fd26b"><code>dca2366</code></a> feat: added <code>client.overlay.runtimeErrors</code> option to control runtime errors (...</li>
<li><a href="https://github.com/webpack/webpack-dev-server/commit/46e02f3d0b8406b120dc60f6c61960fb498c5d15"><code>46e02f3</code></a> chore(deps): bump graceful-fs from 4.2.10 to 4.2.11 (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4775">#4775</a>)</li>
<li><a href="https://github.com/webpack/webpack-dev-server/commit/cf7b0dbadb7718092ac4311dab92fd81c0c55636"><code>cf7b0db</code></a> chore(deps-dev): bump webpack from 5.76.1 to 5.76.2 (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4772">#4772</a>)</li>
<li><a href="https://github.com/webpack/webpack-dev-server/commit/2c8d98ca37f6b510591e7f855043db0bf49f76e3"><code>2c8d98c</code></a> chore(deps-dev): bump <code>@​babel/core</code> from 7.21.0 to 7.21.3 (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4769">#4769</a>)</li>
<li><a href="https://github.com/webpack/webpack-dev-server/commit/f1df0436922daa89650671a2be04671d8d05dce2"><code>f1df043</code></a> chore(deps-dev): bump <code>@​babel/eslint-parser</code> from 7.19.1 to 7.21.3 (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4770">#4770</a>)</li>
<li><a href="https://github.com/webpack/webpack-dev-server/commit/4ffcf2bd7100cb317b8606f3059ad31e754ec5ec"><code>4ffcf2b</code></a> chore(release): 4.12.0</li>
<li><a href="https://github.com/webpack/webpack-dev-server/commit/a615d5b52a77a57318da9ceac890015938452d9e"><code>a615d5b</code></a> chore(deps): update (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4768">#4768</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack-dev-server/compare/v3.11.3...v4.13.1">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-toolbox/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-24 16:43:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-toolbox/pull/317" class=".btn">#317</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump node-forge and webpack-dev-server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [node-forge](https://github.com/digitalbazaar/forge) to 1.3.1 and updates ancestor dependency [webpack-dev-server](https://github.com/webpack/webpack-dev-server). These dependencies need to be updated together.

Updates `node-forge` from 0.10.0 to 1.3.1
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/digitalbazaar/forge/blob/main/CHANGELOG.md">node-forge's changelog</a>.</em></p>
<blockquote>
<h2>1.3.1 - 2022-03-29</h2>
<h3>Fixes</h3>
<ul>
<li>RFC 3447 and RFC 8017 allow for optional <code>DigestAlgorithm</code> <code>NULL</code> parameters
for <code>sha*</code> algorithms and require <code>NULL</code> paramters for <code>md2</code> and <code>md5</code>
algorithms.</li>
</ul>
<h2>1.3.0 - 2022-03-17</h2>
<h3>Security</h3>
<ul>
<li>Three RSA PKCS#1 v1.5 signature verification issues were reported by Moosa
Yahyazadeh (<a href="mailto:moosa-yahyazadeh@uiowa.edu">moosa-yahyazadeh@uiowa.edu</a>).</li>
<li><strong>HIGH</strong>: Leniency in checking <code>digestAlgorithm</code> structure can lead to
signature forgery.
<ul>
<li>The code is lenient in checking the digest algorithm structure. This can
allow a crafted structure that steals padding bytes and uses unchecked
portion of the PKCS#1 encoded message to forge a signature when a low
public exponent is being used. For more information, please see
<a href="https://mailarchive.ietf.org/arch/msg/openpgp/5rnE9ZRN1AokBVj3VqblGlP63QE/">&quot;Bleichenbacher's RSA signature forgery based on implementation
error&quot;</a>
by Hal Finney.</li>
<li>CVE ID: <a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2022-24771">CVE-2022-24771</a></li>
<li>GHSA ID: <a href="https://github.com/digitalbazaar/forge/security/advisories/GHSA-cfm4-qjh2-4765">GHSA-cfm4-qjh2-4765</a></li>
</ul>
</li>
<li><strong>HIGH</strong>: Failing to check tailing garbage bytes can lead to signature
forgery.
<ul>
<li>The code does not check for tailing garbage bytes after decoding a
<code>DigestInfo</code> ASN.1 structure. This can allow padding bytes to be removed
and garbage data added to forge a signature when a low public exponent is
being used.  For more information, please see <a href="https://mailarchive.ietf.org/arch/msg/openpgp/5rnE9ZRN1AokBVj3VqblGlP63QE/">&quot;Bleichenbacher's RSA
signature forgery based on implementation
error&quot;</a>
by Hal Finney.</li>
<li>CVE ID: <a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2022-24772">CVE-2022-24772</a></li>
<li>GHSA ID: <a href="https://github.com/digitalbazaar/forge/security/advisories/GHSA-x4jg-mjrx-434g">GHSA-x4jg-mjrx-434g</a></li>
</ul>
</li>
<li><strong>MEDIUM</strong>: Leniency in checking type octet.
<ul>
<li><code>DigestInfo</code> is not properly checked for proper ASN.1 structure. This can
lead to successful verification with signatures that contain invalid
structures but a valid digest.</li>
<li>CVE ID: <a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2022-24773">CVE-2022-24773</a></li>
<li>GHSA ID: <a href="https://github.com/digitalbazaar/forge/security/advisories/GHSA-2r2c-g63r-vccr">GHSA-2r2c-g63r-vccr</a></li>
</ul>
</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>[asn1] Add fallback to pretty print invalid UTF8 data.</li>
<li>[asn1] <code>fromDer</code> is now more strict and will default to ensuring all input
bytes are parsed or throw an error. A new option <code>parseAllBytes</code> can disable
this behavior.
<ul>
<li><strong>NOTE</strong>: The previous behavior is being changed since it can lead to
security issues with crafted inputs. It is possible that code doing custom
DER parsing may need to adapt to this new behavior and optional flag.</li>
</ul>
</li>
<li>[rsa] Add and use a validator to check for proper structure of parsed ASN.1</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/digitalbazaar/forge/commit/a0a4a4264bedb3296974b9675349c9c190144aeb"><code>a0a4a42</code></a> Release 1.3.1.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/a33830f61c351e8e3a34309767e8dd0de148376b"><code>a33830f</code></a> Update changelog.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/740954d747ac56b76a6e1ae12a057c9548843436"><code>740954d</code></a> Allow optional DigestAlgorithm parameters.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/56f4316b4cc6592e678f8c416209c45984b6547b"><code>56f4316</code></a> Allow DigestInfo.DigestAlgorith.parameters to be optional</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/cbf0bd590d47fe3120a57e7c36f2f4e64381ad81"><code>cbf0bd5</code></a> Start 1.3.1-0.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/6c5b90133d46af63d139b98bf65371732c8c7dad"><code>6c5b901</code></a> Release 1.3.0.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/0f3972ad5883a9869703c6f54a0627bc454bca47"><code>0f3972a</code></a> Update changelog.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/dc77b39dd347e7f8b60a0f25a311fe5f06130579"><code>dc77b39</code></a> Fix error checking.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/bb822c02df0b61211836472e29b9790cc541cdb2"><code>bb822c0</code></a> Add advisory links.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/d4395fec831622837ecfec9e428d4620e208f9a8"><code>d4395fe</code></a> Update changelog.</li>
<li>Additional commits viewable in <a href="https://github.com/digitalbazaar/forge/compare/0.10.0...v1.3.1">compare view</a></li>
</ul>
</details>
<br />

Updates `webpack-dev-server` from 3.11.3 to 4.13.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack-dev-server/releases">webpack-dev-server's releases</a>.</em></p>
<blockquote>
<h2>v4.13.1</h2>
<h3><a href="https://github.com/webpack/webpack-dev-server/compare/v4.13.0...v4.13.1">4.13.1</a> (2023-03-18)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>make webpack optional peer dependency (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4778">#4778</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/71be54edcb890f53d2cd900c2801989a17c2c9b1">71be54e</a>)</li>
</ul>
<h2>v4.13.0</h2>
<h2><a href="https://github.com/webpack/webpack-dev-server/compare/v4.12.0...v4.13.0">4.13.0</a> (2023-03-17)</h2>
<h3>Features</h3>
<ul>
<li>added <code>client.overlay.runtimeErrors</code> option to control runtime errors (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4773">#4773</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/dca2366e22a262e6052dae060c8b237f4e6fd26b">dca2366</a>)</li>
</ul>
<h2>v4.12.0</h2>
<h2><a href="https://github.com/webpack/webpack-dev-server/compare/v4.11.1...v4.12.0">4.12.0</a> (2023-03-14)</h2>
<h3>Features</h3>
<ul>
<li>allow to set the <code>sockjs_url</code> option (only <code>sockjs</code>) using the <code>webSocketServer.options.sockjsUrl</code> option (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4586">#4586</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/69a2fba4e915b4814de1c3cb27930a13dc994945">69a2fba</a>)</li>
<li>catch runtime error (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4605">#4605</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/87a26cf4c1fd9ac8140d345a8520a8d5cb059556">87a26cf</a>)</li>
<li>improve styles for overlay (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4576">#4576</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/791fb85931299eea052b3c37d4353d48ea34fa5e">791fb85</a>)</li>
<li>open editor when clicking error on overlay (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4587">#4587</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/efb2cec3f8acbbe5113aad20529e268c01ac29c2">efb2cec</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>compatibility with <code>experiments.buildHttp</code> (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4585">#4585</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/5b846cbe9bfb8444bc7605654fcebf4e87766aa4">5b846cb</a>)</li>
<li>respect <code>NODE_PATH</code> env variable (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4581">#4581</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/b857e6fa3b86facc63811438eef17be92dc36dc6">b857e6f</a>)</li>
</ul>
<h2>v4.11.1</h2>
<h3><a href="https://github.com/webpack/webpack-dev-server/compare/v4.11.0...v4.11.1">4.11.1</a> (2022-09-19)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>respect <code>client.logging</code> option for all logs (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4572">#4572</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/375835c926ec03fdfecae9ab1b54fd43b1ff4b31">375835c</a>)</li>
</ul>
<h2>v4.11.0</h2>
<h2><a href="https://github.com/webpack/webpack-dev-server/compare/v4.10.1...v4.11.0">4.11.0</a> (2022-09-07)</h2>
<h3>Features</h3>
<ul>
<li>make allowedHosts accept localhost subdomains by default (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4357">#4357</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/0a33e6a7529ef20ec8841c3fd501c37da179be3e">0a33e6a</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack-dev-server/blob/master/CHANGELOG.md">webpack-dev-server's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/webpack/webpack-dev-server/compare/v4.13.0...v4.13.1">4.13.1</a> (2023-03-18)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>make webpack optional peer dependency (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4778">#4778</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/71be54edcb890f53d2cd900c2801989a17c2c9b1">71be54e</a>)</li>
</ul>
<h2><a href="https://github.com/webpack/webpack-dev-server/compare/v4.12.0...v4.13.0">4.13.0</a> (2023-03-17)</h2>
<h3>Features</h3>
<ul>
<li>added <code>client.overlay.runtimeErrors</code> option to control runtime errors (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4773">#4773</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/dca2366e22a262e6052dae060c8b237f4e6fd26b">dca2366</a>)</li>
</ul>
<h2><a href="https://github.com/webpack/webpack-dev-server/compare/v4.11.1...v4.12.0">4.12.0</a> (2023-03-14)</h2>
<h3>Features</h3>
<ul>
<li>allow to set the <code>sockjs_url</code> option (only <code>sockjs</code>) using the <code>webSocketServer.options.sockjsUrl</code> option (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4586">#4586</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/69a2fba4e915b4814de1c3cb27930a13dc994945">69a2fba</a>)</li>
<li>catch runtime error (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4605">#4605</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/87a26cf4c1fd9ac8140d345a8520a8d5cb059556">87a26cf</a>)</li>
<li>improve styles for overlay (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4576">#4576</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/791fb85931299eea052b3c37d4353d48ea34fa5e">791fb85</a>)</li>
<li>open editor when clicking error on overlay (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4587">#4587</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/efb2cec3f8acbbe5113aad20529e268c01ac29c2">efb2cec</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>compatibility with <code>experiments.buildHttp</code> (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4585">#4585</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/5b846cbe9bfb8444bc7605654fcebf4e87766aa4">5b846cb</a>)</li>
<li>respect <code>NODE_PATH</code> env variable (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4581">#4581</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/b857e6fa3b86facc63811438eef17be92dc36dc6">b857e6f</a>)</li>
</ul>
<h3><a href="https://github.com/webpack/webpack-dev-server/compare/v4.11.0...v4.11.1">4.11.1</a> (2022-09-19)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>respect <code>client.logging</code> option for all logs (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4572">#4572</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/375835c926ec03fdfecae9ab1b54fd43b1ff4b31">375835c</a>)</li>
</ul>
<h2><a href="https://github.com/webpack/webpack-dev-server/compare/v4.10.1...v4.11.0">4.11.0</a> (2022-09-07)</h2>
<h3>Features</h3>
<ul>
<li>make allowedHosts accept localhost subdomains by default (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4357">#4357</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/0a33e6a7529ef20ec8841c3fd501c37da179be3e">0a33e6a</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>auto reply to OPTIONS requests only when unhandled (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4559">#4559</a>) (<a href="https://github.com/webpack/webpack-dev-server/commit/984af026a50f3e77c58abe24475da40a4ed038f1">984af02</a>), closes <a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4551">#4551</a></li>
</ul>
<h3><a href="https://github.com/webpack/webpack-dev-server/compare/v4.10.0...v4.10.1">4.10.1</a> (2022-08-29)</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack-dev-server/commit/ed0ca20af719e553b666ad2a5bc35f0cecef6dd0"><code>ed0ca20</code></a> chore(release): 4.13.1</li>
<li><a href="https://github.com/webpack/webpack-dev-server/commit/71be54edcb890f53d2cd900c2801989a17c2c9b1"><code>71be54e</code></a> fix: make webpack optional peer dependency (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4778">#4778</a>)</li>
<li><a href="https://github.com/webpack/webpack-dev-server/commit/4e846078b3b9befafbc56b1cd6db7778175355c9"><code>4e84607</code></a> chore(release): 4.13.0</li>
<li><a href="https://github.com/webpack/webpack-dev-server/commit/dca2366e22a262e6052dae060c8b237f4e6fd26b"><code>dca2366</code></a> feat: added <code>client.overlay.runtimeErrors</code> option to control runtime errors (...</li>
<li><a href="https://github.com/webpack/webpack-dev-server/commit/46e02f3d0b8406b120dc60f6c61960fb498c5d15"><code>46e02f3</code></a> chore(deps): bump graceful-fs from 4.2.10 to 4.2.11 (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4775">#4775</a>)</li>
<li><a href="https://github.com/webpack/webpack-dev-server/commit/cf7b0dbadb7718092ac4311dab92fd81c0c55636"><code>cf7b0db</code></a> chore(deps-dev): bump webpack from 5.76.1 to 5.76.2 (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4772">#4772</a>)</li>
<li><a href="https://github.com/webpack/webpack-dev-server/commit/2c8d98ca37f6b510591e7f855043db0bf49f76e3"><code>2c8d98c</code></a> chore(deps-dev): bump <code>@​babel/core</code> from 7.21.0 to 7.21.3 (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4769">#4769</a>)</li>
<li><a href="https://github.com/webpack/webpack-dev-server/commit/f1df0436922daa89650671a2be04671d8d05dce2"><code>f1df043</code></a> chore(deps-dev): bump <code>@​babel/eslint-parser</code> from 7.19.1 to 7.21.3 (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4770">#4770</a>)</li>
<li><a href="https://github.com/webpack/webpack-dev-server/commit/4ffcf2bd7100cb317b8606f3059ad31e754ec5ec"><code>4ffcf2b</code></a> chore(release): 4.12.0</li>
<li><a href="https://github.com/webpack/webpack-dev-server/commit/a615d5b52a77a57318da9ceac890015938452d9e"><code>a615d5b</code></a> chore(deps): update (<a href="https://redirect.github.com/webpack/webpack-dev-server/issues/4768">#4768</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack-dev-server/compare/v3.11.3...v4.13.1">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-toolbox/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-22 16:31:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-toolbox/pull/315" class=".btn">#315</a>
            </td>
            <td>
                <b>
                    feat: add retrieve credential definitions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Summary

This pull request closes #314 by making the necessary changes to the `cred-def-list` component. 

The updates include setting the component property to be `retrievable` and passing the full list of `cred_defs`. Additionally, the `cred_defs` are now fetched during the `created` lifecycle. 

These changes will enable the user to retrieve the Credential Definitions by `TxID` and use them when creating the `Request Presentation`.

### Main Changes

- Set the `cred-def-list` component property to be `retrievable`
- Pass the full list of `cred_defs`
- Fetch the `cred_defs` during the `created` lifecycle

With these changes, users will be able to easily retrieve the Credential Definitions and use them in creating a Request Presentation, ultimately improving the overall functionality of the component.

![image](https://user-images.githubusercontent.com/6604111/226535339-657caf86-3292-4103-8b43-63f770b0bbd1.png)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-21 06:49:21 +0000 UTC
    </div>
</div>

