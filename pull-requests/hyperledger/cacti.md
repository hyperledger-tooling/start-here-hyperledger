---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3048" class=".btn">#3048</a>
            </td>
            <td>
                <b>
                    style(docs/examples/supply-chain): move block scoped code to functions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a purely stylistic change that makes the code read much better
and also reduces the chance of future bugs that would get introduced due
to block scoping side effects that people not experienced with the
language could make.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-02 02:47:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3047" class=".btn">#3047</a>
            </td>
            <td>
                <b>
                    refactor(test-tooling): fix types of streams: use NodeJS.ReadableStream
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. The container management library that we use in the test infrastructure
(called dockerode) is expecting streams that are defined in the global
namespace of the `@types/node` library, e.g. the standard library of NodeJS
itself.
2. Previously we were using the "streams" package to provide type information
to the streams that we were passing around to dockerode and it was working
fine, but after some changes that seem unrelated this has broken the
compilation process.
3. The mentioned changes are not yet on the main branch, but we expect
them to be there soon and so this change is laying the groundwork for that
by pre-emptively fixing the broken build's root cause which is that the
test-tooling package does not declare it's typings related dependencies
correctly: It implicitly uses the NodeJS standard library's types but
so far had not declared them on the package level.
4. This change is therefore to rectify the issue of the `@types/node`
dependency missing from the test-tooling package and also the refactoring
of some of the test ledger classes which were relying on the `streams`
builtin package instead of correctly using the NodeJS.ReadableStream global.
5. Earlier the reasoning for this was that we try to avoid pulling in
types from the global scope because we try to avoid any sort of dependency
on the global scope in general. Once we have proof though that this is
causing issues with the build, then we must give up the principle for
practical reasons (and only in the minimum viable scope, e.g. this does
not change the fact that everywhere else in the codebase we should still
do our best to avoid using the global scoped classes, types, functions,
etc..).

Thank you to @AndreAugusto11 and @RafaelAPB for pointing out this issue
through the pull request of his that is currently being worked on at the
time of this writing:
https://github.com/RafaelAPB/blockchain-integration-framework/pull/72

Related to but does not address #2811

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-01 19:04:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3046" class=".btn">#3046</a>
            </td>
            <td>
                <b>
                    build(deps): bump sanitize-html from 2.7.0 to 2.12.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [sanitize-html](https://github.com/apostrophecms/sanitize-html) from 2.7.0 to 2.12.1.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/apostrophecms/sanitize-html/blob/main/CHANGELOG.md">sanitize-html's changelog</a>.</em></p>
<blockquote>
<h2>2.12.1 (2024-02-22)</h2>
<ul>
<li>Do not parse sourcemaps in <code>post-css</code>. This fixes a vulnerability in which information about the existence or non-existence of files on a server could be disclosed via properly crafted HTML input when the <code>style</code> attribute is allowed by the configuration. Thanks to the <a href="https://snyk.io/">Snyk Security team</a> for the disclosure and to <a href="https://dylan.is/">Dylan Armstrong</a> for the fix.</li>
</ul>
<h2>2.12.0 (2024-02-21)</h2>
<ul>
<li>
<p>Introduced the <code>allowedEmptyAttributes</code> option, enabling explicit specification of empty string values for select attributes, with the default attribute set to <code>alt</code>. Thanks to <a href="https://github.com/zhna123">Na</a> for the contribution.</p>
</li>
<li>
<p>Clarified the use of SVGs with a new test and changes to documentation. Thanks to <a href="https://github.com/gkumar9891">Gauav Kumar</a> for the contribution.</p>
</li>
<li>
<p>Do not process source maps when processing style tags with PostCSS.</p>
</li>
</ul>
<h2>2.11.0 (2023-06-21)</h2>
<ul>
<li>Fix to allow <code>false</code> in <code>allowedClasses</code> attributes. Thanks to <a href="https://github.com/KevinSJ">Kevin Jiang</a> for this fix!</li>
<li>Upgrade mocha version</li>
<li>Apply small linter fixes in tests</li>
<li>Add <code>.idea</code> temp files to <code>.gitignore</code></li>
<li>Thanks to <a href="https://github.com/VitaliiShpital">Vitalii Shpital</a> for the updates!</li>
<li>Show parseStyleAttributes warning in browser only. Thanks to <a href="https://github.com/mog422">mog422</a> for this update!</li>
<li>Remove empty non-boolean attributes via an exhaustive, configurable list of known non-boolean attributes. <a href="https://github.com/dylanarmstrong">Thanks to Dylan Armstrong</a> for this update!</li>
</ul>
<h2>2.10.0 (2023-02-17)</h2>
<ul>
<li>Fix auto-adding escaped closing tags. In other words, do not add implied closing tags to disallowed tags when <code>disallowedTagMode</code> is set to any variant of <code>escape</code> -- just escape the disallowed tags that are present. This fixes [issue <a href="https://redirect.github.com/apostrophecms/sanitize-html/issues/464">#464</a>](<a href="https://redirect.github.com/apostrophecms/sanitize-html/issues/464">apostrophecms/sanitize-html#464</a>). Thanks to <a href="https://github.com/dliebner">Daniel Liebner</a></li>
<li>Add <code>tagAllowed()</code> helper function which takes a tag name and checks it against <code>options.allowedTags</code> and returns <code>true</code> if the tag is allowed and <code>false</code> if it is not.</li>
</ul>
<h2>2.9.0 (2023-01-27)</h2>
<ul>
<li>Add option parseStyleAttributes to skip style parsing. This fixes [issue <a href="https://redirect.github.com/apostrophecms/sanitize-html/issues/547">#547</a>](<a href="https://redirect.github.com/apostrophecms/sanitize-html/issues/547">apostrophecms/sanitize-html#547</a>). Thanks to <a href="https://github.com/bertyhell">Bert Verhelst</a>.</li>
</ul>
<h2>2.8.1 (2022-12-21)</h2>
<ul>
<li>If the argument is a number, convert it to a string, for backwards compatibility. Thanks to <a href="https://github.com/alexander-schranz">Alexander Schranz</a>.</li>
</ul>
<h2>2.8.0 (2022-12-12)</h2>
<ul>
<li>Upgrades <code>htmlparser2</code> to new major version <code>^8.0.0</code>. Thanks to <a href="https://github.com/kedarchandrayan">Kedar Chandrayan</a> for this contribution.</li>
</ul>
<h2>2.7.3 (2022-10-24)</h2>
<ul>
<li>If allowedTags is falsy but not exactly <code>false</code>, then do not assume that all tags are allowed. Rather, allow no tags in this case, to be on the safe side. This matches the existing documentation and fixes [issue <a href="https://redirect.github.com/apostrophecms/sanitize-html/issues/176">#176</a>](<a href="https://redirect.github.com/apostrophecms/sanitize-html/issues/176">apostrophecms/sanitize-html#176</a>). Thanks to <a href="https://github.com/kedarchandrayan">Kedar Chandrayan</a> for the fix.</li>
</ul>
<h2>2.7.2 (2022-09-15)</h2>
<ul>
<li>Closing tags must agree with opening tags. This fixes [issue <a href="https://redirect.github.com/apostrophecms/sanitize-html/issues/549">#549</a>](<a href="https://redirect.github.com/apostrophecms/sanitize-html/issues/549">apostrophecms/sanitize-html#549</a>), in which closing tags not associated with any permitted opening tag could be passed through. No known exploit exists, but it's better not to permit this. Thanks to
<a href="https://github.com/kedarchandrayan">Kedar Chandrayan</a> for the report and the fix.</li>
</ul>
<h2>2.7.1 (2022-07-20)</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/apostrophecms/sanitize-html/commit/4a7d7dd099b41c909f2faac056d34cf027515079"><code>4a7d7dd</code></a> Merge pull request <a href="https://redirect.github.com/apostrophecms/sanitize-html/issues/654">#654</a> from apostrophecms/release-2.12.1</li>
<li><a href="https://github.com/apostrophecms/sanitize-html/commit/f8e02be9fc3ea639edccfcaa50c6e71a22b2c068"><code>f8e02be</code></a> release 2.12.1</li>
<li><a href="https://github.com/apostrophecms/sanitize-html/commit/c5dbdf77fe8b836d3bf4554ea39edb45281ec0b4"><code>c5dbdf7</code></a> Merge pull request <a href="https://redirect.github.com/apostrophecms/sanitize-html/issues/650">#650</a> from dylanarmstrong/fix/ignore-source-maps</li>
<li><a href="https://github.com/apostrophecms/sanitize-html/commit/5a5a74e179ef98075a0c61789f64e009f6b4ac29"><code>5a5a74e</code></a> Merge pull request <a href="https://redirect.github.com/apostrophecms/sanitize-html/issues/652">#652</a> from apostrophecms/add-thanks-to-changelog</li>
<li><a href="https://github.com/apostrophecms/sanitize-html/commit/ee71ff0c04b2e00f730b8e29206cd65209cca5c4"><code>ee71ff0</code></a> Add community contribution thanks you</li>
<li><a href="https://github.com/apostrophecms/sanitize-html/commit/a226fe7af4c3a8faee6d114984da3f2964e4ae65"><code>a226fe7</code></a> Merge pull request <a href="https://redirect.github.com/apostrophecms/sanitize-html/issues/651">#651</a> from apostrophecms/release-2.12.0</li>
<li><a href="https://github.com/apostrophecms/sanitize-html/commit/ff18600f01a390c81c27442d6e858ec0eb4ef67e"><code>ff18600</code></a> release 2.12.0</li>
<li><a href="https://github.com/apostrophecms/sanitize-html/commit/1e2294c8001ce07c89448e03289818da631795ba"><code>1e2294c</code></a> test: added test for postcss map</li>
<li><a href="https://github.com/apostrophecms/sanitize-html/commit/c376501b9a066479736f0a088fba3492e7122811"><code>c376501</code></a> doc: update changelog</li>
<li><a href="https://github.com/apostrophecms/sanitize-html/commit/075499d1b98c387f4200fd59972ca9b15796b51b"><code>075499d</code></a> fix: ignore source maps when processing with postcss</li>
<li>Additional commits viewable in <a href="https://github.com/apostrophecms/sanitize-html/compare/2.7.0...2.12.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=sanitize-html&package-manager=npm_and_yarn&previous-version=2.7.0&new-version=2.12.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-01 17:37:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3045" class=".btn">#3045</a>
            </td>
            <td>
                <b>
                    build(deps): bump @openzeppelin/contracts-upgradeable from 4.9.3 to 4.9.6 in /examples/cactus-example-carbon-accounting-backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts-upgradeable](https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable) from 4.9.3 to 4.9.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/releases"><code>@​openzeppelin/contracts-upgradeable</code>'s releases</a>.</em></p>
<blockquote>
<h2>v4.9.6</h2>
<ul>
<li><code>Base64</code>: Fix issue where dirty memory located just after the input buffer is affecting the result. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4926">#4926</a>)</li>
</ul>
<h2>v4.9.5</h2>
<ul>
<li><code>Multicall</code>: Patch duplicated <code>Address.functionDelegateCall</code>.</li>
</ul>
<h2>v4.9.4</h2>
<ul>
<li><code>ERC2771Context</code> and <code>Context</code>: Introduce a <code>_contextPrefixLength()</code> getter, used to trim extra information appended to <code>msg.data</code>.</li>
<li><code>Multicall</code>: Make aware of non-canonical context (i.e. <code>msg.sender</code> is not <code>_msgSender()</code>), allowing compatibility with <code>ERC2771Context</code>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/blob/master/CHANGELOG.md"><code>@​openzeppelin/contracts-upgradeable</code>'s changelog</a>.</em></p>
<blockquote>
<h2>4.9.6 (2024-02-29)</h2>
<ul>
<li><code>Base64</code>: Fix issue where dirty memory located just after the input buffer is affecting the result. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4929">#4929</a>)</li>
</ul>
<h2>4.9.5 (2023-12-08)</h2>
<ul>
<li><code>Multicall</code>: Make aware of non-canonical context (i.e. <code>msg.sender</code> is not <code>_msgSender()</code>), allowing compatibility with <code>ERC2771Context</code>. Patch duplicated <code>Address.functionDelegateCall</code> in v4.9.4 (removed).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/2d081f24cac1a867f6f73d512f2022e1fa987854"><code>2d081f2</code></a> Transpile dc44c9f1</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/2492017bf2727ea6bbfb100b6a53959b08ed7243"><code>2492017</code></a> Transpile a6286d0f</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/a40cb0bda838c2ef3dfc252c179f5c37c32e80c4"><code>a40cb0b</code></a> Transpile bd325d56</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/4c73bfa29bced89fc96f440e6424b69424690459"><code>4c73bfa</code></a> Transpile ad6a5b68</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/31f9fb9d171f60b2271b2b9c6f62d43302bf9489"><code>31f9fb9</code></a> Transpile 88ac712e</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/f55babcbeef1d1c42c8e0f8884abcd6663a7909f"><code>f55babc</code></a> Transpile a83918df</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/5bc59992591b84bba18dc1ac46942f1886b30ccd"><code>5bc5999</code></a> Transpile 98c7a4cf</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/152b82019370360578ee273630567bf67b977a40"><code>152b820</code></a> Transpile 0ed435b7</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/f34a3a7e5a1d698d87d517fda698d48286310bee"><code>f34a3a7</code></a> Transpile 17c1a3a4</li>
<li>See full diff in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/compare/v4.9.3...v4.9.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@openzeppelin/contracts-upgradeable&package-manager=npm_and_yarn&previous-version=4.9.3&new-version=4.9.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-01 13:53:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3043" class=".btn">#3043</a>
            </td>
            <td>
                <b>
                    build(deps): bump sqlite3 from 5.0.8 to 5.1.5 in /examples/cactus-example-cbdc-bridging-backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [sqlite3](https://github.com/TryGhost/node-sqlite3) from 5.0.8 to 5.1.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/TryGhost/node-sqlite3/releases">sqlite3's releases</a>.</em></p>
<blockquote>
<h2>v5.1.5</h2>
<h2>What's Changed</h2>
<ul>
<li>🔒 Fixed code execution vulnerability due to Object coercion by <a href="https://github.com/daniellockyer"><code>@​daniellockyer</code></a></li>
<li>Updated bundled SQLite to v3.41.1 by <a href="https://github.com/daniellockyer"><code>@​daniellockyer</code></a></li>
<li>Fixed rpath linker option when using a custom sqlite by <a href="https://github.com/jeromew"><code>@​jeromew</code></a> in <a href="https://redirect.github.com/TryGhost/node-sqlite3/pull/1654">TryGhost/node-sqlite3#1654</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/TryGhost/node-sqlite3/compare/v5.1.4...v5.1.5">https://github.com/TryGhost/node-sqlite3/compare/v5.1.4...v5.1.5</a></p>
<h2>v5.1.4</h2>
<h2>What's Changed</h2>
<ul>
<li>Fixed glibc compatibility by downgrading CI to Ubuntu 20 by <a href="https://github.com/daniellockyer"><code>@​daniellockyer</code></a> in <a href="https://redirect.github.com/TryGhost/node-sqlite3/pull/1664">TryGhost/node-sqlite3#1664</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/TryGhost/node-sqlite3/compare/v5.1.3...v5.1.4">https://github.com/TryGhost/node-sqlite3/compare/v5.1.3...v5.1.4</a></p>
<h2>v5.1.3</h2>
<h2>What's Changed</h2>
<ul>
<li>Updated bundled SQLite to v3.40.0 by <a href="https://github.com/daniellockyer"><code>@​daniellockyer</code></a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/TryGhost/node-sqlite3/compare/v5.1.2...v5.1.3">https://github.com/TryGhost/node-sqlite3/compare/v5.1.2...v5.1.3</a></p>
<h2>v5.1.2</h2>
<h2>What's Changed</h2>
<ul>
<li>Updated bundled SQLite to v3.39.4 by <a href="https://github.com/daniellockyer"><code>@​daniellockyer</code></a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/TryGhost/node-sqlite3/compare/v5.1.1...v5.1.2">https://github.com/TryGhost/node-sqlite3/compare/v5.1.1...v5.1.2</a></p>
<h2>v5.1.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Added Darwin ARM64 binaries by <a href="https://github.com/daniellockyer"><code>@​daniellockyer</code></a> in <a href="https://redirect.github.com/TryGhost/node-sqlite3/pull/1594">TryGhost/node-sqlite3#1594</a></li>
</ul>
<p>A huge thanks to <a href="https://www.macstadium.com/">MacStadium</a> for providing an M1 Mac Mini so we can offer ARM64 binaries.</p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/TryGhost/node-sqlite3/compare/v5.1.0...v5.1.1">https://github.com/TryGhost/node-sqlite3/compare/v5.1.0...v5.1.1</a></p>
<h2>v5.1.0</h2>
<p>✨ We're very excited to announce node-sqlite3's first minor release of v5, packed with features and improvements.</p>
<p>If you encounter any problems, please open a detailed issue using the <a href="https://github.com/TryGhost/node-sqlite3/issues/new/choose">templates</a>.</p>
<h2>What's Changed</h2>
<ul>
<li>Updated bundled SQLite to v3.39.3 by <a href="https://github.com/daniellockyer"><code>@​daniellockyer</code></a></li>
<li>Added ability to receive updates from <code>sqlite3_update_hook</code> by <a href="https://github.com/soukand"><code>@​soukand</code></a> in <a href="https://redirect.github.com/TryGhost/node-sqlite3/pull/1267">TryGhost/node-sqlite3#1267</a></li>
<li>Added support for setting SQLite limits by <a href="https://github.com/paulfitz"><code>@​paulfitz</code></a> in <a href="https://redirect.github.com/TryGhost/node-sqlite3/pull/1548">TryGhost/node-sqlite3#1548</a></li>
<li>Added library types file by <a href="https://github.com/bpasero"><code>@​bpasero</code></a> in <a href="https://redirect.github.com/TryGhost/node-sqlite3/pull/1527">TryGhost/node-sqlite3#1527</a></li>
<li>Added <code>package-lock.json</code> to <code>.gitignore</code> by <a href="https://github.com/JoelEinbinder"><code>@​JoelEinbinder</code></a> in <a href="https://redirect.github.com/TryGhost/node-sqlite3/pull/1628">TryGhost/node-sqlite3#1628</a></li>
<li>Fixed remaining method declarations by <a href="https://github.com/alexanderfloh"><code>@​alexanderfloh</code></a> in <a href="https://redirect.github.com/TryGhost/node-sqlite3/pull/1633">TryGhost/node-sqlite3#1633</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/TryGhost/node-sqlite3/commit/6a806f87903d778d520bce09f6e893752619383b"><code>6a806f8</code></a> v5.1.5</li>
<li><a href="https://github.com/TryGhost/node-sqlite3/commit/edb1934dd222ae55632e120d8f64552d5191c781"><code>edb1934</code></a> Fixed code execution vulnerability due to Object coercion</li>
<li><a href="https://github.com/TryGhost/node-sqlite3/commit/3a4888894dd0e0463d3bf4dc833fdcc995b614af"><code>3a48888</code></a> Updated bundled SQLite to v3.41.1</li>
<li><a href="https://github.com/TryGhost/node-sqlite3/commit/c1440bdaa47ffdda852ff576ac543114c4f0fb4b"><code>c1440bd</code></a> Fixed rpath linker option when using a custom sqlite (<a href="https://redirect.github.com/TryGhost/node-sqlite3/issues/1654">#1654</a>)</li>
<li><a href="https://github.com/TryGhost/node-sqlite3/commit/93affa425958f479150b699f08eb67af3e5b522c"><code>93affa4</code></a> Update microsoft/setup-msbuild action to v1.3</li>
<li><a href="https://github.com/TryGhost/node-sqlite3/commit/6f6318e929367ae05f395c5e0e5e4b09c62e87f4"><code>6f6318e</code></a> v5.1.4</li>
<li><a href="https://github.com/TryGhost/node-sqlite3/commit/aeafe2591d664fcf6c70e7ddadc7875c8f691a4d"><code>aeafe25</code></a> Revert &quot;Renamed <code>master</code> references to <code>main</code>&quot;</li>
<li><a href="https://github.com/TryGhost/node-sqlite3/commit/57ce2d4519d0fe1c801081389d20cc7f357cdc02"><code>57ce2d4</code></a> Fixed glib compatibility by downgrading to Ubuntu 20</li>
<li><a href="https://github.com/TryGhost/node-sqlite3/commit/af8e567f25f9da7e0c14f90ede688efe56486ce4"><code>af8e567</code></a> Renamed <code>master</code> references to <code>main</code></li>
<li><a href="https://github.com/TryGhost/node-sqlite3/commit/8fd18a392c4844288811330dddfcf171c18ed93f"><code>8fd18a3</code></a> Extracted function checking code into macro</li>
<li>Additional commits viewable in <a href="https://github.com/TryGhost/node-sqlite3/compare/v5.0.8...v5.1.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=sqlite3&package-manager=npm_and_yarn&previous-version=5.0.8&new-version=5.1.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-01 13:42:57 +0000 UTC
    </div>
</div>

