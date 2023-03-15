---
layout: default
title: bevel-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/bevel-samples
---

# bevel-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/bevel-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel-samples/pull/18" class=".btn">#18</a>
            </td>
            <td>
                <b>
                    Bump minimist and mkdirp in /examples/supplychain-app/supplychain-frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [minimist](https://github.com/minimistjs/minimist) and [mkdirp](https://github.com/isaacs/node-mkdirp). These dependencies needed to be updated together.
Updates `minimist` from 1.2.0 to 1.2.6
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/minimistjs/minimist/blob/main/CHANGELOG.md">minimist's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/minimistjs/minimist/compare/v1.2.5...v1.2.6">v1.2.6</a> - 2022-03-21</h2>
<h3>Commits</h3>
<ul>
<li>test from prototype pollution PR <a href="https://github.com/minimistjs/minimist/commit/bc8ecee43875261f4f17eb20b1243d3ed15e70eb"><code>bc8ecee</code></a></li>
<li>isConstructorOrProto adapted from PR <a href="https://github.com/minimistjs/minimist/commit/c2b981977fa834b223b408cfb860f933c9811e4d"><code>c2b9819</code></a></li>
<li>security notice for additional prototype pollution issue <a href="https://github.com/minimistjs/minimist/commit/ef88b9325f77b5ee643ccfc97e2ebda577e4c4e2"><code>ef88b93</code></a></li>
</ul>
<h2><a href="https://github.com/minimistjs/minimist/compare/v1.2.4...v1.2.5">v1.2.5</a> - 2020-03-12</h2>
<h2><a href="https://github.com/minimistjs/minimist/compare/v1.2.3...v1.2.4">v1.2.4</a> - 2020-03-11</h2>
<h3>Commits</h3>
<ul>
<li>security notice <a href="https://github.com/minimistjs/minimist/commit/4cf1354839cb972e38496d35e12f806eea92c11f"><code>4cf1354</code></a></li>
<li>additional test for constructor prototype pollution <a href="https://github.com/minimistjs/minimist/commit/1043d212c3caaf871966e710f52cfdf02f9eea4b"><code>1043d21</code></a></li>
</ul>
<h2><a href="https://github.com/minimistjs/minimist/compare/v1.2.2...v1.2.3">v1.2.3</a> - 2020-03-10</h2>
<h3>Commits</h3>
<ul>
<li>more failing proto pollution tests <a href="https://github.com/minimistjs/minimist/commit/13c01a5327736903704984b7f65616b8476850cc"><code>13c01a5</code></a></li>
<li>even more aggressive checks for protocol pollution <a href="https://github.com/minimistjs/minimist/commit/38a4d1caead72ef99e824bb420a2528eec03d9ab"><code>38a4d1c</code></a></li>
</ul>
<h2><a href="https://github.com/minimistjs/minimist/compare/v1.2.1...v1.2.2">v1.2.2</a> - 2020-03-10</h2>
<h3>Commits</h3>
<ul>
<li>failing test for protocol pollution <a href="https://github.com/minimistjs/minimist/commit/0efed0340ec8433638758f7ca0c77cb20a0bfbab"><code>0efed03</code></a></li>
<li>cleanup <a href="https://github.com/minimistjs/minimist/commit/67d3722413448d00a62963d2d30c34656a92d7e2"><code>67d3722</code></a></li>
<li>console.dir -&gt; console.log <a href="https://github.com/minimistjs/minimist/commit/47acf72c715a630bf9ea013867f47f1dd69dfc54"><code>47acf72</code></a></li>
<li>don't assign onto <strong>proto</strong> <a href="https://github.com/minimistjs/minimist/commit/63e7ed05aa4b1889ec2f3b196426db4500cbda94"><code>63e7ed0</code></a></li>
</ul>
<h2><a href="https://github.com/minimistjs/minimist/compare/v1.2.0...v1.2.1">v1.2.1</a> - 2020-03-10</h2>
<h3>Merged</h3>
<ul>
<li>move the <code>opts['--']</code> example back where it belongs <a href="https://redirect.github.com/minimistjs/minimist/pull/63"><code>[#63](https://github.com/minimistjs/minimist/issues/63)</code></a></li>
</ul>
<h3>Commits</h3>
<ul>
<li>add test <a href="https://github.com/minimistjs/minimist/commit/6be5dae35a32a987bcf4137fcd6c19c5200ee909"><code>6be5dae</code></a></li>
<li>fix bad boolean regexp <a href="https://github.com/minimistjs/minimist/commit/ac3fc796e63b95128fdbdf67ea7fad71bd59aa76"><code>ac3fc79</code></a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/minimistjs/minimist/commit/7efb22a518b53b06f5b02a1038a88bd6290c2846"><code>7efb22a</code></a> 1.2.6</li>
<li><a href="https://github.com/minimistjs/minimist/commit/ef88b9325f77b5ee643ccfc97e2ebda577e4c4e2"><code>ef88b93</code></a> security notice for additional prototype pollution issue</li>
<li><a href="https://github.com/minimistjs/minimist/commit/c2b981977fa834b223b408cfb860f933c9811e4d"><code>c2b9819</code></a> isConstructorOrProto adapted from PR</li>
<li><a href="https://github.com/minimistjs/minimist/commit/bc8ecee43875261f4f17eb20b1243d3ed15e70eb"><code>bc8ecee</code></a> test from prototype pollution PR</li>
<li><a href="https://github.com/minimistjs/minimist/commit/aeb3e27dae0412de5c0494e9563a5f10c82cc7a9"><code>aeb3e27</code></a> 1.2.5</li>
<li><a href="https://github.com/minimistjs/minimist/commit/278677b171d956b46613a158c6c486c3ef979b20"><code>278677b</code></a> 1.2.4</li>
<li><a href="https://github.com/minimistjs/minimist/commit/4cf1354839cb972e38496d35e12f806eea92c11f"><code>4cf1354</code></a> security notice</li>
<li><a href="https://github.com/minimistjs/minimist/commit/1043d212c3caaf871966e710f52cfdf02f9eea4b"><code>1043d21</code></a> additional test for constructor prototype pollution</li>
<li><a href="https://github.com/minimistjs/minimist/commit/6457d7440a47f329c12c4a5abfbce211c4235b93"><code>6457d74</code></a> 1.2.3</li>
<li><a href="https://github.com/minimistjs/minimist/commit/38a4d1caead72ef99e824bb420a2528eec03d9ab"><code>38a4d1c</code></a> even more aggressive checks for protocol pollution</li>
<li>Additional commits viewable in <a href="https://github.com/minimistjs/minimist/compare/v1.2.0...v1.2.6">compare view</a></li>
</ul>
</details>
<br />

Updates `mkdirp` from 0.5.1 to 0.5.5
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/isaacs/node-mkdirp/commit/049cf185c9e91727bc505b796a2d16a4fe70d64d"><code>049cf18</code></a> 0.5.5</li>
<li><a href="https://github.com/isaacs/node-mkdirp/commit/bea638225aa991095f29a9e16d914effa0c134fe"><code>bea6382</code></a> Remove unnecessary umask calls</li>
<li><a href="https://github.com/isaacs/node-mkdirp/commit/42a012cc6dbd4648790f380df88190bb697dbb9c"><code>42a012c</code></a> 0.5.4</li>
<li><a href="https://github.com/isaacs/node-mkdirp/commit/2867920c08dc6c47bad0ea5b385a8e78bade0c8f"><code>2867920</code></a> fix infinite loop on windows machines</li>
<li><a href="https://github.com/isaacs/node-mkdirp/commit/d784e70d1eb3fc73bcda52f22f57ec55c00c2525"><code>d784e70</code></a> 0.5.3</li>
<li><a href="https://github.com/isaacs/node-mkdirp/commit/d612c5ddca62d50282147f5d199810bf1de0b314"><code>d612c5d</code></a> add files list so this package isn't a monster</li>
<li><a href="https://github.com/isaacs/node-mkdirp/commit/b2e7ba0dd8ac7029735969c5a6062d49e839b30d"><code>b2e7ba0</code></a> 0.5.2</li>
<li><a href="https://github.com/isaacs/node-mkdirp/commit/c5b97d17d45a22bcf4c815645cbb989dab57ddd8"><code>c5b97d1</code></a> bump minimist to 1.2 to fix security issue</li>
<li><a href="https://github.com/isaacs/node-mkdirp/commit/f2003bbcffa80f8c9744579fabab1212fc84545a"><code>f2003bb</code></a> test: add v4 and v5 to travis</li>
<li><a href="https://github.com/isaacs/node-mkdirp/commit/b8629ffd27c7f3fa8a6fc28b60206ab1d0cb081e"><code>b8629ff</code></a> tools: update tap + mock-fs. Fix broken test</li>
<li>See full diff in <a href="https://github.com/isaacs/node-mkdirp/compare/0.5.1...v0.5.5">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~isaacs">isaacs</a>, a new releaser for mkdirp since your current version.</p>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-14 17:29:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel-samples/pull/17" class=".btn">#17</a>
            </td>
            <td>
                <b>
                    Bump vertx-web from 3.7.1 to 3.9.4 in /images/doorman
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">java</span>
            </td>
            <td>
                Bumps vertx-web from 3.7.1 to 3.9.4.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=io.vertx:vertx-web&package-manager=maven&previous-version=3.7.1&new-version=3.9.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-14 17:27:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel-samples/pull/16" class=".btn">#16</a>
            </td>
            <td>
                <b>
                    Update maintainers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Move Jonathan to emeritus status
Add Jagpreet and Aditya to maintainers
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-14 17:11:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel-samples/pull/15" class=".btn">#15</a>
            </td>
            <td>
                <b>
                    Update: Move tkuhrt to emeritus maintainer
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
        Created At 2023-03-14 16:43:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel-samples/pull/14" class=".btn">#14</a>
            </td>
            <td>
                <b>
                    Bump postcss and stylus-brunch in /images/doorman/website
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [postcss](https://github.com/postcss/postcss) to 7.0.39 and updates ancestor dependency [stylus-brunch](https://github.com/brunch/stylus-brunch). These dependencies need to be updated together.

Updates `postcss` from 5.0.21 to 7.0.39
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/postcss/postcss/releases">postcss's releases</a>.</em></p>
<blockquote>
<h2>7.0.39</h2>
<ul>
<li>Reduce package size.</li>
<li>Backport <code>nanocolors</code> to <code>picocolors</code> migration.</li>
</ul>
<h2>7.0.38</h2>
<ul>
<li>Update <code>Processor#version</code>.</li>
</ul>
<h2>7.0.37</h2>
<ul>
<li>Backport <code>chalk</code> to <code>nanocolors</code> migration.</li>
</ul>
<h2>7.0.36</h2>
<ul>
<li>Backport ReDoS vulnerabilities from PostCSS 8.</li>
</ul>
<h2>7.0.35</h2>
<ul>
<li>Add <a href="https://github.com/postcss/postcss/wiki/PostCSS-8-for-end-users">migration guide link</a> to PostCSS 8 error text.</li>
</ul>
<h2>7.0.34</h2>
<ul>
<li>Fix compatibility with <code>postcss-scss</code> 2.</li>
</ul>
<h2>7.0.33</h2>
<ul>
<li>Add error message for PostCSS 8 plugins.</li>
</ul>
<h2>7.0.32</h2>
<ul>
<li>Fix error message (by <a href="https://github.com/admosity"><code>@​admosity</code></a>).</li>
</ul>
<h2>7.0.31</h2>
<ul>
<li>Use only the latest source map annotation (by <a href="https://github.com/emzoumpo"><code>@​emzoumpo</code></a>).</li>
</ul>
<h2>7.0.30</h2>
<ul>
<li>Fix TypeScript definition (by <a href="https://github.com/nex3"><code>@​nex3</code></a>)</li>
</ul>
<h2>7.0.29</h2>
<ul>
<li>Update <code>Processor#version</code>.</li>
</ul>
<h2>7.0.28</h2>
<ul>
<li>Fix TypeScript definition (by <a href="https://github.com/nex3"><code>@​nex3</code></a>).</li>
</ul>
<h2>7.0.27</h2>
<ul>
<li>Fix TypeScript definition (by <a href="https://github.com/nex3"><code>@​nex3</code></a>).</li>
</ul>
<h2>7.0.26</h2>
<ul>
<li>Fix TypeScript definition (by <a href="https://github.com/nex3"><code>@​nex3</code></a>)</li>
</ul>
<h2>7.0.25</h2>
<ul>
<li>Fix absolute path support for Windows (by <a href="https://github.com/tomrav"><code>@​tomrav</code></a>)</li>
</ul>
<h2>7.0.24</h2>
<ul>
<li>Fix TypeScript definition (by <a href="https://github.com/keithamus"><code>@​keithamus</code></a>).</li>
</ul>
<h2>7.0.23</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/postcss/postcss/blob/7.0.39/CHANGELOG.md">postcss's changelog</a>.</em></p>
<blockquote>
<h2>7.0.39</h2>
<ul>
<li>Reduce package size.</li>
<li>Backport <code>nanocolors</code> to <code>picocolors</code> migration.</li>
</ul>
<h2>7.0.38</h2>
<ul>
<li>Update <code>Processor#version</code>.</li>
</ul>
<h2>7.0.37</h2>
<ul>
<li>Backport <code>chalk</code> to <code>nanocolors</code> migration.</li>
</ul>
<h2>7.0.36</h2>
<ul>
<li>Backport ReDoS vulnerabilities from PostCSS 8.</li>
</ul>
<h2>7.0.35</h2>
<ul>
<li>Add migration guide link to PostCSS 8 error text.</li>
</ul>
<h2>7.0.34</h2>
<ul>
<li>Fix compatibility with <code>postcss-scss</code> 2.</li>
</ul>
<h2>7.0.33</h2>
<ul>
<li>Add error message for PostCSS 8 plugins.</li>
</ul>
<h2>7.0.32</h2>
<ul>
<li>Fix error message (by <a href="https://github.com/admosity"><code>@​admosity</code></a>).</li>
</ul>
<h2>7.0.31</h2>
<ul>
<li>Use only the latest source map annotation (by Emmanouil Zoumpoulakis).</li>
</ul>
<h2>7.0.30</h2>
<ul>
<li>Fix TypeScript definition (by Natalie Weizenbaum).</li>
</ul>
<h2>7.0.29</h2>
<ul>
<li>Update <code>Processor#version</code>.</li>
</ul>
<h2>7.0.28</h2>
<ul>
<li>Fix TypeScript definition (by Natalie Weizenbaum).</li>
</ul>
<h2>7.0.27</h2>
<ul>
<li>Fix TypeScript definition (by Natalie Weizenbaum).</li>
</ul>
<h2>7.0.26</h2>
<ul>
<li>Fix TypeScript definition (by Natalie Weizenbaum).</li>
</ul>
<h2>7.0.25</h2>
<ul>
<li>Fix absolute path support for Windows (by Tom Raviv).</li>
</ul>
<h2>7.0.24</h2>
<ul>
<li>Fix TypeScript definition (by Keith Cirkel).</li>
</ul>
<h2>7.0.23</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/postcss/postcss/commit/e17c1ef7623a71be5732432ca8499bc9928aa08d"><code>e17c1ef</code></a> Release 7.0.39 version</li>
<li><a href="https://github.com/postcss/postcss/commit/6791bd3d5f7ab27ad36dc075033a5beb4bdbfe9e"><code>6791bd3</code></a> Reduce npm package</li>
<li><a href="https://github.com/postcss/postcss/commit/44c581a55a9aab339ee319aa67c264b02c4a6448"><code>44c581a</code></a> Replace nanocolors with picocolors</li>
<li><a href="https://github.com/postcss/postcss/commit/8ba21fd8f4c3bff146b8a71d2d12f31435444394"><code>8ba21fd</code></a> Remove eslint-ci</li>
<li><a href="https://github.com/postcss/postcss/commit/3994c4aa3ce1835c9b36ae17ab94e45c21b56fb2"><code>3994c4a</code></a> Release 7.0.38 version</li>
<li><a href="https://github.com/postcss/postcss/commit/6944e1dd808da66cee4ebf287c66c6aa0fc5c2a0"><code>6944e1d</code></a> Remove development keys from package.json</li>
<li><a href="https://github.com/postcss/postcss/commit/4dd0af024a915bd12d2d53990c5a4fa4129563d5"><code>4dd0af0</code></a> Release 7.0.37 version</li>
<li><a href="https://github.com/postcss/postcss/commit/8408eb4105755c43dbf09a000fd2f1308f240232"><code>8408eb4</code></a> Add compilation step</li>
<li><a href="https://github.com/postcss/postcss/commit/0c680639c3d717b4c8c0b2b2a9d1799fbf239a76"><code>0c68063</code></a> Move tests to GitHub Actions</li>
<li><a href="https://github.com/postcss/postcss/commit/98b61ba5b46622de48bb2592583757ab846212ad"><code>98b61ba</code></a> Replace chalk to nanocolors</li>
<li>Additional commits viewable in <a href="https://github.com/postcss/postcss/compare/5.0.21...7.0.39">compare view</a></li>
</ul>
</details>
<br />

Updates `stylus-brunch` from 2.10.0 to 3.0.0
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/brunch/stylus-brunch/commit/006560182f404e6dae1a81b0e4a0a93111d124a3"><code>0065601</code></a> Release 3.0.0.</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/72ddf4e58abe0651e05b54db5ef94fbe18d3d02e"><code>72ddf4e</code></a> Updates.</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/5d33bd456a94763b554f18cdb12a6181caa75142"><code>5d33bd4</code></a> Updates.</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/4f1836b6c01e92a17e3c4d896ffa5c928b343d0c"><code>4f1836b</code></a> Reorganize for brunch 3.</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/17c771ce42730660ae114f2af37d44684126d108"><code>17c771c</code></a> Release 2.10.1.</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/ced960d9d9e3438185f1a192800a49d23948f824"><code>ced960d</code></a> Merge pull request <a href="https://redirect.github.com/brunch/stylus-brunch/issues/65">#65</a> from brunch/target-extension</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/90e050ebd6ffc1f5c51f881844792c077b9a58a0"><code>90e050e</code></a> Bring back nib.</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/98265a87bbdeb1e1a4a171b06419552896b907b0"><code>98265a8</code></a> Bring back nib.</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/eba579f91968e7e0ed3530b5d9548b8a5ae0915b"><code>eba579f</code></a> Include CSS by default</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/f7935f34b1c3579ac363b4dccb4812d448b72bdf"><code>f7935f3</code></a> Update index.js</li>
<li>Additional commits viewable in <a href="https://github.com/brunch/stylus-brunch/compare/2.10.0...3.0.0">compare view</a></li>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-10 07:09:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel-samples/pull/13" class=".btn">#13</a>
            </td>
            <td>
                <b>
                    Bump postcss and stylus-brunch in /images/networkmap/website
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [postcss](https://github.com/postcss/postcss) to 7.0.39 and updates ancestor dependency [stylus-brunch](https://github.com/brunch/stylus-brunch). These dependencies need to be updated together.

Updates `postcss` from 5.0.21 to 7.0.39
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/postcss/postcss/releases">postcss's releases</a>.</em></p>
<blockquote>
<h2>7.0.39</h2>
<ul>
<li>Reduce package size.</li>
<li>Backport <code>nanocolors</code> to <code>picocolors</code> migration.</li>
</ul>
<h2>7.0.38</h2>
<ul>
<li>Update <code>Processor#version</code>.</li>
</ul>
<h2>7.0.37</h2>
<ul>
<li>Backport <code>chalk</code> to <code>nanocolors</code> migration.</li>
</ul>
<h2>7.0.36</h2>
<ul>
<li>Backport ReDoS vulnerabilities from PostCSS 8.</li>
</ul>
<h2>7.0.35</h2>
<ul>
<li>Add <a href="https://github.com/postcss/postcss/wiki/PostCSS-8-for-end-users">migration guide link</a> to PostCSS 8 error text.</li>
</ul>
<h2>7.0.34</h2>
<ul>
<li>Fix compatibility with <code>postcss-scss</code> 2.</li>
</ul>
<h2>7.0.33</h2>
<ul>
<li>Add error message for PostCSS 8 plugins.</li>
</ul>
<h2>7.0.32</h2>
<ul>
<li>Fix error message (by <a href="https://github.com/admosity"><code>@​admosity</code></a>).</li>
</ul>
<h2>7.0.31</h2>
<ul>
<li>Use only the latest source map annotation (by <a href="https://github.com/emzoumpo"><code>@​emzoumpo</code></a>).</li>
</ul>
<h2>7.0.30</h2>
<ul>
<li>Fix TypeScript definition (by <a href="https://github.com/nex3"><code>@​nex3</code></a>)</li>
</ul>
<h2>7.0.29</h2>
<ul>
<li>Update <code>Processor#version</code>.</li>
</ul>
<h2>7.0.28</h2>
<ul>
<li>Fix TypeScript definition (by <a href="https://github.com/nex3"><code>@​nex3</code></a>).</li>
</ul>
<h2>7.0.27</h2>
<ul>
<li>Fix TypeScript definition (by <a href="https://github.com/nex3"><code>@​nex3</code></a>).</li>
</ul>
<h2>7.0.26</h2>
<ul>
<li>Fix TypeScript definition (by <a href="https://github.com/nex3"><code>@​nex3</code></a>)</li>
</ul>
<h2>7.0.25</h2>
<ul>
<li>Fix absolute path support for Windows (by <a href="https://github.com/tomrav"><code>@​tomrav</code></a>)</li>
</ul>
<h2>7.0.24</h2>
<ul>
<li>Fix TypeScript definition (by <a href="https://github.com/keithamus"><code>@​keithamus</code></a>).</li>
</ul>
<h2>7.0.23</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/postcss/postcss/blob/7.0.39/CHANGELOG.md">postcss's changelog</a>.</em></p>
<blockquote>
<h2>7.0.39</h2>
<ul>
<li>Reduce package size.</li>
<li>Backport <code>nanocolors</code> to <code>picocolors</code> migration.</li>
</ul>
<h2>7.0.38</h2>
<ul>
<li>Update <code>Processor#version</code>.</li>
</ul>
<h2>7.0.37</h2>
<ul>
<li>Backport <code>chalk</code> to <code>nanocolors</code> migration.</li>
</ul>
<h2>7.0.36</h2>
<ul>
<li>Backport ReDoS vulnerabilities from PostCSS 8.</li>
</ul>
<h2>7.0.35</h2>
<ul>
<li>Add migration guide link to PostCSS 8 error text.</li>
</ul>
<h2>7.0.34</h2>
<ul>
<li>Fix compatibility with <code>postcss-scss</code> 2.</li>
</ul>
<h2>7.0.33</h2>
<ul>
<li>Add error message for PostCSS 8 plugins.</li>
</ul>
<h2>7.0.32</h2>
<ul>
<li>Fix error message (by <a href="https://github.com/admosity"><code>@​admosity</code></a>).</li>
</ul>
<h2>7.0.31</h2>
<ul>
<li>Use only the latest source map annotation (by Emmanouil Zoumpoulakis).</li>
</ul>
<h2>7.0.30</h2>
<ul>
<li>Fix TypeScript definition (by Natalie Weizenbaum).</li>
</ul>
<h2>7.0.29</h2>
<ul>
<li>Update <code>Processor#version</code>.</li>
</ul>
<h2>7.0.28</h2>
<ul>
<li>Fix TypeScript definition (by Natalie Weizenbaum).</li>
</ul>
<h2>7.0.27</h2>
<ul>
<li>Fix TypeScript definition (by Natalie Weizenbaum).</li>
</ul>
<h2>7.0.26</h2>
<ul>
<li>Fix TypeScript definition (by Natalie Weizenbaum).</li>
</ul>
<h2>7.0.25</h2>
<ul>
<li>Fix absolute path support for Windows (by Tom Raviv).</li>
</ul>
<h2>7.0.24</h2>
<ul>
<li>Fix TypeScript definition (by Keith Cirkel).</li>
</ul>
<h2>7.0.23</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/postcss/postcss/commit/e17c1ef7623a71be5732432ca8499bc9928aa08d"><code>e17c1ef</code></a> Release 7.0.39 version</li>
<li><a href="https://github.com/postcss/postcss/commit/6791bd3d5f7ab27ad36dc075033a5beb4bdbfe9e"><code>6791bd3</code></a> Reduce npm package</li>
<li><a href="https://github.com/postcss/postcss/commit/44c581a55a9aab339ee319aa67c264b02c4a6448"><code>44c581a</code></a> Replace nanocolors with picocolors</li>
<li><a href="https://github.com/postcss/postcss/commit/8ba21fd8f4c3bff146b8a71d2d12f31435444394"><code>8ba21fd</code></a> Remove eslint-ci</li>
<li><a href="https://github.com/postcss/postcss/commit/3994c4aa3ce1835c9b36ae17ab94e45c21b56fb2"><code>3994c4a</code></a> Release 7.0.38 version</li>
<li><a href="https://github.com/postcss/postcss/commit/6944e1dd808da66cee4ebf287c66c6aa0fc5c2a0"><code>6944e1d</code></a> Remove development keys from package.json</li>
<li><a href="https://github.com/postcss/postcss/commit/4dd0af024a915bd12d2d53990c5a4fa4129563d5"><code>4dd0af0</code></a> Release 7.0.37 version</li>
<li><a href="https://github.com/postcss/postcss/commit/8408eb4105755c43dbf09a000fd2f1308f240232"><code>8408eb4</code></a> Add compilation step</li>
<li><a href="https://github.com/postcss/postcss/commit/0c680639c3d717b4c8c0b2b2a9d1799fbf239a76"><code>0c68063</code></a> Move tests to GitHub Actions</li>
<li><a href="https://github.com/postcss/postcss/commit/98b61ba5b46622de48bb2592583757ab846212ad"><code>98b61ba</code></a> Replace chalk to nanocolors</li>
<li>Additional commits viewable in <a href="https://github.com/postcss/postcss/compare/5.0.21...7.0.39">compare view</a></li>
</ul>
</details>
<br />

Updates `stylus-brunch` from 2.10.0 to 3.0.0
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/brunch/stylus-brunch/commit/006560182f404e6dae1a81b0e4a0a93111d124a3"><code>0065601</code></a> Release 3.0.0.</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/72ddf4e58abe0651e05b54db5ef94fbe18d3d02e"><code>72ddf4e</code></a> Updates.</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/5d33bd456a94763b554f18cdb12a6181caa75142"><code>5d33bd4</code></a> Updates.</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/4f1836b6c01e92a17e3c4d896ffa5c928b343d0c"><code>4f1836b</code></a> Reorganize for brunch 3.</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/17c771ce42730660ae114f2af37d44684126d108"><code>17c771c</code></a> Release 2.10.1.</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/ced960d9d9e3438185f1a192800a49d23948f824"><code>ced960d</code></a> Merge pull request <a href="https://redirect.github.com/brunch/stylus-brunch/issues/65">#65</a> from brunch/target-extension</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/90e050ebd6ffc1f5c51f881844792c077b9a58a0"><code>90e050e</code></a> Bring back nib.</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/98265a87bbdeb1e1a4a171b06419552896b907b0"><code>98265a8</code></a> Bring back nib.</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/eba579f91968e7e0ed3530b5d9548b8a5ae0915b"><code>eba579f</code></a> Include CSS by default</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/f7935f34b1c3579ac363b4dccb4812d448b72bdf"><code>f7935f3</code></a> Update index.js</li>
<li>Additional commits viewable in <a href="https://github.com/brunch/stylus-brunch/compare/2.10.0...3.0.0">compare view</a></li>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-10 07:09:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel-samples/pull/12" class=".btn">#12</a>
            </td>
            <td>
                <b>
                    Bump ua-parser-js from 0.7.31 to 0.7.34 in /images/networkmap/website
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [ua-parser-js](https://github.com/faisalman/ua-parser-js) from 0.7.31 to 0.7.34.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/faisalman/ua-parser-js/blob/0.7.34/changelog.md">ua-parser-js's changelog</a>.</em></p>
<blockquote>
<h2>Version 0.7.34 / 1.0.34</h2>
<ul>
<li>Fix Sharp Mobile detected as Huawei Tablet</li>
<li>Fix IE8 bug</li>
<li>Add new devices : Kobo e-Reader, Apple Watch, and some new SmartTV devices</li>
<li>Add new OS : watchOS</li>
<li>Improve browser detection : Kakao, Naver, Brave</li>
<li>Improve device detection : Oculus, iPad</li>
<li>Improve OS detection : Chrome OS</li>
<li>Using navigator.userAgentData as fallback for device.type &amp; os.name</li>
</ul>
<h2>Version 0.7.33 / 1.0.33</h2>
<ul>
<li>Add new browser : Cobalt</li>
<li>Identify Macintosh as an Apple device</li>
<li>Fix ReDoS vulnerability</li>
</ul>
<h2>Version 0.7.32 / 1.0.32</h2>
<ul>
<li>Add new browser : DuckDuckGo, Huawei Browser, LinkedIn</li>
<li>Add new OS : HarmonyOS</li>
<li>Add some Huawei models</li>
<li>Add Sharp Aquos TV</li>
<li>Improve detection Xiaomi Mi CC9</li>
<li>Fix Sony Xperia 1 III misidentified as Acer tablet</li>
<li>Fix Detect Sony BRAVIA as SmartTV</li>
<li>Fix Detect Xiaomi Mi TV as SmartTV</li>
<li>Fix Detect Galaxy Tab S8 as tablet</li>
<li>Fix WeGame mistakenly identified as WeChat</li>
<li>Fix included commas in Safari / Mobile Safari version</li>
<li>Increase UA_MAX_LENGTH to 350</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/3218051f0739a4a7990b06210983917a11da7904"><code>3218051</code></a> Bump version 0.7.34</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/551ad8847403b82f06c8a834d946d7c6ade6e9ad"><code>551ad88</code></a> Add new device: Apple Watch, new os: watchOS</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/097f736c4d6913312880810d8452b775ec2fa020"><code>097f736</code></a> Fix <a href="https://redirect.github.com/faisalman/ua-parser-js/issues/387">#387</a> <a href="https://redirect.github.com/faisalman/ua-parser-js/issues/554">#554</a> - Detect iPadOS 13</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/73c25771dcd152d415bedb5c0569bc06f6ff65f2"><code>73c2577</code></a> Fix <a href="https://redirect.github.com/faisalman/ua-parser-js/issues/498">#498</a> - Detect Brave Browser by checking navigator.brave</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/f8e5a1fb4fbe55b781a48d7d141fdc41ba93fa38"><code>f8e5a1f</code></a> Fix <a href="https://redirect.github.com/faisalman/ua-parser-js/issues/601">#601</a> - Detect Chrome OS without version</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/c9d1ab95610a9754859ff97c7fda76694f3f76ea"><code>c9d1ab9</code></a> Merge branch 'develop'</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/f815ca6e9cabce4099103b21423d7a9c4531c57a"><code>f815ca6</code></a> Fix <a href="https://redirect.github.com/faisalman/ua-parser-js/issues/620">#620</a> - Add new Device: Kobo</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/0cbeb7a82966aac71e7cadb4794669dabd339868"><code>0cbeb7a</code></a> Rearrange the recently added smarttv detection</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/bf4fb916ca6586c70076a31dd44369d56c44a9e8"><code>bf4fb91</code></a> Merge pull request <a href="https://redirect.github.com/faisalman/ua-parser-js/issues/618">#618</a> from garritfra/smarttv</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/68447d883afc9cdc03e32aad610f4296563c9a5c"><code>68447d8</code></a> Merge branch 'develop' of github.com:faisalman/ua-parser-js into develop</li>
<li>Additional commits viewable in <a href="https://github.com/faisalman/ua-parser-js/compare/0.7.31...0.7.34">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ua-parser-js&package-manager=npm_and_yarn&previous-version=0.7.31&new-version=0.7.34)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-10 07:09:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel-samples/pull/11" class=".btn">#11</a>
            </td>
            <td>
                <b>
                    Bump ua-parser-js from 0.7.28 to 0.7.34 in /images/doorman/website
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [ua-parser-js](https://github.com/faisalman/ua-parser-js) from 0.7.28 to 0.7.34.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/faisalman/ua-parser-js/blob/0.7.34/changelog.md">ua-parser-js's changelog</a>.</em></p>
<blockquote>
<h2>Version 0.7.34 / 1.0.34</h2>
<ul>
<li>Fix Sharp Mobile detected as Huawei Tablet</li>
<li>Fix IE8 bug</li>
<li>Add new devices : Kobo e-Reader, Apple Watch, and some new SmartTV devices</li>
<li>Add new OS : watchOS</li>
<li>Improve browser detection : Kakao, Naver, Brave</li>
<li>Improve device detection : Oculus, iPad</li>
<li>Improve OS detection : Chrome OS</li>
<li>Using navigator.userAgentData as fallback for device.type &amp; os.name</li>
</ul>
<h2>Version 0.7.33 / 1.0.33</h2>
<ul>
<li>Add new browser : Cobalt</li>
<li>Identify Macintosh as an Apple device</li>
<li>Fix ReDoS vulnerability</li>
</ul>
<h2>Version 0.7.32 / 1.0.32</h2>
<ul>
<li>Add new browser : DuckDuckGo, Huawei Browser, LinkedIn</li>
<li>Add new OS : HarmonyOS</li>
<li>Add some Huawei models</li>
<li>Add Sharp Aquos TV</li>
<li>Improve detection Xiaomi Mi CC9</li>
<li>Fix Sony Xperia 1 III misidentified as Acer tablet</li>
<li>Fix Detect Sony BRAVIA as SmartTV</li>
<li>Fix Detect Xiaomi Mi TV as SmartTV</li>
<li>Fix Detect Galaxy Tab S8 as tablet</li>
<li>Fix WeGame mistakenly identified as WeChat</li>
<li>Fix included commas in Safari / Mobile Safari version</li>
<li>Increase UA_MAX_LENGTH to 350</li>
</ul>
<h2>Version 0.7.31 / 1.0.2</h2>
<ul>
<li>Fix OPPO Reno A5 incorrect detection</li>
<li>Fix TypeError Bug</li>
<li>Use AST to extract regexes and verify them with safe-regex</li>
</ul>
<h2>Version 0.7.30 / 1.0.1</h2>
<ul>
<li>Add new browser : Obigo, UP.Browser, Klar</li>
<li>Add new device : Oculus, Roku</li>
<li>Add new OS: Maemo, HP-UX, Android-x86, Deepin, elementary OS, GhostBSD, Linspire, Manjaro, Sabayon</li>
<li>Improve detection for Sony Xperia 1ii, LG Android TV, and some more devices</li>
<li>Improve detection for ARM64 CPU</li>
<li>Improve detection for Windows Mobile, Netscape, Mac on PowerPC</li>
<li>Categorize PDA as mobile</li>
<li>Fix Sharp devices misjudged as Huawei</li>
<li>Fix trailing comma for ES3 compatibility</li>
<li>Some code refactor</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/3218051f0739a4a7990b06210983917a11da7904"><code>3218051</code></a> Bump version 0.7.34</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/551ad8847403b82f06c8a834d946d7c6ade6e9ad"><code>551ad88</code></a> Add new device: Apple Watch, new os: watchOS</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/097f736c4d6913312880810d8452b775ec2fa020"><code>097f736</code></a> Fix <a href="https://redirect.github.com/faisalman/ua-parser-js/issues/387">#387</a> <a href="https://redirect.github.com/faisalman/ua-parser-js/issues/554">#554</a> - Detect iPadOS 13</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/73c25771dcd152d415bedb5c0569bc06f6ff65f2"><code>73c2577</code></a> Fix <a href="https://redirect.github.com/faisalman/ua-parser-js/issues/498">#498</a> - Detect Brave Browser by checking navigator.brave</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/f8e5a1fb4fbe55b781a48d7d141fdc41ba93fa38"><code>f8e5a1f</code></a> Fix <a href="https://redirect.github.com/faisalman/ua-parser-js/issues/601">#601</a> - Detect Chrome OS without version</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/c9d1ab95610a9754859ff97c7fda76694f3f76ea"><code>c9d1ab9</code></a> Merge branch 'develop'</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/f815ca6e9cabce4099103b21423d7a9c4531c57a"><code>f815ca6</code></a> Fix <a href="https://redirect.github.com/faisalman/ua-parser-js/issues/620">#620</a> - Add new Device: Kobo</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/0cbeb7a82966aac71e7cadb4794669dabd339868"><code>0cbeb7a</code></a> Rearrange the recently added smarttv detection</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/bf4fb916ca6586c70076a31dd44369d56c44a9e8"><code>bf4fb91</code></a> Merge pull request <a href="https://redirect.github.com/faisalman/ua-parser-js/issues/618">#618</a> from garritfra/smarttv</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/68447d883afc9cdc03e32aad610f4296563c9a5c"><code>68447d8</code></a> Merge branch 'develop' of github.com:faisalman/ua-parser-js into develop</li>
<li>Additional commits viewable in <a href="https://github.com/faisalman/ua-parser-js/compare/0.7.28...0.7.34">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ua-parser-js&package-manager=npm_and_yarn&previous-version=0.7.28&new-version=0.7.34)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-10 07:09:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel-samples/pull/10" class=".btn">#10</a>
            </td>
            <td>
                <b>
                    Bump minimist from 1.2.5 to 1.2.8 in /images/doorman/website
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [minimist](https://github.com/minimistjs/minimist) from 1.2.5 to 1.2.8.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/minimistjs/minimist/blob/main/CHANGELOG.md">minimist's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/minimistjs/minimist/compare/v1.2.7...v1.2.8">v1.2.8</a> - 2023-02-09</h2>
<h3>Merged</h3>
<ul>
<li>[Fix] Fix long option followed by single dash <a href="https://redirect.github.com/minimistjs/minimist/pull/17"><code>[#17](https://github.com/minimistjs/minimist/issues/17)</code></a></li>
<li>[Tests] Remove duplicate test <a href="https://redirect.github.com/minimistjs/minimist/pull/12"><code>[#12](https://github.com/minimistjs/minimist/issues/12)</code></a></li>
<li>[Fix] opt.string works with multiple aliases <a href="https://redirect.github.com/minimistjs/minimist/pull/10"><code>[#10](https://github.com/minimistjs/minimist/issues/10)</code></a></li>
</ul>
<h3>Fixed</h3>
<ul>
<li>[Fix] Fix long option followed by single dash (<a href="https://redirect.github.com/minimistjs/minimist/issues/17">#17</a>) <a href="https://redirect.github.com/minimistjs/minimist/issues/15"><code>[#15](https://github.com/minimistjs/minimist/issues/15)</code></a></li>
<li>[Tests] Remove duplicate test (<a href="https://redirect.github.com/minimistjs/minimist/issues/12">#12</a>) <a href="https://redirect.github.com/minimistjs/minimist/issues/8"><code>[#8](https://github.com/minimistjs/minimist/issues/8)</code></a></li>
<li>[Fix] Fix long option followed by single dash <a href="https://redirect.github.com/minimistjs/minimist/issues/15"><code>[#15](https://github.com/minimistjs/minimist/issues/15)</code></a></li>
<li>[Fix] opt.string works with multiple aliases (<a href="https://redirect.github.com/minimistjs/minimist/issues/10">#10</a>) <a href="https://redirect.github.com/minimistjs/minimist/issues/9"><code>[#9](https://github.com/minimistjs/minimist/issues/9)</code></a></li>
<li>[Fix] Fix handling of short option with non-trivial equals <a href="https://redirect.github.com/minimistjs/minimist/issues/5"><code>[#5](https://github.com/minimistjs/minimist/issues/5)</code></a></li>
<li>[Tests] Remove duplicate test <a href="https://redirect.github.com/minimistjs/minimist/issues/8"><code>[#8](https://github.com/minimistjs/minimist/issues/8)</code></a></li>
<li>[Fix] opt.string works with multiple aliases <a href="https://redirect.github.com/minimistjs/minimist/issues/9"><code>[#9](https://github.com/minimistjs/minimist/issues/9)</code></a></li>
</ul>
<h3>Commits</h3>
<ul>
<li>Merge tag 'v0.2.3' <a href="https://github.com/minimistjs/minimist/commit/a0267947c7870fc5847cf2d437fbe33f392767da"><code>a026794</code></a></li>
<li>[eslint] fix indentation and whitespace <a href="https://github.com/minimistjs/minimist/commit/5368ca4147e974138a54cc0dc4cea8f756546b70"><code>5368ca4</code></a></li>
<li>[eslint] fix indentation and whitespace <a href="https://github.com/minimistjs/minimist/commit/e5f5067259ceeaf0b098d14bec910f87e58708c7"><code>e5f5067</code></a></li>
<li>[eslint] more cleanup <a href="https://github.com/minimistjs/minimist/commit/62fde7d935f83417fb046741531a9e2346a36976"><code>62fde7d</code></a></li>
<li>[eslint] more cleanup <a href="https://github.com/minimistjs/minimist/commit/36ac5d0d95e4947d074e5737d94814034ca335d1"><code>36ac5d0</code></a></li>
<li>[meta] add <code>auto-changelog</code> <a href="https://github.com/minimistjs/minimist/commit/73923d223553fca08b1ba77e3fbc2a492862ae4c"><code>73923d2</code></a></li>
<li>[actions] add reusable workflows <a href="https://github.com/minimistjs/minimist/commit/d80727df77bfa9e631044d7f16368d8f09242c91"><code>d80727d</code></a></li>
<li>[eslint] add eslint; rules to enable later are warnings <a href="https://github.com/minimistjs/minimist/commit/48bc06a1b41f00e9cdf183db34f7a51ba70e98d4"><code>48bc06a</code></a></li>
<li>[eslint] fix indentation <a href="https://github.com/minimistjs/minimist/commit/34b0f1ccaa45183c3c4f06a91f9b405180a6f982"><code>34b0f1c</code></a></li>
<li>[readme] rename and add badges <a href="https://github.com/minimistjs/minimist/commit/5df0fe49211bd09a3636f8686a7cb3012c3e98f0"><code>5df0fe4</code></a></li>
<li>[Dev Deps] switch from <code>covert</code> to <code>nyc</code> <a href="https://github.com/minimistjs/minimist/commit/a48b128fdb8d427dfb20a15273f83e38d97bef07"><code>a48b128</code></a></li>
<li>[Dev Deps] update <code>covert</code>, <code>tape</code>; remove unnecessary <code>tap</code> <a href="https://github.com/minimistjs/minimist/commit/f0fb958e9a1fe980cdffc436a211b0bda58f621b"><code>f0fb958</code></a></li>
<li>[meta] create FUNDING.yml; add <code>funding</code> in package.json <a href="https://github.com/minimistjs/minimist/commit/3639e0c819359a366387e425ab6eabf4c78d3caa"><code>3639e0c</code></a></li>
<li>[meta] use <code>npmignore</code> to autogenerate an npmignore file <a href="https://github.com/minimistjs/minimist/commit/be2e038c342d8333b32f0fde67a0026b79c8150e"><code>be2e038</code></a></li>
<li>Only apps should have lockfiles <a href="https://github.com/minimistjs/minimist/commit/282b570e7489d01b03f2d6d3dabf79cd3e5f84cf"><code>282b570</code></a></li>
<li>isConstructorOrProto adapted from PR <a href="https://github.com/minimistjs/minimist/commit/ef9153fc52b6cea0744b2239921c5dcae4697f11"><code>ef9153f</code></a></li>
<li>[Dev Deps] update <code>@ljharb/eslint-config</code>, <code>aud</code> <a href="https://github.com/minimistjs/minimist/commit/098873c213cdb7c92e55ae1ef5aa1af3a8192a79"><code>098873c</code></a></li>
<li>[Dev Deps] update <code>@ljharb/eslint-config</code>, <code>aud</code> <a href="https://github.com/minimistjs/minimist/commit/3124ed3e46306301ebb3c834874ce0241555c2c4"><code>3124ed3</code></a></li>
<li>[meta] add <code>safe-publish-latest</code> <a href="https://github.com/minimistjs/minimist/commit/4b927de696d561c636b4f43bf49d4597cb36d6d6"><code>4b927de</code></a></li>
<li>[Tests] add <code>aud</code> in <code>posttest</code> <a href="https://github.com/minimistjs/minimist/commit/b32d9bd0ab340f4e9f8c3a97ff2a4424f25fab8c"><code>b32d9bd</code></a></li>
<li>[meta] update repo URLs <a href="https://github.com/minimistjs/minimist/commit/f9fdfc032c54884d9a9996a390c63cd0719bbe1a"><code>f9fdfc0</code></a></li>
<li>[actions] Avoid 0.6 tests due to build failures <a href="https://github.com/minimistjs/minimist/commit/ba92fe6ebbdc0431cca9a2ea8f27beb492f5e4ec"><code>ba92fe6</code></a></li>
<li>[Dev Deps] update <code>tape</code> <a href="https://github.com/minimistjs/minimist/commit/950eaa74f112e04d23e9c606c67472c46739b473"><code>950eaa7</code></a></li>
<li>[Dev Deps] add missing <code>npmignore</code> dev dep <a href="https://github.com/minimistjs/minimist/commit/3226afaf09e9d127ca369742437fe6e88f752d6b"><code>3226afa</code></a></li>
<li>Merge tag 'v0.2.2' <a href="https://github.com/minimistjs/minimist/commit/980d7ac61a0b4bd552711251ac107d506b23e41f"><code>980d7ac</code></a></li>
</ul>
<h2><a href="https://github.com/minimistjs/minimist/compare/v1.2.6...v1.2.7">v1.2.7</a> - 2022-10-10</h2>
<h3>Commits</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/minimistjs/minimist/commit/6901ee286bc4c16da6830b48b46ce1574703cea1"><code>6901ee2</code></a> v1.2.8</li>
<li><a href="https://github.com/minimistjs/minimist/commit/a0267947c7870fc5847cf2d437fbe33f392767da"><code>a026794</code></a> Merge tag 'v0.2.3'</li>
<li><a href="https://github.com/minimistjs/minimist/commit/c0b26618322e94adea26c68e613ef0be482c6c63"><code>c0b2661</code></a> v0.2.3</li>
<li><a href="https://github.com/minimistjs/minimist/commit/63b8fee87b8e7a003216d5d77ba5d6decf3cfb0d"><code>63b8fee</code></a> [Fix] Fix long option followed by single dash (<a href="https://redirect.github.com/minimistjs/minimist/issues/17">#17</a>)</li>
<li><a href="https://github.com/minimistjs/minimist/commit/72239e6f0ea77d8be0ad4f682b7ae7d142144395"><code>72239e6</code></a> [Tests] Remove duplicate test (<a href="https://redirect.github.com/minimistjs/minimist/issues/12">#12</a>)</li>
<li><a href="https://github.com/minimistjs/minimist/commit/34b0f1ccaa45183c3c4f06a91f9b405180a6f982"><code>34b0f1c</code></a> [eslint] fix indentation</li>
<li><a href="https://github.com/minimistjs/minimist/commit/3226afaf09e9d127ca369742437fe6e88f752d6b"><code>3226afa</code></a> [Dev Deps] add missing <code>npmignore</code> dev dep</li>
<li><a href="https://github.com/minimistjs/minimist/commit/098873c213cdb7c92e55ae1ef5aa1af3a8192a79"><code>098873c</code></a> [Dev Deps] update <code>@ljharb/eslint-config</code>, <code>aud</code></li>
<li><a href="https://github.com/minimistjs/minimist/commit/9ec4d279ced72ea2f60237218e71cc03aa0dfdd6"><code>9ec4d27</code></a> [Fix] Fix long option followed by single dash</li>
<li><a href="https://github.com/minimistjs/minimist/commit/ba92fe6ebbdc0431cca9a2ea8f27beb492f5e4ec"><code>ba92fe6</code></a> [actions] Avoid 0.6 tests due to build failures</li>
<li>Additional commits viewable in <a href="https://github.com/minimistjs/minimist/compare/v1.2.5...v1.2.8">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~ljharb">ljharb</a>, a new releaser for minimist since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=minimist&package-manager=npm_and_yarn&previous-version=1.2.5&new-version=1.2.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-10 07:09:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel-samples/pull/9" class=".btn">#9</a>
            </td>
            <td>
                <b>
                    Bump vertx-web from 3.7.1 to 3.9.4 in /images/networkmap
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">java</span>
            </td>
            <td>
                Bumps vertx-web from 3.7.1 to 3.9.4.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=io.vertx:vertx-web&package-manager=maven&previous-version=3.7.1&new-version=3.9.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-10 07:09:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel-samples/pull/8" class=".btn">#8</a>
            </td>
            <td>
                <b>
                    Bump postcss and stylus-brunch in /platforms/r3-corda/images/doorman/website
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [postcss](https://github.com/postcss/postcss) to 7.0.39 and updates ancestor dependency [stylus-brunch](https://github.com/brunch/stylus-brunch). These dependencies need to be updated together.

Updates `postcss` from 5.0.21 to 7.0.39
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/postcss/postcss/releases">postcss's releases</a>.</em></p>
<blockquote>
<h2>7.0.39</h2>
<ul>
<li>Reduce package size.</li>
<li>Backport <code>nanocolors</code> to <code>picocolors</code> migration.</li>
</ul>
<h2>7.0.38</h2>
<ul>
<li>Update <code>Processor#version</code>.</li>
</ul>
<h2>7.0.37</h2>
<ul>
<li>Backport <code>chalk</code> to <code>nanocolors</code> migration.</li>
</ul>
<h2>7.0.36</h2>
<ul>
<li>Backport ReDoS vulnerabilities from PostCSS 8.</li>
</ul>
<h2>7.0.35</h2>
<ul>
<li>Add <a href="https://github.com/postcss/postcss/wiki/PostCSS-8-for-end-users">migration guide link</a> to PostCSS 8 error text.</li>
</ul>
<h2>7.0.34</h2>
<ul>
<li>Fix compatibility with <code>postcss-scss</code> 2.</li>
</ul>
<h2>7.0.33</h2>
<ul>
<li>Add error message for PostCSS 8 plugins.</li>
</ul>
<h2>7.0.32</h2>
<ul>
<li>Fix error message (by <a href="https://github.com/admosity"><code>@​admosity</code></a>).</li>
</ul>
<h2>7.0.31</h2>
<ul>
<li>Use only the latest source map annotation (by <a href="https://github.com/emzoumpo"><code>@​emzoumpo</code></a>).</li>
</ul>
<h2>7.0.30</h2>
<ul>
<li>Fix TypeScript definition (by <a href="https://github.com/nex3"><code>@​nex3</code></a>)</li>
</ul>
<h2>7.0.29</h2>
<ul>
<li>Update <code>Processor#version</code>.</li>
</ul>
<h2>7.0.28</h2>
<ul>
<li>Fix TypeScript definition (by <a href="https://github.com/nex3"><code>@​nex3</code></a>).</li>
</ul>
<h2>7.0.27</h2>
<ul>
<li>Fix TypeScript definition (by <a href="https://github.com/nex3"><code>@​nex3</code></a>).</li>
</ul>
<h2>7.0.26</h2>
<ul>
<li>Fix TypeScript definition (by <a href="https://github.com/nex3"><code>@​nex3</code></a>)</li>
</ul>
<h2>7.0.25</h2>
<ul>
<li>Fix absolute path support for Windows (by <a href="https://github.com/tomrav"><code>@​tomrav</code></a>)</li>
</ul>
<h2>7.0.24</h2>
<ul>
<li>Fix TypeScript definition (by <a href="https://github.com/keithamus"><code>@​keithamus</code></a>).</li>
</ul>
<h2>7.0.23</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/postcss/postcss/blob/7.0.39/CHANGELOG.md">postcss's changelog</a>.</em></p>
<blockquote>
<h2>7.0.39</h2>
<ul>
<li>Reduce package size.</li>
<li>Backport <code>nanocolors</code> to <code>picocolors</code> migration.</li>
</ul>
<h2>7.0.38</h2>
<ul>
<li>Update <code>Processor#version</code>.</li>
</ul>
<h2>7.0.37</h2>
<ul>
<li>Backport <code>chalk</code> to <code>nanocolors</code> migration.</li>
</ul>
<h2>7.0.36</h2>
<ul>
<li>Backport ReDoS vulnerabilities from PostCSS 8.</li>
</ul>
<h2>7.0.35</h2>
<ul>
<li>Add migration guide link to PostCSS 8 error text.</li>
</ul>
<h2>7.0.34</h2>
<ul>
<li>Fix compatibility with <code>postcss-scss</code> 2.</li>
</ul>
<h2>7.0.33</h2>
<ul>
<li>Add error message for PostCSS 8 plugins.</li>
</ul>
<h2>7.0.32</h2>
<ul>
<li>Fix error message (by <a href="https://github.com/admosity"><code>@​admosity</code></a>).</li>
</ul>
<h2>7.0.31</h2>
<ul>
<li>Use only the latest source map annotation (by Emmanouil Zoumpoulakis).</li>
</ul>
<h2>7.0.30</h2>
<ul>
<li>Fix TypeScript definition (by Natalie Weizenbaum).</li>
</ul>
<h2>7.0.29</h2>
<ul>
<li>Update <code>Processor#version</code>.</li>
</ul>
<h2>7.0.28</h2>
<ul>
<li>Fix TypeScript definition (by Natalie Weizenbaum).</li>
</ul>
<h2>7.0.27</h2>
<ul>
<li>Fix TypeScript definition (by Natalie Weizenbaum).</li>
</ul>
<h2>7.0.26</h2>
<ul>
<li>Fix TypeScript definition (by Natalie Weizenbaum).</li>
</ul>
<h2>7.0.25</h2>
<ul>
<li>Fix absolute path support for Windows (by Tom Raviv).</li>
</ul>
<h2>7.0.24</h2>
<ul>
<li>Fix TypeScript definition (by Keith Cirkel).</li>
</ul>
<h2>7.0.23</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/postcss/postcss/commit/e17c1ef7623a71be5732432ca8499bc9928aa08d"><code>e17c1ef</code></a> Release 7.0.39 version</li>
<li><a href="https://github.com/postcss/postcss/commit/6791bd3d5f7ab27ad36dc075033a5beb4bdbfe9e"><code>6791bd3</code></a> Reduce npm package</li>
<li><a href="https://github.com/postcss/postcss/commit/44c581a55a9aab339ee319aa67c264b02c4a6448"><code>44c581a</code></a> Replace nanocolors with picocolors</li>
<li><a href="https://github.com/postcss/postcss/commit/8ba21fd8f4c3bff146b8a71d2d12f31435444394"><code>8ba21fd</code></a> Remove eslint-ci</li>
<li><a href="https://github.com/postcss/postcss/commit/3994c4aa3ce1835c9b36ae17ab94e45c21b56fb2"><code>3994c4a</code></a> Release 7.0.38 version</li>
<li><a href="https://github.com/postcss/postcss/commit/6944e1dd808da66cee4ebf287c66c6aa0fc5c2a0"><code>6944e1d</code></a> Remove development keys from package.json</li>
<li><a href="https://github.com/postcss/postcss/commit/4dd0af024a915bd12d2d53990c5a4fa4129563d5"><code>4dd0af0</code></a> Release 7.0.37 version</li>
<li><a href="https://github.com/postcss/postcss/commit/8408eb4105755c43dbf09a000fd2f1308f240232"><code>8408eb4</code></a> Add compilation step</li>
<li><a href="https://github.com/postcss/postcss/commit/0c680639c3d717b4c8c0b2b2a9d1799fbf239a76"><code>0c68063</code></a> Move tests to GitHub Actions</li>
<li><a href="https://github.com/postcss/postcss/commit/98b61ba5b46622de48bb2592583757ab846212ad"><code>98b61ba</code></a> Replace chalk to nanocolors</li>
<li>Additional commits viewable in <a href="https://github.com/postcss/postcss/compare/5.0.21...7.0.39">compare view</a></li>
</ul>
</details>
<br />

Updates `stylus-brunch` from 2.10.0 to 3.0.0
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/brunch/stylus-brunch/commit/006560182f404e6dae1a81b0e4a0a93111d124a3"><code>0065601</code></a> Release 3.0.0.</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/72ddf4e58abe0651e05b54db5ef94fbe18d3d02e"><code>72ddf4e</code></a> Updates.</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/5d33bd456a94763b554f18cdb12a6181caa75142"><code>5d33bd4</code></a> Updates.</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/4f1836b6c01e92a17e3c4d896ffa5c928b343d0c"><code>4f1836b</code></a> Reorganize for brunch 3.</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/17c771ce42730660ae114f2af37d44684126d108"><code>17c771c</code></a> Release 2.10.1.</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/ced960d9d9e3438185f1a192800a49d23948f824"><code>ced960d</code></a> Merge pull request <a href="https://redirect.github.com/brunch/stylus-brunch/issues/65">#65</a> from brunch/target-extension</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/90e050ebd6ffc1f5c51f881844792c077b9a58a0"><code>90e050e</code></a> Bring back nib.</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/98265a87bbdeb1e1a4a171b06419552896b907b0"><code>98265a8</code></a> Bring back nib.</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/eba579f91968e7e0ed3530b5d9548b8a5ae0915b"><code>eba579f</code></a> Include CSS by default</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/f7935f34b1c3579ac363b4dccb4812d448b72bdf"><code>f7935f3</code></a> Update index.js</li>
<li>Additional commits viewable in <a href="https://github.com/brunch/stylus-brunch/compare/2.10.0...3.0.0">compare view</a></li>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-10 07:04:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel-samples/pull/7" class=".btn">#7</a>
            </td>
            <td>
                <b>
                    Bump ua-parser-js from 0.7.31 to 0.7.34 in /platforms/r3-corda/images/networkmap/website
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [ua-parser-js](https://github.com/faisalman/ua-parser-js) from 0.7.31 to 0.7.34.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/faisalman/ua-parser-js/blob/0.7.34/changelog.md">ua-parser-js's changelog</a>.</em></p>
<blockquote>
<h2>Version 0.7.34 / 1.0.34</h2>
<ul>
<li>Fix Sharp Mobile detected as Huawei Tablet</li>
<li>Fix IE8 bug</li>
<li>Add new devices : Kobo e-Reader, Apple Watch, and some new SmartTV devices</li>
<li>Add new OS : watchOS</li>
<li>Improve browser detection : Kakao, Naver, Brave</li>
<li>Improve device detection : Oculus, iPad</li>
<li>Improve OS detection : Chrome OS</li>
<li>Using navigator.userAgentData as fallback for device.type &amp; os.name</li>
</ul>
<h2>Version 0.7.33 / 1.0.33</h2>
<ul>
<li>Add new browser : Cobalt</li>
<li>Identify Macintosh as an Apple device</li>
<li>Fix ReDoS vulnerability</li>
</ul>
<h2>Version 0.7.32 / 1.0.32</h2>
<ul>
<li>Add new browser : DuckDuckGo, Huawei Browser, LinkedIn</li>
<li>Add new OS : HarmonyOS</li>
<li>Add some Huawei models</li>
<li>Add Sharp Aquos TV</li>
<li>Improve detection Xiaomi Mi CC9</li>
<li>Fix Sony Xperia 1 III misidentified as Acer tablet</li>
<li>Fix Detect Sony BRAVIA as SmartTV</li>
<li>Fix Detect Xiaomi Mi TV as SmartTV</li>
<li>Fix Detect Galaxy Tab S8 as tablet</li>
<li>Fix WeGame mistakenly identified as WeChat</li>
<li>Fix included commas in Safari / Mobile Safari version</li>
<li>Increase UA_MAX_LENGTH to 350</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/3218051f0739a4a7990b06210983917a11da7904"><code>3218051</code></a> Bump version 0.7.34</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/551ad8847403b82f06c8a834d946d7c6ade6e9ad"><code>551ad88</code></a> Add new device: Apple Watch, new os: watchOS</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/097f736c4d6913312880810d8452b775ec2fa020"><code>097f736</code></a> Fix <a href="https://redirect.github.com/faisalman/ua-parser-js/issues/387">#387</a> <a href="https://redirect.github.com/faisalman/ua-parser-js/issues/554">#554</a> - Detect iPadOS 13</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/73c25771dcd152d415bedb5c0569bc06f6ff65f2"><code>73c2577</code></a> Fix <a href="https://redirect.github.com/faisalman/ua-parser-js/issues/498">#498</a> - Detect Brave Browser by checking navigator.brave</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/f8e5a1fb4fbe55b781a48d7d141fdc41ba93fa38"><code>f8e5a1f</code></a> Fix <a href="https://redirect.github.com/faisalman/ua-parser-js/issues/601">#601</a> - Detect Chrome OS without version</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/c9d1ab95610a9754859ff97c7fda76694f3f76ea"><code>c9d1ab9</code></a> Merge branch 'develop'</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/f815ca6e9cabce4099103b21423d7a9c4531c57a"><code>f815ca6</code></a> Fix <a href="https://redirect.github.com/faisalman/ua-parser-js/issues/620">#620</a> - Add new Device: Kobo</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/0cbeb7a82966aac71e7cadb4794669dabd339868"><code>0cbeb7a</code></a> Rearrange the recently added smarttv detection</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/bf4fb916ca6586c70076a31dd44369d56c44a9e8"><code>bf4fb91</code></a> Merge pull request <a href="https://redirect.github.com/faisalman/ua-parser-js/issues/618">#618</a> from garritfra/smarttv</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/68447d883afc9cdc03e32aad610f4296563c9a5c"><code>68447d8</code></a> Merge branch 'develop' of github.com:faisalman/ua-parser-js into develop</li>
<li>Additional commits viewable in <a href="https://github.com/faisalman/ua-parser-js/compare/0.7.31...0.7.34">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ua-parser-js&package-manager=npm_and_yarn&previous-version=0.7.31&new-version=0.7.34)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-10 07:04:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel-samples/pull/6" class=".btn">#6</a>
            </td>
            <td>
                <b>
                    Bump minimist from 1.2.5 to 1.2.8 in /platforms/r3-corda/images/doorman/website
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [minimist](https://github.com/minimistjs/minimist) from 1.2.5 to 1.2.8.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/minimistjs/minimist/blob/main/CHANGELOG.md">minimist's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/minimistjs/minimist/compare/v1.2.7...v1.2.8">v1.2.8</a> - 2023-02-09</h2>
<h3>Merged</h3>
<ul>
<li>[Fix] Fix long option followed by single dash <a href="https://redirect.github.com/minimistjs/minimist/pull/17"><code>[#17](https://github.com/minimistjs/minimist/issues/17)</code></a></li>
<li>[Tests] Remove duplicate test <a href="https://redirect.github.com/minimistjs/minimist/pull/12"><code>[#12](https://github.com/minimistjs/minimist/issues/12)</code></a></li>
<li>[Fix] opt.string works with multiple aliases <a href="https://redirect.github.com/minimistjs/minimist/pull/10"><code>[#10](https://github.com/minimistjs/minimist/issues/10)</code></a></li>
</ul>
<h3>Fixed</h3>
<ul>
<li>[Fix] Fix long option followed by single dash (<a href="https://redirect.github.com/minimistjs/minimist/issues/17">#17</a>) <a href="https://redirect.github.com/minimistjs/minimist/issues/15"><code>[#15](https://github.com/minimistjs/minimist/issues/15)</code></a></li>
<li>[Tests] Remove duplicate test (<a href="https://redirect.github.com/minimistjs/minimist/issues/12">#12</a>) <a href="https://redirect.github.com/minimistjs/minimist/issues/8"><code>[#8](https://github.com/minimistjs/minimist/issues/8)</code></a></li>
<li>[Fix] Fix long option followed by single dash <a href="https://redirect.github.com/minimistjs/minimist/issues/15"><code>[#15](https://github.com/minimistjs/minimist/issues/15)</code></a></li>
<li>[Fix] opt.string works with multiple aliases (<a href="https://redirect.github.com/minimistjs/minimist/issues/10">#10</a>) <a href="https://redirect.github.com/minimistjs/minimist/issues/9"><code>[#9](https://github.com/minimistjs/minimist/issues/9)</code></a></li>
<li>[Fix] Fix handling of short option with non-trivial equals <a href="https://redirect.github.com/minimistjs/minimist/issues/5"><code>[#5](https://github.com/minimistjs/minimist/issues/5)</code></a></li>
<li>[Tests] Remove duplicate test <a href="https://redirect.github.com/minimistjs/minimist/issues/8"><code>[#8](https://github.com/minimistjs/minimist/issues/8)</code></a></li>
<li>[Fix] opt.string works with multiple aliases <a href="https://redirect.github.com/minimistjs/minimist/issues/9"><code>[#9](https://github.com/minimistjs/minimist/issues/9)</code></a></li>
</ul>
<h3>Commits</h3>
<ul>
<li>Merge tag 'v0.2.3' <a href="https://github.com/minimistjs/minimist/commit/a0267947c7870fc5847cf2d437fbe33f392767da"><code>a026794</code></a></li>
<li>[eslint] fix indentation and whitespace <a href="https://github.com/minimistjs/minimist/commit/5368ca4147e974138a54cc0dc4cea8f756546b70"><code>5368ca4</code></a></li>
<li>[eslint] fix indentation and whitespace <a href="https://github.com/minimistjs/minimist/commit/e5f5067259ceeaf0b098d14bec910f87e58708c7"><code>e5f5067</code></a></li>
<li>[eslint] more cleanup <a href="https://github.com/minimistjs/minimist/commit/62fde7d935f83417fb046741531a9e2346a36976"><code>62fde7d</code></a></li>
<li>[eslint] more cleanup <a href="https://github.com/minimistjs/minimist/commit/36ac5d0d95e4947d074e5737d94814034ca335d1"><code>36ac5d0</code></a></li>
<li>[meta] add <code>auto-changelog</code> <a href="https://github.com/minimistjs/minimist/commit/73923d223553fca08b1ba77e3fbc2a492862ae4c"><code>73923d2</code></a></li>
<li>[actions] add reusable workflows <a href="https://github.com/minimistjs/minimist/commit/d80727df77bfa9e631044d7f16368d8f09242c91"><code>d80727d</code></a></li>
<li>[eslint] add eslint; rules to enable later are warnings <a href="https://github.com/minimistjs/minimist/commit/48bc06a1b41f00e9cdf183db34f7a51ba70e98d4"><code>48bc06a</code></a></li>
<li>[eslint] fix indentation <a href="https://github.com/minimistjs/minimist/commit/34b0f1ccaa45183c3c4f06a91f9b405180a6f982"><code>34b0f1c</code></a></li>
<li>[readme] rename and add badges <a href="https://github.com/minimistjs/minimist/commit/5df0fe49211bd09a3636f8686a7cb3012c3e98f0"><code>5df0fe4</code></a></li>
<li>[Dev Deps] switch from <code>covert</code> to <code>nyc</code> <a href="https://github.com/minimistjs/minimist/commit/a48b128fdb8d427dfb20a15273f83e38d97bef07"><code>a48b128</code></a></li>
<li>[Dev Deps] update <code>covert</code>, <code>tape</code>; remove unnecessary <code>tap</code> <a href="https://github.com/minimistjs/minimist/commit/f0fb958e9a1fe980cdffc436a211b0bda58f621b"><code>f0fb958</code></a></li>
<li>[meta] create FUNDING.yml; add <code>funding</code> in package.json <a href="https://github.com/minimistjs/minimist/commit/3639e0c819359a366387e425ab6eabf4c78d3caa"><code>3639e0c</code></a></li>
<li>[meta] use <code>npmignore</code> to autogenerate an npmignore file <a href="https://github.com/minimistjs/minimist/commit/be2e038c342d8333b32f0fde67a0026b79c8150e"><code>be2e038</code></a></li>
<li>Only apps should have lockfiles <a href="https://github.com/minimistjs/minimist/commit/282b570e7489d01b03f2d6d3dabf79cd3e5f84cf"><code>282b570</code></a></li>
<li>isConstructorOrProto adapted from PR <a href="https://github.com/minimistjs/minimist/commit/ef9153fc52b6cea0744b2239921c5dcae4697f11"><code>ef9153f</code></a></li>
<li>[Dev Deps] update <code>@ljharb/eslint-config</code>, <code>aud</code> <a href="https://github.com/minimistjs/minimist/commit/098873c213cdb7c92e55ae1ef5aa1af3a8192a79"><code>098873c</code></a></li>
<li>[Dev Deps] update <code>@ljharb/eslint-config</code>, <code>aud</code> <a href="https://github.com/minimistjs/minimist/commit/3124ed3e46306301ebb3c834874ce0241555c2c4"><code>3124ed3</code></a></li>
<li>[meta] add <code>safe-publish-latest</code> <a href="https://github.com/minimistjs/minimist/commit/4b927de696d561c636b4f43bf49d4597cb36d6d6"><code>4b927de</code></a></li>
<li>[Tests] add <code>aud</code> in <code>posttest</code> <a href="https://github.com/minimistjs/minimist/commit/b32d9bd0ab340f4e9f8c3a97ff2a4424f25fab8c"><code>b32d9bd</code></a></li>
<li>[meta] update repo URLs <a href="https://github.com/minimistjs/minimist/commit/f9fdfc032c54884d9a9996a390c63cd0719bbe1a"><code>f9fdfc0</code></a></li>
<li>[actions] Avoid 0.6 tests due to build failures <a href="https://github.com/minimistjs/minimist/commit/ba92fe6ebbdc0431cca9a2ea8f27beb492f5e4ec"><code>ba92fe6</code></a></li>
<li>[Dev Deps] update <code>tape</code> <a href="https://github.com/minimistjs/minimist/commit/950eaa74f112e04d23e9c606c67472c46739b473"><code>950eaa7</code></a></li>
<li>[Dev Deps] add missing <code>npmignore</code> dev dep <a href="https://github.com/minimistjs/minimist/commit/3226afaf09e9d127ca369742437fe6e88f752d6b"><code>3226afa</code></a></li>
<li>Merge tag 'v0.2.2' <a href="https://github.com/minimistjs/minimist/commit/980d7ac61a0b4bd552711251ac107d506b23e41f"><code>980d7ac</code></a></li>
</ul>
<h2><a href="https://github.com/minimistjs/minimist/compare/v1.2.6...v1.2.7">v1.2.7</a> - 2022-10-10</h2>
<h3>Commits</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/minimistjs/minimist/commit/6901ee286bc4c16da6830b48b46ce1574703cea1"><code>6901ee2</code></a> v1.2.8</li>
<li><a href="https://github.com/minimistjs/minimist/commit/a0267947c7870fc5847cf2d437fbe33f392767da"><code>a026794</code></a> Merge tag 'v0.2.3'</li>
<li><a href="https://github.com/minimistjs/minimist/commit/c0b26618322e94adea26c68e613ef0be482c6c63"><code>c0b2661</code></a> v0.2.3</li>
<li><a href="https://github.com/minimistjs/minimist/commit/63b8fee87b8e7a003216d5d77ba5d6decf3cfb0d"><code>63b8fee</code></a> [Fix] Fix long option followed by single dash (<a href="https://redirect.github.com/minimistjs/minimist/issues/17">#17</a>)</li>
<li><a href="https://github.com/minimistjs/minimist/commit/72239e6f0ea77d8be0ad4f682b7ae7d142144395"><code>72239e6</code></a> [Tests] Remove duplicate test (<a href="https://redirect.github.com/minimistjs/minimist/issues/12">#12</a>)</li>
<li><a href="https://github.com/minimistjs/minimist/commit/34b0f1ccaa45183c3c4f06a91f9b405180a6f982"><code>34b0f1c</code></a> [eslint] fix indentation</li>
<li><a href="https://github.com/minimistjs/minimist/commit/3226afaf09e9d127ca369742437fe6e88f752d6b"><code>3226afa</code></a> [Dev Deps] add missing <code>npmignore</code> dev dep</li>
<li><a href="https://github.com/minimistjs/minimist/commit/098873c213cdb7c92e55ae1ef5aa1af3a8192a79"><code>098873c</code></a> [Dev Deps] update <code>@ljharb/eslint-config</code>, <code>aud</code></li>
<li><a href="https://github.com/minimistjs/minimist/commit/9ec4d279ced72ea2f60237218e71cc03aa0dfdd6"><code>9ec4d27</code></a> [Fix] Fix long option followed by single dash</li>
<li><a href="https://github.com/minimistjs/minimist/commit/ba92fe6ebbdc0431cca9a2ea8f27beb492f5e4ec"><code>ba92fe6</code></a> [actions] Avoid 0.6 tests due to build failures</li>
<li>Additional commits viewable in <a href="https://github.com/minimistjs/minimist/compare/v1.2.5...v1.2.8">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~ljharb">ljharb</a>, a new releaser for minimist since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=minimist&package-manager=npm_and_yarn&previous-version=1.2.5&new-version=1.2.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-10 07:04:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel-samples/pull/5" class=".btn">#5</a>
            </td>
            <td>
                <b>
                    Bump postcss and stylus-brunch in /platforms/r3-corda/images/networkmap/website
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [postcss](https://github.com/postcss/postcss) to 7.0.39 and updates ancestor dependency [stylus-brunch](https://github.com/brunch/stylus-brunch). These dependencies need to be updated together.

Updates `postcss` from 5.0.21 to 7.0.39
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/postcss/postcss/releases">postcss's releases</a>.</em></p>
<blockquote>
<h2>7.0.39</h2>
<ul>
<li>Reduce package size.</li>
<li>Backport <code>nanocolors</code> to <code>picocolors</code> migration.</li>
</ul>
<h2>7.0.38</h2>
<ul>
<li>Update <code>Processor#version</code>.</li>
</ul>
<h2>7.0.37</h2>
<ul>
<li>Backport <code>chalk</code> to <code>nanocolors</code> migration.</li>
</ul>
<h2>7.0.36</h2>
<ul>
<li>Backport ReDoS vulnerabilities from PostCSS 8.</li>
</ul>
<h2>7.0.35</h2>
<ul>
<li>Add <a href="https://github.com/postcss/postcss/wiki/PostCSS-8-for-end-users">migration guide link</a> to PostCSS 8 error text.</li>
</ul>
<h2>7.0.34</h2>
<ul>
<li>Fix compatibility with <code>postcss-scss</code> 2.</li>
</ul>
<h2>7.0.33</h2>
<ul>
<li>Add error message for PostCSS 8 plugins.</li>
</ul>
<h2>7.0.32</h2>
<ul>
<li>Fix error message (by <a href="https://github.com/admosity"><code>@​admosity</code></a>).</li>
</ul>
<h2>7.0.31</h2>
<ul>
<li>Use only the latest source map annotation (by <a href="https://github.com/emzoumpo"><code>@​emzoumpo</code></a>).</li>
</ul>
<h2>7.0.30</h2>
<ul>
<li>Fix TypeScript definition (by <a href="https://github.com/nex3"><code>@​nex3</code></a>)</li>
</ul>
<h2>7.0.29</h2>
<ul>
<li>Update <code>Processor#version</code>.</li>
</ul>
<h2>7.0.28</h2>
<ul>
<li>Fix TypeScript definition (by <a href="https://github.com/nex3"><code>@​nex3</code></a>).</li>
</ul>
<h2>7.0.27</h2>
<ul>
<li>Fix TypeScript definition (by <a href="https://github.com/nex3"><code>@​nex3</code></a>).</li>
</ul>
<h2>7.0.26</h2>
<ul>
<li>Fix TypeScript definition (by <a href="https://github.com/nex3"><code>@​nex3</code></a>)</li>
</ul>
<h2>7.0.25</h2>
<ul>
<li>Fix absolute path support for Windows (by <a href="https://github.com/tomrav"><code>@​tomrav</code></a>)</li>
</ul>
<h2>7.0.24</h2>
<ul>
<li>Fix TypeScript definition (by <a href="https://github.com/keithamus"><code>@​keithamus</code></a>).</li>
</ul>
<h2>7.0.23</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/postcss/postcss/blob/7.0.39/CHANGELOG.md">postcss's changelog</a>.</em></p>
<blockquote>
<h2>7.0.39</h2>
<ul>
<li>Reduce package size.</li>
<li>Backport <code>nanocolors</code> to <code>picocolors</code> migration.</li>
</ul>
<h2>7.0.38</h2>
<ul>
<li>Update <code>Processor#version</code>.</li>
</ul>
<h2>7.0.37</h2>
<ul>
<li>Backport <code>chalk</code> to <code>nanocolors</code> migration.</li>
</ul>
<h2>7.0.36</h2>
<ul>
<li>Backport ReDoS vulnerabilities from PostCSS 8.</li>
</ul>
<h2>7.0.35</h2>
<ul>
<li>Add migration guide link to PostCSS 8 error text.</li>
</ul>
<h2>7.0.34</h2>
<ul>
<li>Fix compatibility with <code>postcss-scss</code> 2.</li>
</ul>
<h2>7.0.33</h2>
<ul>
<li>Add error message for PostCSS 8 plugins.</li>
</ul>
<h2>7.0.32</h2>
<ul>
<li>Fix error message (by <a href="https://github.com/admosity"><code>@​admosity</code></a>).</li>
</ul>
<h2>7.0.31</h2>
<ul>
<li>Use only the latest source map annotation (by Emmanouil Zoumpoulakis).</li>
</ul>
<h2>7.0.30</h2>
<ul>
<li>Fix TypeScript definition (by Natalie Weizenbaum).</li>
</ul>
<h2>7.0.29</h2>
<ul>
<li>Update <code>Processor#version</code>.</li>
</ul>
<h2>7.0.28</h2>
<ul>
<li>Fix TypeScript definition (by Natalie Weizenbaum).</li>
</ul>
<h2>7.0.27</h2>
<ul>
<li>Fix TypeScript definition (by Natalie Weizenbaum).</li>
</ul>
<h2>7.0.26</h2>
<ul>
<li>Fix TypeScript definition (by Natalie Weizenbaum).</li>
</ul>
<h2>7.0.25</h2>
<ul>
<li>Fix absolute path support for Windows (by Tom Raviv).</li>
</ul>
<h2>7.0.24</h2>
<ul>
<li>Fix TypeScript definition (by Keith Cirkel).</li>
</ul>
<h2>7.0.23</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/postcss/postcss/commit/e17c1ef7623a71be5732432ca8499bc9928aa08d"><code>e17c1ef</code></a> Release 7.0.39 version</li>
<li><a href="https://github.com/postcss/postcss/commit/6791bd3d5f7ab27ad36dc075033a5beb4bdbfe9e"><code>6791bd3</code></a> Reduce npm package</li>
<li><a href="https://github.com/postcss/postcss/commit/44c581a55a9aab339ee319aa67c264b02c4a6448"><code>44c581a</code></a> Replace nanocolors with picocolors</li>
<li><a href="https://github.com/postcss/postcss/commit/8ba21fd8f4c3bff146b8a71d2d12f31435444394"><code>8ba21fd</code></a> Remove eslint-ci</li>
<li><a href="https://github.com/postcss/postcss/commit/3994c4aa3ce1835c9b36ae17ab94e45c21b56fb2"><code>3994c4a</code></a> Release 7.0.38 version</li>
<li><a href="https://github.com/postcss/postcss/commit/6944e1dd808da66cee4ebf287c66c6aa0fc5c2a0"><code>6944e1d</code></a> Remove development keys from package.json</li>
<li><a href="https://github.com/postcss/postcss/commit/4dd0af024a915bd12d2d53990c5a4fa4129563d5"><code>4dd0af0</code></a> Release 7.0.37 version</li>
<li><a href="https://github.com/postcss/postcss/commit/8408eb4105755c43dbf09a000fd2f1308f240232"><code>8408eb4</code></a> Add compilation step</li>
<li><a href="https://github.com/postcss/postcss/commit/0c680639c3d717b4c8c0b2b2a9d1799fbf239a76"><code>0c68063</code></a> Move tests to GitHub Actions</li>
<li><a href="https://github.com/postcss/postcss/commit/98b61ba5b46622de48bb2592583757ab846212ad"><code>98b61ba</code></a> Replace chalk to nanocolors</li>
<li>Additional commits viewable in <a href="https://github.com/postcss/postcss/compare/5.0.21...7.0.39">compare view</a></li>
</ul>
</details>
<br />

Updates `stylus-brunch` from 2.10.0 to 3.0.0
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/brunch/stylus-brunch/commit/006560182f404e6dae1a81b0e4a0a93111d124a3"><code>0065601</code></a> Release 3.0.0.</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/72ddf4e58abe0651e05b54db5ef94fbe18d3d02e"><code>72ddf4e</code></a> Updates.</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/5d33bd456a94763b554f18cdb12a6181caa75142"><code>5d33bd4</code></a> Updates.</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/4f1836b6c01e92a17e3c4d896ffa5c928b343d0c"><code>4f1836b</code></a> Reorganize for brunch 3.</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/17c771ce42730660ae114f2af37d44684126d108"><code>17c771c</code></a> Release 2.10.1.</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/ced960d9d9e3438185f1a192800a49d23948f824"><code>ced960d</code></a> Merge pull request <a href="https://redirect.github.com/brunch/stylus-brunch/issues/65">#65</a> from brunch/target-extension</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/90e050ebd6ffc1f5c51f881844792c077b9a58a0"><code>90e050e</code></a> Bring back nib.</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/98265a87bbdeb1e1a4a171b06419552896b907b0"><code>98265a8</code></a> Bring back nib.</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/eba579f91968e7e0ed3530b5d9548b8a5ae0915b"><code>eba579f</code></a> Include CSS by default</li>
<li><a href="https://github.com/brunch/stylus-brunch/commit/f7935f34b1c3579ac363b4dccb4812d448b72bdf"><code>f7935f3</code></a> Update index.js</li>
<li>Additional commits viewable in <a href="https://github.com/brunch/stylus-brunch/compare/2.10.0...3.0.0">compare view</a></li>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-10 07:04:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel-samples/pull/4" class=".btn">#4</a>
            </td>
            <td>
                <b>
                    Bump ua-parser-js from 0.7.28 to 0.7.34 in /platforms/r3-corda/images/doorman/website
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [ua-parser-js](https://github.com/faisalman/ua-parser-js) from 0.7.28 to 0.7.34.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/faisalman/ua-parser-js/blob/0.7.34/changelog.md">ua-parser-js's changelog</a>.</em></p>
<blockquote>
<h2>Version 0.7.34 / 1.0.34</h2>
<ul>
<li>Fix Sharp Mobile detected as Huawei Tablet</li>
<li>Fix IE8 bug</li>
<li>Add new devices : Kobo e-Reader, Apple Watch, and some new SmartTV devices</li>
<li>Add new OS : watchOS</li>
<li>Improve browser detection : Kakao, Naver, Brave</li>
<li>Improve device detection : Oculus, iPad</li>
<li>Improve OS detection : Chrome OS</li>
<li>Using navigator.userAgentData as fallback for device.type &amp; os.name</li>
</ul>
<h2>Version 0.7.33 / 1.0.33</h2>
<ul>
<li>Add new browser : Cobalt</li>
<li>Identify Macintosh as an Apple device</li>
<li>Fix ReDoS vulnerability</li>
</ul>
<h2>Version 0.7.32 / 1.0.32</h2>
<ul>
<li>Add new browser : DuckDuckGo, Huawei Browser, LinkedIn</li>
<li>Add new OS : HarmonyOS</li>
<li>Add some Huawei models</li>
<li>Add Sharp Aquos TV</li>
<li>Improve detection Xiaomi Mi CC9</li>
<li>Fix Sony Xperia 1 III misidentified as Acer tablet</li>
<li>Fix Detect Sony BRAVIA as SmartTV</li>
<li>Fix Detect Xiaomi Mi TV as SmartTV</li>
<li>Fix Detect Galaxy Tab S8 as tablet</li>
<li>Fix WeGame mistakenly identified as WeChat</li>
<li>Fix included commas in Safari / Mobile Safari version</li>
<li>Increase UA_MAX_LENGTH to 350</li>
</ul>
<h2>Version 0.7.31 / 1.0.2</h2>
<ul>
<li>Fix OPPO Reno A5 incorrect detection</li>
<li>Fix TypeError Bug</li>
<li>Use AST to extract regexes and verify them with safe-regex</li>
</ul>
<h2>Version 0.7.30 / 1.0.1</h2>
<ul>
<li>Add new browser : Obigo, UP.Browser, Klar</li>
<li>Add new device : Oculus, Roku</li>
<li>Add new OS: Maemo, HP-UX, Android-x86, Deepin, elementary OS, GhostBSD, Linspire, Manjaro, Sabayon</li>
<li>Improve detection for Sony Xperia 1ii, LG Android TV, and some more devices</li>
<li>Improve detection for ARM64 CPU</li>
<li>Improve detection for Windows Mobile, Netscape, Mac on PowerPC</li>
<li>Categorize PDA as mobile</li>
<li>Fix Sharp devices misjudged as Huawei</li>
<li>Fix trailing comma for ES3 compatibility</li>
<li>Some code refactor</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/3218051f0739a4a7990b06210983917a11da7904"><code>3218051</code></a> Bump version 0.7.34</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/551ad8847403b82f06c8a834d946d7c6ade6e9ad"><code>551ad88</code></a> Add new device: Apple Watch, new os: watchOS</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/097f736c4d6913312880810d8452b775ec2fa020"><code>097f736</code></a> Fix <a href="https://redirect.github.com/faisalman/ua-parser-js/issues/387">#387</a> <a href="https://redirect.github.com/faisalman/ua-parser-js/issues/554">#554</a> - Detect iPadOS 13</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/73c25771dcd152d415bedb5c0569bc06f6ff65f2"><code>73c2577</code></a> Fix <a href="https://redirect.github.com/faisalman/ua-parser-js/issues/498">#498</a> - Detect Brave Browser by checking navigator.brave</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/f8e5a1fb4fbe55b781a48d7d141fdc41ba93fa38"><code>f8e5a1f</code></a> Fix <a href="https://redirect.github.com/faisalman/ua-parser-js/issues/601">#601</a> - Detect Chrome OS without version</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/c9d1ab95610a9754859ff97c7fda76694f3f76ea"><code>c9d1ab9</code></a> Merge branch 'develop'</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/f815ca6e9cabce4099103b21423d7a9c4531c57a"><code>f815ca6</code></a> Fix <a href="https://redirect.github.com/faisalman/ua-parser-js/issues/620">#620</a> - Add new Device: Kobo</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/0cbeb7a82966aac71e7cadb4794669dabd339868"><code>0cbeb7a</code></a> Rearrange the recently added smarttv detection</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/bf4fb916ca6586c70076a31dd44369d56c44a9e8"><code>bf4fb91</code></a> Merge pull request <a href="https://redirect.github.com/faisalman/ua-parser-js/issues/618">#618</a> from garritfra/smarttv</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/68447d883afc9cdc03e32aad610f4296563c9a5c"><code>68447d8</code></a> Merge branch 'develop' of github.com:faisalman/ua-parser-js into develop</li>
<li>Additional commits viewable in <a href="https://github.com/faisalman/ua-parser-js/compare/0.7.28...0.7.34">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ua-parser-js&package-manager=npm_and_yarn&previous-version=0.7.28&new-version=0.7.34)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-10 07:04:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel-samples/pull/3" class=".btn">#3</a>
            </td>
            <td>
                <b>
                    Bump vertx-web from 3.7.1 to 3.9.4 in /platforms/r3-corda/images/networkmap
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">java</span>
            </td>
            <td>
                Bumps vertx-web from 3.7.1 to 3.9.4.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=io.vertx:vertx-web&package-manager=maven&previous-version=3.7.1&new-version=3.9.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-10 07:04:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel-samples/pull/2" class=".btn">#2</a>
            </td>
            <td>
                <b>
                    Inital commit for bevel-samples -
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Commits from bevel repo
Keeping only reference application and related workflows Corda OS helper images
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-10 07:03:38 +0000 UTC
    </div>
</div>

