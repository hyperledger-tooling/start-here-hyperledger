---
layout: default
title: university-course
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/university-course
---

# university-course <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/university-course){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/university-course/pull/79" class=".btn">#79</a>
            </td>
            <td>
                <b>
                    chore(deps): bump protobufjs from 6.10.1 to 6.11.3 in /support/Lab06/chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [protobufjs](https://github.com/protobufjs/protobuf.js) from 6.10.1 to 6.11.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/protobufjs/protobuf.js/releases">protobufjs's releases</a>.</em></p>
<blockquote>
<h2>v6.11.3</h2>
<h3><a href="https://github.com/protobufjs/protobuf.js/compare/v6.11.2...v6.11.3">6.11.3</a> (2022-05-20)</h3>
<h3>Bug Fixes</h3>
<ul>
<li><strong>deps:</strong> use eslint 8.x (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1728">#1728</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/a8681ceab4763e706a848121a2dde56791b89eea">a8681ce</a>)</li>
<li>do not let setProperty change the prototype (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1731">#1731</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/b5f1391dff5515894830a6570e6d73f5511b2e8f">b5f1391</a>)</li>
</ul>
<h2>v6.11.2</h2>
<h3><a href="https://www.github.com/protobufjs/protobuf.js/compare/v6.11.1...v6.11.2">6.11.2</a> (2021-04-30)</h3>
<ul>
<li>regenerated index.d.ts to fix the unintended breaking change in types.</li>
</ul>
<h2>v6.11.1</h2>
<h3><a href="https://www.github.com/protobufjs/protobuf.js/compare/v6.11.0...v6.11.1">6.11.1</a> (2021-04-29)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>parse.js &quot;parent.add(oneof)“ error (<a href="https://github.com/leon776"><code>@​leon776</code></a>) (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/pull/1602">#1602</a>)</li>
</ul>
<h2>v6.11.0</h2>
<h2><a href="https://www.github.com/protobufjs/protobuf.js/compare/v6.10.2...v6.11.0">6.11.0</a> (2021-04-28)</h2>
<h3>Features</h3>
<ul>
<li>support for proto3 <code>optional</code> fields (<a href="https://github.com/alexander-fenster"><code>@​alexander-fenster</code></a>) (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/pull/1584">#1584</a>)</li>
<li>add <code>--no-service</code> option for <code>pbjs</code> (<a href="https://github.com/mdouglass"><code>@​mdouglass</code></a>) (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/pull/1577">#1577</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>do not assign <code>oneof</code> members to default values, use <code>null</code> instead (<a href="https://github.com/alexander-fenster"><code>@​alexander-fenster</code></a>) (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/pull/1597">#1597</a>)</li>
</ul>
<h3>Dependencies</h3>
<ul>
<li>set <code>@types/node</code> to <code>&gt;= 13.7.0</code> in dependencies (<a href="https://github.com/indutny"><code>@​indutny</code></a>) (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/pull/1575">#1575</a>)</li>
</ul>
<h2>protobuf.js v6.10.2</h2>
<h3>Bug Fixes</h3>
<ul>
<li>es6 export enum (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1446">#1446</a>) (<a href="https://www.github.com/protobufjs/protobuf.js/commit/9f33784350b1efc2e774bbfc087cbd2c47828748">9f33784</a>)</li>
<li>make parsedOptions appear in method JSON representation (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1506">#1506</a>) (<a href="https://www.github.com/protobufjs/protobuf.js/commit/3d29969865f2119550d9dc88391846469da9fa7f">3d29969</a>)</li>
<li>utf8 -&gt; utf16 decoding bug on surrogate pairs (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1486">#1486</a>) (<a href="https://www.github.com/protobufjs/protobuf.js/commit/75172cd11be137bbabd2fba7a02b15067695ebad">75172cd</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/protobufjs/protobuf.js/blob/v6.11.3/CHANGELOG.md">protobufjs's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/protobufjs/protobuf.js/compare/v6.11.2...v6.11.3">6.11.3</a> (2022-05-20)</h3>
<h3>Bug Fixes</h3>
<ul>
<li><strong>deps:</strong> use eslint 8.x (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1728">#1728</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/a8681ceab4763e706a848121a2dde56791b89eea">a8681ce</a>)</li>
<li>do not let setProperty change the prototype (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1731">#1731</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/b5f1391dff5515894830a6570e6d73f5511b2e8f">b5f1391</a>)</li>
</ul>
<h3><a href="https://www.github.com/protobufjs/protobuf.js/compare/v6.11.1...v6.11.2">6.11.2</a> (2021-04-30)</h3>
<ul>
<li>regenerated index.d.ts to fix the unintended breaking change in types.</li>
</ul>
<h3><a href="https://www.github.com/protobufjs/protobuf.js/compare/v6.11.0...v6.11.1">6.11.1</a> (2021-04-29)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>parse.js &quot;parent.add(oneof)“ error (<a href="https://github.com/leon776"><code>@​leon776</code></a>) (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/pull/1602">#1602</a>)</li>
</ul>
<h2><a href="https://www.github.com/protobufjs/protobuf.js/compare/v6.10.2...v6.11.0">6.11.0</a> (2021-04-28)</h2>
<h3>Features</h3>
<ul>
<li>support for proto3 <code>optional</code> fields (<a href="https://github.com/alexander-fenster"><code>@​alexander-fenster</code></a>) (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/pull/1584">#1584</a>)</li>
<li>add <code>--no-service</code> option for <code>pbjs</code> (<a href="https://github.com/mdouglass"><code>@​mdouglass</code></a>) (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/pull/1577">#1577</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>do not assign <code>oneof</code> members to default values, use <code>null</code> instead (<a href="https://github.com/alexander-fenster"><code>@​alexander-fenster</code></a>) (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/pull/1597">#1597</a>)</li>
</ul>
<h3>Dependencies</h3>
<ul>
<li>set <code>@types/node</code> to <code>&gt;= 13.7.0</code> in dependencies (<a href="https://github.com/indutny"><code>@​indutny</code></a>) (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/pull/1575">#1575</a>)</li>
</ul>
<h3><a href="https://www.github.com/protobufjs/protobuf.js/compare/v6.10.1...v6.10.2">6.10.2</a> (2020-11-13)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>es6 export enum (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1446">#1446</a>) (<a href="https://www.github.com/protobufjs/protobuf.js/commit/9f33784350b1efc2e774bbfc087cbd2c47828748">9f33784</a>)</li>
<li>make parsedOptions appear in method JSON representation (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1506">#1506</a>) (<a href="https://www.github.com/protobufjs/protobuf.js/commit/3d29969865f2119550d9dc88391846469da9fa7f">3d29969</a>)</li>
<li>utf8 -&gt; utf16 decoding bug on surrogate pairs (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1486">#1486</a>) (<a href="https://www.github.com/protobufjs/protobuf.js/commit/75172cd11be137bbabd2fba7a02b15067695ebad">75172cd</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/b130dfd4f06b642d4b7c3ccc9f3f9fb6a6e6ed0d"><code>b130dfd</code></a> chore(6.x): release 6.11.3 (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1737">#1737</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/c2c17ae66810378fbad616964d80894794f1dad1"><code>c2c17ae</code></a> build: publish to main</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/b2c6a5c76eccd4bbe445d13e3a04b949f344dd63"><code>b2c6a5c</code></a> build: run tests if ci label added (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1734">#1734</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/a8681ceab4763e706a848121a2dde56791b89eea"><code>a8681ce</code></a> fix(deps): use eslint 8.x (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1728">#1728</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/b5f1391dff5515894830a6570e6d73f5511b2e8f"><code>b5f1391</code></a> fix: do not let setProperty change the prototype (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1731">#1731</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/7afd0a39f41d6df5fda6fa10c319cdf829027d3e"><code>7afd0a3</code></a> build: configure 6.x as default branch</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/37285d0cdc8b20acacd0227daa2e577921de46a7"><code>37285d0</code></a> build: configure backports</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/d127871fb562a5f323994dcc62f304a9ff8e87aa"><code>d127871</code></a> fix: rebuild type, release v6.11.2</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/da9fdd2c57aede410cdeb72b68472707c6d38359"><code>da9fdd2</code></a> fix(types): bring back Field.rule to .d.ts</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/a2ccda1e362ba0124ed246b2ff29c82e8da98bea"><code>a2ccda1</code></a> chore: release v6.11.1</li>
<li>Additional commits viewable in <a href="https://github.com/protobufjs/protobuf.js/compare/v6.10.1...v6.11.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=protobufjs&package-manager=npm_and_yarn&previous-version=6.10.1&new-version=6.11.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/university-course/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-02 22:08:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/university-course/pull/78" class=".btn">#78</a>
            </td>
            <td>
                <b>
                    chore(deps): bump protobufjs from 6.10.1 to 6.11.3 in /support/Lab05/chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [protobufjs](https://github.com/protobufjs/protobuf.js) from 6.10.1 to 6.11.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/protobufjs/protobuf.js/releases">protobufjs's releases</a>.</em></p>
<blockquote>
<h2>v6.11.3</h2>
<h3><a href="https://github.com/protobufjs/protobuf.js/compare/v6.11.2...v6.11.3">6.11.3</a> (2022-05-20)</h3>
<h3>Bug Fixes</h3>
<ul>
<li><strong>deps:</strong> use eslint 8.x (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1728">#1728</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/a8681ceab4763e706a848121a2dde56791b89eea">a8681ce</a>)</li>
<li>do not let setProperty change the prototype (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1731">#1731</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/b5f1391dff5515894830a6570e6d73f5511b2e8f">b5f1391</a>)</li>
</ul>
<h2>v6.11.2</h2>
<h3><a href="https://www.github.com/protobufjs/protobuf.js/compare/v6.11.1...v6.11.2">6.11.2</a> (2021-04-30)</h3>
<ul>
<li>regenerated index.d.ts to fix the unintended breaking change in types.</li>
</ul>
<h2>v6.11.1</h2>
<h3><a href="https://www.github.com/protobufjs/protobuf.js/compare/v6.11.0...v6.11.1">6.11.1</a> (2021-04-29)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>parse.js &quot;parent.add(oneof)“ error (<a href="https://github.com/leon776"><code>@​leon776</code></a>) (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/pull/1602">#1602</a>)</li>
</ul>
<h2>v6.11.0</h2>
<h2><a href="https://www.github.com/protobufjs/protobuf.js/compare/v6.10.2...v6.11.0">6.11.0</a> (2021-04-28)</h2>
<h3>Features</h3>
<ul>
<li>support for proto3 <code>optional</code> fields (<a href="https://github.com/alexander-fenster"><code>@​alexander-fenster</code></a>) (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/pull/1584">#1584</a>)</li>
<li>add <code>--no-service</code> option for <code>pbjs</code> (<a href="https://github.com/mdouglass"><code>@​mdouglass</code></a>) (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/pull/1577">#1577</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>do not assign <code>oneof</code> members to default values, use <code>null</code> instead (<a href="https://github.com/alexander-fenster"><code>@​alexander-fenster</code></a>) (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/pull/1597">#1597</a>)</li>
</ul>
<h3>Dependencies</h3>
<ul>
<li>set <code>@types/node</code> to <code>&gt;= 13.7.0</code> in dependencies (<a href="https://github.com/indutny"><code>@​indutny</code></a>) (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/pull/1575">#1575</a>)</li>
</ul>
<h2>protobuf.js v6.10.2</h2>
<h3>Bug Fixes</h3>
<ul>
<li>es6 export enum (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1446">#1446</a>) (<a href="https://www.github.com/protobufjs/protobuf.js/commit/9f33784350b1efc2e774bbfc087cbd2c47828748">9f33784</a>)</li>
<li>make parsedOptions appear in method JSON representation (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1506">#1506</a>) (<a href="https://www.github.com/protobufjs/protobuf.js/commit/3d29969865f2119550d9dc88391846469da9fa7f">3d29969</a>)</li>
<li>utf8 -&gt; utf16 decoding bug on surrogate pairs (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1486">#1486</a>) (<a href="https://www.github.com/protobufjs/protobuf.js/commit/75172cd11be137bbabd2fba7a02b15067695ebad">75172cd</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/protobufjs/protobuf.js/blob/v6.11.3/CHANGELOG.md">protobufjs's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/protobufjs/protobuf.js/compare/v6.11.2...v6.11.3">6.11.3</a> (2022-05-20)</h3>
<h3>Bug Fixes</h3>
<ul>
<li><strong>deps:</strong> use eslint 8.x (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1728">#1728</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/a8681ceab4763e706a848121a2dde56791b89eea">a8681ce</a>)</li>
<li>do not let setProperty change the prototype (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1731">#1731</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/b5f1391dff5515894830a6570e6d73f5511b2e8f">b5f1391</a>)</li>
</ul>
<h3><a href="https://www.github.com/protobufjs/protobuf.js/compare/v6.11.1...v6.11.2">6.11.2</a> (2021-04-30)</h3>
<ul>
<li>regenerated index.d.ts to fix the unintended breaking change in types.</li>
</ul>
<h3><a href="https://www.github.com/protobufjs/protobuf.js/compare/v6.11.0...v6.11.1">6.11.1</a> (2021-04-29)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>parse.js &quot;parent.add(oneof)“ error (<a href="https://github.com/leon776"><code>@​leon776</code></a>) (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/pull/1602">#1602</a>)</li>
</ul>
<h2><a href="https://www.github.com/protobufjs/protobuf.js/compare/v6.10.2...v6.11.0">6.11.0</a> (2021-04-28)</h2>
<h3>Features</h3>
<ul>
<li>support for proto3 <code>optional</code> fields (<a href="https://github.com/alexander-fenster"><code>@​alexander-fenster</code></a>) (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/pull/1584">#1584</a>)</li>
<li>add <code>--no-service</code> option for <code>pbjs</code> (<a href="https://github.com/mdouglass"><code>@​mdouglass</code></a>) (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/pull/1577">#1577</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>do not assign <code>oneof</code> members to default values, use <code>null</code> instead (<a href="https://github.com/alexander-fenster"><code>@​alexander-fenster</code></a>) (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/pull/1597">#1597</a>)</li>
</ul>
<h3>Dependencies</h3>
<ul>
<li>set <code>@types/node</code> to <code>&gt;= 13.7.0</code> in dependencies (<a href="https://github.com/indutny"><code>@​indutny</code></a>) (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/pull/1575">#1575</a>)</li>
</ul>
<h3><a href="https://www.github.com/protobufjs/protobuf.js/compare/v6.10.1...v6.10.2">6.10.2</a> (2020-11-13)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>es6 export enum (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1446">#1446</a>) (<a href="https://www.github.com/protobufjs/protobuf.js/commit/9f33784350b1efc2e774bbfc087cbd2c47828748">9f33784</a>)</li>
<li>make parsedOptions appear in method JSON representation (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1506">#1506</a>) (<a href="https://www.github.com/protobufjs/protobuf.js/commit/3d29969865f2119550d9dc88391846469da9fa7f">3d29969</a>)</li>
<li>utf8 -&gt; utf16 decoding bug on surrogate pairs (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1486">#1486</a>) (<a href="https://www.github.com/protobufjs/protobuf.js/commit/75172cd11be137bbabd2fba7a02b15067695ebad">75172cd</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/b130dfd4f06b642d4b7c3ccc9f3f9fb6a6e6ed0d"><code>b130dfd</code></a> chore(6.x): release 6.11.3 (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1737">#1737</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/c2c17ae66810378fbad616964d80894794f1dad1"><code>c2c17ae</code></a> build: publish to main</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/b2c6a5c76eccd4bbe445d13e3a04b949f344dd63"><code>b2c6a5c</code></a> build: run tests if ci label added (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1734">#1734</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/a8681ceab4763e706a848121a2dde56791b89eea"><code>a8681ce</code></a> fix(deps): use eslint 8.x (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1728">#1728</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/b5f1391dff5515894830a6570e6d73f5511b2e8f"><code>b5f1391</code></a> fix: do not let setProperty change the prototype (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1731">#1731</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/7afd0a39f41d6df5fda6fa10c319cdf829027d3e"><code>7afd0a3</code></a> build: configure 6.x as default branch</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/37285d0cdc8b20acacd0227daa2e577921de46a7"><code>37285d0</code></a> build: configure backports</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/d127871fb562a5f323994dcc62f304a9ff8e87aa"><code>d127871</code></a> fix: rebuild type, release v6.11.2</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/da9fdd2c57aede410cdeb72b68472707c6d38359"><code>da9fdd2</code></a> fix(types): bring back Field.rule to .d.ts</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/a2ccda1e362ba0124ed246b2ff29c82e8da98bea"><code>a2ccda1</code></a> chore: release v6.11.1</li>
<li>Additional commits viewable in <a href="https://github.com/protobufjs/protobuf.js/compare/v6.10.1...v6.11.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=protobufjs&package-manager=npm_and_yarn&previous-version=6.10.1&new-version=6.11.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/university-course/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-02 22:07:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/university-course/pull/77" class=".btn">#77</a>
            </td>
            <td>
                <b>
                    chore(deps): bump eventsource from 1.0.7 to 1.1.1 in /support/Lab06/b4s/organization/university/user-interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [eventsource](https://github.com/EventSource/eventsource) from 1.0.7 to 1.1.1.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/EventSource/eventsource/blob/master/HISTORY.md">eventsource's changelog</a>.</em></p>
<blockquote>
<h1><a href="https://github.com/EventSource/eventsource/compare/v1.1.0...v1.1.1">1.1.1</a></h1>
<ul>
<li>Do not include authorization and cookie headers on redirect to different origin (<a href="https://github-redirect.dependabot.com/EventSource/eventsource/pull/273">#273</a> Espen Hovlandsdal)</li>
</ul>
<h1><a href="https://github.com/EventSource/eventsource/compare/v1.0.7...v1.1.0">1.1.0</a></h1>
<ul>
<li>Improve performance for large messages across many chunks (<a href="https://github-redirect.dependabot.com/EventSource/eventsource/pull/130">#130</a> Trent Willis)</li>
<li>Add <code>createConnection</code> option for http or https requests (<a href="https://github-redirect.dependabot.com/EventSource/eventsource/pull/120">#120</a> Vasily Lavrov)</li>
<li>Support HTTP 302 redirects (<a href="https://github-redirect.dependabot.com/EventSource/eventsource/pull/116">#116</a> Ryan Bonte)</li>
<li>Prevent sequential errors from attempting multiple reconnections (<a href="https://github-redirect.dependabot.com/EventSource/eventsource/pull/125">#125</a> David Patty)</li>
<li>Add <code>new</code> to correct test (<a href="https://github-redirect.dependabot.com/EventSource/eventsource/pull/101">#111</a> Stéphane Alnet)</li>
<li>Fix reconnections attempts now happen more than once (<a href="https://github-redirect.dependabot.com/EventSource/eventsource/pull/136">#136</a> Icy Fish)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/EventSource/eventsource/commit/aa7a40843a978f42c0babdec125bf9e0a83bf515"><code>aa7a408</code></a> 1.1.1</li>
<li><a href="https://github.com/EventSource/eventsource/commit/56d489ef853a891deca121bbd463c732fee94dce"><code>56d489e</code></a> chore: rebuild polyfill</li>
<li><a href="https://github.com/EventSource/eventsource/commit/4a951e58b04118c9c4d3da3d27d454972a1b4b8d"><code>4a951e5</code></a> docs: update history for 1.1.1</li>
<li><a href="https://github.com/EventSource/eventsource/commit/f9f6416567bff62c1af2f4314be51d9870e94bc2"><code>f9f6416</code></a> fix: strip sensitive headers on redirect to different origin</li>
<li><a href="https://github.com/EventSource/eventsource/commit/9dd06876ab43af37c3313c679fbdc7f722293a0d"><code>9dd0687</code></a> 1.1.0</li>
<li><a href="https://github.com/EventSource/eventsource/commit/49497ba7107a7a94d7dbc73b6e5cc0117f8606e8"><code>49497ba</code></a> Update history for 1.1.0 (<a href="https://github-redirect.dependabot.com/EventSource/eventsource/issues/146">#146</a>)</li>
<li><a href="https://github.com/EventSource/eventsource/commit/3a3853793f63eb5dab9d863504817a9d37b992e6"><code>3a38537</code></a> Update history for <a href="https://github-redirect.dependabot.com/EventSource/eventsource/issues/136">#136</a></li>
<li><a href="https://github.com/EventSource/eventsource/commit/46fe04e03e54f4129a28bf75b3a1e5f4ab68b52a"><code>46fe04e</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/EventSource/eventsource/issues/136">#136</a> from icy-fish/master</li>
<li><a href="https://github.com/EventSource/eventsource/commit/9a4190f65e761ee672d786a6d01c60392950064b"><code>9a4190f</code></a> Fix issue: reconnection only happends for 1 time after connection drops</li>
<li><a href="https://github.com/EventSource/eventsource/commit/61e1b19c8616aa151835a4ae599b299afb574ebf"><code>61e1b19</code></a> test: destroy both proxied request and response on close</li>
<li>Additional commits viewable in <a href="https://github.com/EventSource/eventsource/compare/v1.0.7...v1.1.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=eventsource&package-manager=npm_and_yarn&previous-version=1.0.7&new-version=1.1.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/university-course/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-01 20:11:45 +0000 UTC
    </div>
</div>

