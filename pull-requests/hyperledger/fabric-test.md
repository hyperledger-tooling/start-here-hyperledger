---
layout: default
title: fabric-test
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-test
---

# fabric-test <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-test){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-test/pull/317" class=".btn">#317</a>
            </td>
            <td>
                <b>
                    Bump handlebars from 4.7.6 to 4.7.7 in /tools/chaincode-integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [handlebars](https://github.com/wycats/handlebars.js) from 4.7.6 to 4.7.7.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/handlebars-lang/handlebars.js/blob/master/release-notes.md">handlebars's changelog</a>.</em></p>
<blockquote>
<h2>v4.7.7 - February 15th, 2021</h2>
<ul>
<li>fix weird error in integration tests - eb860c0</li>
<li>fix: check prototype property access in strict-mode (<a href="https://github-redirect.dependabot.com/wycats/handlebars.js/issues/1736">#1736</a>) - b6d3de7</li>
<li>fix: escape property names in compat mode (<a href="https://github-redirect.dependabot.com/wycats/handlebars.js/issues/1736">#1736</a>) - f058970</li>
<li>refactor: In spec tests, use expectTemplate over equals and shouldThrow (<a href="https://github-redirect.dependabot.com/wycats/handlebars.js/issues/1683">#1683</a>) - 77825f8</li>
<li>chore: start testing on Node.js 12 and 13 - 3789a30</li>
</ul>
<p>(POSSIBLY) BREAKING CHANGES:</p>
<ul>
<li>the changes from version <a href="https://github.com/handlebars-lang/handlebars.js/blob/master/release-notes.md#v460---january-8th-2020">4.6.0</a> now also apply
in when using the compile-option &quot;strict: true&quot;. Access to prototype properties is forbidden completely by default, specific properties or methods
can be allowed via runtime-options. See <a href="https://github-redirect.dependabot.com/wycats/handlebars.js/issues/1633">#1633</a> for details. If you are using Handlebars as documented, you should not be accessing prototype properties
from your template anyway, so the changes should not be a problem for you. Only the use of undocumented features can break your build.</li>
</ul>
<p>That is why we only bump the patch version despite mentioning breaking changes.</p>
<p><a href="https://github.com/wycats/handlebars.js/compare/v4.7.6...v4.7.7">Commits</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/handlebars-lang/handlebars.js/commit/a9a8e403213583ca90cb7c872d3a22796c37d961"><code>a9a8e40</code></a> v4.7.7</li>
<li><a href="https://github.com/handlebars-lang/handlebars.js/commit/e66aed5b99c1b6c93564f37d627e34e5d60eb76e"><code>e66aed5</code></a> Update release notes</li>
<li><a href="https://github.com/handlebars-lang/handlebars.js/commit/7d4d170ce46a53084a41920c5c7387c131357989"><code>7d4d170</code></a> disable IE in Saucelabs tests</li>
<li><a href="https://github.com/handlebars-lang/handlebars.js/commit/eb860c08998f8f506360d305d89e1f4b40f72a0a"><code>eb860c0</code></a> fix weird error in integration tests</li>
<li><a href="https://github.com/handlebars-lang/handlebars.js/commit/b6d3de7123eebba603e321f04afdbae608e8fea8"><code>b6d3de7</code></a> fix: check prototype property access in strict-mode (<a href="https://github-redirect.dependabot.com/wycats/handlebars.js/issues/1736">#1736</a>)</li>
<li><a href="https://github.com/handlebars-lang/handlebars.js/commit/f0589701698268578199be25285b2ebea1c1e427"><code>f058970</code></a> fix: escape property names in compat mode (<a href="https://github-redirect.dependabot.com/wycats/handlebars.js/issues/1736">#1736</a>)</li>
<li><a href="https://github.com/handlebars-lang/handlebars.js/commit/77825f8d3522356feb8e4160fac16344104d192b"><code>77825f8</code></a> refator: In spec tests, use expectTemplate over equals and shouldThrow (<a href="https://github-redirect.dependabot.com/wycats/handlebars.js/issues/1683">#1683</a>)</li>
<li><a href="https://github.com/handlebars-lang/handlebars.js/commit/3789a309554fd600caeae442f40881cf93eb3b54"><code>3789a30</code></a> chore: start testing on Node.js 12 and 13</li>
<li>See full diff in <a href="https://github.com/wycats/handlebars.js/compare/v4.7.6...v4.7.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=handlebars&package-manager=npm_and_yarn&previous-version=4.7.6&new-version=4.7.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-test/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-08 17:22:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-test/pull/316" class=".btn">#316</a>
            </td>
            <td>
                <b>
                    Bump underscore from 1.9.2 to 1.13.1 in /tools/chaincode-integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [underscore](https://github.com/jashkenas/underscore) from 1.9.2 to 1.13.1.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jashkenas/underscore/commit/943977e34e2279503528a71ddcc2dd5f96483945"><code>943977e</code></a> Merge branch 'umd-alias', tag 1.13.1 release</li>
<li><a href="https://github.com/jashkenas/underscore/commit/5630f882932552ba23f34b57f91c0c6e2a38ad82"><code>5630f88</code></a> Add version 1.13.1 to the change log</li>
<li><a href="https://github.com/jashkenas/underscore/commit/5aa5b526a94edf487ab1d4a4e3cde8f7749e6d2c"><code>5aa5b52</code></a> Update the bundle sizes</li>
<li><a href="https://github.com/jashkenas/underscore/commit/76c8d8a05db2d0f9ecfb193ba2ab7780c4a26441"><code>76c8d8a</code></a> Bump the version to 1.13.1</li>
<li><a href="https://github.com/jashkenas/underscore/commit/9cda0b09742c9ed6ae5e1bccb709b63f32a04f45"><code>9cda0b0</code></a> Add some build clarifications to the documentation (<a href="https://github-redirect.dependabot.com/jashkenas/underscore/issues/2923">#2923</a>)</li>
<li><a href="https://github.com/jashkenas/underscore/commit/8b5928c04b9a61a99e2704740b80287247e9f47a"><code>8b5928c</code></a> Revert .gitignore underscore.js from 57a4a0e (fix <a href="https://github-redirect.dependabot.com/jashkenas/underscore/issues/2923">#2923</a>)</li>
<li><a href="https://github.com/jashkenas/underscore/commit/7054a54d63af2ed1c99eb3707836da709b5e625e"><code>7054a54</code></a> Update generated sources and tag 1.13.0 release</li>
<li><a href="https://github.com/jashkenas/underscore/commit/37dc52a61054674115be560ab9cbdd26b05031ed"><code>37dc52a</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/jashkenas/underscore/issues/2921">#2921</a> from jgonggrijp/prepare-1.13.0</li>
<li><a href="https://github.com/jashkenas/underscore/commit/5511d129881253807d728cc6a21fff55953ae4f9"><code>5511d12</code></a> Add version 1.13.0 to the change log</li>
<li><a href="https://github.com/jashkenas/underscore/commit/efe5fbf4a1d43c9a88c1646aa5ab53a4745655b8"><code>efe5fbf</code></a> Bump the version to 1.13.0</li>
<li>Additional commits viewable in <a href="https://github.com/jashkenas/underscore/compare/1.9.2...1.13.1">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~jgonggrijp">jgonggrijp</a>, a new releaser for underscore since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=underscore&package-manager=npm_and_yarn&previous-version=1.9.2&new-version=1.13.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-test/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-07 02:25:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-test/pull/315" class=".btn">#315</a>
            </td>
            <td>
                <b>
                    Update Java SDK interop test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The Java SDK integration test script requires ubuntu-20.04 vm image

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-05 15:42:28 +0000 UTC
    </div>
</div>

