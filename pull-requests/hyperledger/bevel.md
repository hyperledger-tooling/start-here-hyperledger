---
layout: default
title: bevel
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/bevel
---

# bevel <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/bevel){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1815" class=".btn">#1815</a>
            </td>
            <td>
                <b>
                    [ci skip] merge main to develop
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                merge main to develop
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-21 09:52:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1814" class=".btn">#1814</a>
            </td>
            <td>
                <b>
                    [chore] merge develop to main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**
- merge latest to main
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-21 09:45:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1813" class=".btn">#1813</a>
            </td>
            <td>
                <b>
                    [shared] Main to develop merge
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**
- merge main to develop
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-20 16:27:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1812" class=".btn">#1812</a>
            </td>
            <td>
                <b>
                    [fabric] Ensure successful storage of crypto materials in vault
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: mgCepeda <marina.gomez.cepeda@accenture.com>

**Changelog**
- add in ca-tools chart logic to check the storage of cryptographic materials in the vault
- add a new role check/crypto_materials

 

**Reviewed by**
@suvajit-sarkar
@jagpreetsinghsasan

 

**Linked issue**
#1761 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-17 17:02:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1811" class=".btn">#1811</a>
            </td>
            <td>
                <b>
                    Bump handlebars from 4.7.3 to 4.7.7 in /examples/supplychain-app/supplychain-frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [handlebars](https://github.com/wycats/handlebars.js) from 4.7.3 to 4.7.7.
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
<p><a href="https://github.com/handlebars-lang/handlebars.js/compare/v4.7.6...v4.7.7">Commits</a></p>
<h2>v4.7.6 - April 3rd, 2020</h2>
<p>Chore/Housekeeping:</p>
<ul>
<li><a href="https://github-redirect.dependabot.com/handlebars-lang/handlebars.js/issues/1672">#1672</a> - Switch cmd parser to latest minimist (<a href="https://api.github.com/users/dougwilson"><code>@​dougwilson</code></a></li>
</ul>
<p>Compatibility notes:</p>
<ul>
<li>Restored Node.js compatibility</li>
</ul>
<p><a href="https://github.com/handlebars-lang/handlebars.js/compare/v4.7.5...v4.7.6">Commits</a></p>
<h2>v4.7.5 - April 2nd, 2020</h2>
<p>Chore/Housekeeping:</p>
<ul>
<li><del>Node.js version support has been changed to v6+</del> Reverted in 4.7.6</li>
</ul>
<p>Compatibility notes:</p>
<ul>
<li><del>Node.js &lt; v6 is no longer supported</del> Reverted in 4.7.6</li>
</ul>
<p><a href="https://github.com/handlebars-lang/handlebars.js/compare/v4.7.4...v4.7.5">Commits</a></p>
<h2>v4.7.4 - April 1st, 2020</h2>
<p>Chore/Housekeeping:</p>
<ul>
<li><a href="https://github-redirect.dependabot.com/handlebars-lang/handlebars.js/issues/1666">#1666</a> - Replaced minimist with yargs for handlebars CLI (<a href="https://api.github.com/users/aorinevo"><code>@​aorinevo</code></a>, <a href="https://api.github.com/users/AviVahl"><code>@​AviVahl</code></a> &amp; <a href="https://api.github.com/users/fabb"><code>@​fabb</code></a>)</li>
</ul>
<p>Compatibility notes:</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
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
<li><a href="https://github.com/handlebars-lang/handlebars.js/commit/e6ad93ea01bcde1f8ddaa4b4ebe572dd616abfaa"><code>e6ad93e</code></a> v4.7.6</li>
<li><a href="https://github.com/handlebars-lang/handlebars.js/commit/2bf4fc6fd3ae3d8f076d628653f284d85faebeb4"><code>2bf4fc6</code></a> Update release notes</li>
<li>Additional commits viewable in <a href="https://github.com/wycats/handlebars.js/compare/v4.7.3...v4.7.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=handlebars&package-manager=npm_and_yarn&previous-version=4.7.3&new-version=4.7.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-17 15:47:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1810" class=".btn">#1810</a>
            </td>
            <td>
                <b>
                    Bump merge-deep from 3.0.2 to 3.0.3 in /examples/supplychain-app/supplychain-frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [merge-deep](https://github.com/jonschlinkert/merge-deep) from 3.0.2 to 3.0.3.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jonschlinkert/merge-deep/commit/628ff47c9d824ccf21adf9a2b7cc6b74632e11a1"><code>628ff47</code></a> 3.0.3</li>
<li><a href="https://github.com/jonschlinkert/merge-deep/commit/cfbe20ccdb00255b711de57e37ed8ce9f109ef3f"><code>cfbe20c</code></a> run verb to generate README documentation</li>
<li><a href="https://github.com/jonschlinkert/merge-deep/commit/e370968581413a2e5ffdbbf7c2f5094e0e0b3861"><code>e370968</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/jonschlinkert/merge-deep/issues/17">#17</a> from jonschlinkert/key-properties</li>
<li><a href="https://github.com/jonschlinkert/merge-deep/commit/393e2cbaeacf54e77a307c3620a00f0ac057b8d5"><code>393e2cb</code></a> adding a test to ensure using merge-deep for inheritance still works</li>
<li><a href="https://github.com/jonschlinkert/merge-deep/commit/c39b16134a6a9704be2e661b49b92e8561f10d90"><code>c39b161</code></a> add test to ensure constructor is not cloned</li>
<li><a href="https://github.com/jonschlinkert/merge-deep/commit/11e5dd56de8a6aed0b1ed022089dbce6968d82a5"><code>11e5dd5</code></a> add isValidKey function to ensure only valid keys are merged</li>
<li>See full diff in <a href="https://github.com/jonschlinkert/merge-deep/compare/3.0.2...3.0.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=merge-deep&package-manager=npm_and_yarn&previous-version=3.0.2&new-version=3.0.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-17 15:46:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1809" class=".btn">#1809</a>
            </td>
            <td>
                <b>
                    Bump lodash from 4.17.15 to 4.17.21 in /examples/supplychain-app/supplychain-frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [lodash](https://github.com/lodash/lodash) from 4.17.15 to 4.17.21.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/lodash/lodash/commit/f299b52f39486275a9e6483b60a410e06520c538"><code>f299b52</code></a> Bump to v4.17.21</li>
<li><a href="https://github.com/lodash/lodash/commit/c4847ebe7d14540bb28a8b932a9ce1b9ecbfee1a"><code>c4847eb</code></a> Improve performance of <code>toNumber</code>, <code>trim</code> and <code>trimEnd</code> on large input strings</li>
<li><a href="https://github.com/lodash/lodash/commit/3469357cff396a26c363f8c1b5a91dde28ba4b1c"><code>3469357</code></a> Prevent command injection through <code>_.template</code>'s <code>variable</code> option</li>
<li><a href="https://github.com/lodash/lodash/commit/ded9bc66583ed0b4e3b7dc906206d40757b4a90a"><code>ded9bc6</code></a> Bump to v4.17.20.</li>
<li><a href="https://github.com/lodash/lodash/commit/63150ef7645ac07961b63a86490f419f356429aa"><code>63150ef</code></a> Documentation fixes.</li>
<li><a href="https://github.com/lodash/lodash/commit/00f0f62a979d2f5fa0287c06eae70cf9a62d8794"><code>00f0f62</code></a> test.js: Remove trailing comma.</li>
<li><a href="https://github.com/lodash/lodash/commit/846e434c7a5b5692c55ebf5715ed677b70a32389"><code>846e434</code></a> Temporarily use a custom fork of <code>lodash-cli</code>.</li>
<li><a href="https://github.com/lodash/lodash/commit/5d046f39cbd27f573914768e3b36eeefcc4f1229"><code>5d046f3</code></a> Re-enable Travis tests on <code>4.17</code> branch.</li>
<li><a href="https://github.com/lodash/lodash/commit/aa816b36d402a1ad9385142ce7188f17dae514fd"><code>aa816b3</code></a> Remove <code>/npm-package</code>.</li>
<li><a href="https://github.com/lodash/lodash/commit/d7fbc52ee0466a6d248f047b5d5c3e6d1e099056"><code>d7fbc52</code></a> Bump to v4.17.19</li>
<li>Additional commits viewable in <a href="https://github.com/lodash/lodash/compare/4.17.15...4.17.21">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~bnjmnt4n">bnjmnt4n</a>, a new releaser for lodash since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=lodash&package-manager=npm_and_yarn&previous-version=4.17.15&new-version=4.17.21)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-17 13:32:10 +0000 UTC
    </div>
</div>

