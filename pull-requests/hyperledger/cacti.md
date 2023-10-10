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
                PR <a href="https://github.com/hyperledger/cacti/pull/2755" class=".btn">#2755</a>
            </td>
            <td>
                <b>
                    fix(cmd-api-server): add runtime type validation to HTTP verbs pulled from OAS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                This addresses the shortcomings of the linter fix provided in #2751, which
uses unchecked casts to the linter warnings go away.
With the fix of #2751, at runtime, the possibility of a crash is still there
exactly as before, but it has silenced the linter about calling that
possibility out.

We now use a type guard to check the type of the object before casting it
and therefore ensure that at runtime the cast will not produce a crash.

[skip ci]

Depends on #2751
Depends on #2754

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
[x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
[x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
[x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information.

**Character Limit**
[x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
[x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-09 17:59:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2754" class=".btn">#2754</a>
            </td>
            <td>
                <b>
                    feat(common): add express http verb method name string literal type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Also ships with a user-defined typescript type-guard so that we can
ensure at runtime that the string literal value is indeed one of the
valid ExpressJS HTTP verb method names.
2. The primary use-case for this is checking at runtime the HTTP verb
name of OpenAPI specifications that are being loaded into the API.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
[x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
[x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
[x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information.

**Character Limit**
[x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
[x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-09 17:28:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2753" class=".btn">#2753</a>
            </td>
            <td>
                <b>
                    feat(cactus-plugin-ledger-connector-ethereum): add json-rpc proxy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add proxy endpoint handling. Requests sent to this endpoint will be passed directly to the ethereum node.
- Add test to verify that proxy is working.
- Update README of ethereum connector.

**Pull Request Requirements**
[ ] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
[ ] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
[ ] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information.

**Character Limit**
[ ] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
[ ] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-09 12:21:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2751" class=".btn">#2751</a>
            </td>
            <td>
                <b>
                    style(cmd-api-server): fix any linter in getOrCreateWebServices()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description:
This pull request addresses issue #2676  by fixing an Unexpected any linter warning in the getOrCreateWebServices() method of the ApiServer class. The warning occurred due to a typecast using (app as any). 

### Changes:
Replaced (app as any) with (app as express.Express)[httpVerbPrometheus as keyof express.Express](httpPathPrometheus, prometheusExporterHandler);

### Importance of keyof:
The use of keyof here is crucial because it ensures that httpVerbPrometheus and httpVerb are treated as the valid key of the express.Express type. This is necessary because HTTP verbs, like GET, POST, PUT etc... should be treated as keys within the express.Express type. By casting httpVerbPrometheus as keyof express.Express, we enforce type safety and prevent potential runtime errors that could occur if an invalid HTTP verb is used. In essence, it ensures that only valid HTTP verbs are accepted, improving the robustness of the code. 

### Benefits:
This change enhances code readability and maintainability using appropriate types and expressions.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-06 19:26:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2750" class=".btn">#2750</a>
            </td>
            <td>
                <b>
                    feat(cactus-plugin-ledger-connector-ethereum): add signing utils
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add methods for signing transactions to ethereum connector.
- Modify offline signing test to use this new method.
- Modify electricity trade sample to use new signing method.
- Add offline signature section to ethereum connector readme.

**Pull Request Requirements**
[ ] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
[ ] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
[ ] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information.

**Character Limit**
[ ] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
[ ] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-06 12:24:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2749" class=".btn">#2749</a>
            </td>
            <td>
                <b>
                    feat(cactus-plugin-persistence-ethereum): use openapi ethereum connector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                 - Refactor persistence ethereum plugin to use openapi ethereum connector
    instead of ethereum-socketio.
- Upgrade web3js to 4.X in both persistence plugin and its tests.
- Update persistence plugin dependency list.
- Recompile base token contracts in persistence plugin to match format
    required by ethereum connector (full compilation output, not just ABI)
- Minor fix in ethereum connector to return empty transactions
    array instead of undefined.
- Fix minor runtime issues in geth-test-ledger

Depends on #2631

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-05 15:02:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2748" class=".btn">#2748</a>
            </td>
            <td>
                <b>
                    Satp
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Pull Request Requirements**
[ ] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
[ ] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
[ ] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information.

**Character Limit**
[ ] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
[ ] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-05 13:49:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2740" class=".btn">#2740</a>
            </td>
            <td>
                <b>
                    build(lint): fix linter - doesn't work after last prettier upgrade to v3.0.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I ran `yarn up eslint-plugin-prettier --exact` to produce the diff of
this commit. I also ran `yarn lint` to verify that the linter works.

[skip ci]

Fixes #2727

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>


**Pull Request Requirements**
[x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
[x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
[x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information.

**Character Limit**
[x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
[x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-04 22:16:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2738" class=".btn">#2738</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump postcss from 8.4.16 to 8.4.31 in /packages/cacti-ledger-browser
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [postcss](https://github.com/postcss/postcss) from 8.4.16 to 8.4.31.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/postcss/postcss/releases">postcss's releases</a>.</em></p>
<blockquote>
<h2>8.4.31</h2>
<ul>
<li>Fixed <code>\r</code> parsing to fix CVE-2023-44270.</li>
</ul>
<h2>8.4.30</h2>
<ul>
<li>Improved source map performance (by <a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
</ul>
<h2>8.4.29</h2>
<ul>
<li>Fixed <code>Node#source.offset</code> (by <a href="https://github.com/idoros"><code>@​idoros</code></a>).</li>
<li>Fixed docs (by <a href="https://github.com/coliff"><code>@​coliff</code></a>).</li>
</ul>
<h2>8.4.28</h2>
<ul>
<li>Fixed <code>Root.source.end</code> for better source map (by <a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed <code>Result.root</code> types when <code>process()</code> has no parser.</li>
</ul>
<h2>8.4.27</h2>
<ul>
<li>Fixed <code>Container</code> clone methods types.</li>
</ul>
<h2>8.4.26</h2>
<ul>
<li>Fixed clone methods types.</li>
</ul>
<h2>8.4.25</h2>
<ul>
<li>Improve stringify performance (by <a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed docs (by <a href="https://github.com/vikaskaliramna07"><code>@​vikaskaliramna07</code></a>).</li>
</ul>
<h2>8.4.24</h2>
<ul>
<li>Fixed <code>Plugin</code> types.</li>
</ul>
<h2>8.4.23</h2>
<ul>
<li>Fixed warnings in TypeDoc.</li>
</ul>
<h2>8.4.22</h2>
<ul>
<li>Fixed TypeScript support with <code>node16</code> (by <a href="https://github.com/remcohaszing"><code>@​remcohaszing</code></a>).</li>
</ul>
<h2>8.4.21</h2>
<ul>
<li>Fixed <code>Input#error</code> types (by <a href="https://github.com/hudochenkov"><code>@​hudochenkov</code></a>).</li>
</ul>
<h2>8.4.20</h2>
<ul>
<li>Fixed source map generation for childless at-rules like <code>@layer</code>.</li>
</ul>
<h2>8.4.19</h2>
<ul>
<li>Fixed whitespace preserving after AST transformations (by <a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
</ul>
<h2>8.4.18</h2>
<ul>
<li>Fixed an error on <code>absolute: true</code> with empty <code>sourceContent</code> (by <a href="https://github.com/KingSora"><code>@​KingSora</code></a>).</li>
</ul>
<h2>8.4.17</h2>
<ul>
<li>Fixed <code>Node.before()</code> unexpected behavior (by <a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Added TOC to docs (by <a href="https://github.com/muddv"><code>@​muddv</code></a>).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/postcss/postcss/blob/main/CHANGELOG.md">postcss's changelog</a>.</em></p>
<blockquote>
<h2>8.4.31</h2>
<ul>
<li>Fixed <code>\r</code> parsing to fix CVE-2023-44270.</li>
</ul>
<h2>8.4.30</h2>
<ul>
<li>Improved source map performance (by Romain Menke).</li>
</ul>
<h2>8.4.29</h2>
<ul>
<li>Fixed <code>Node#source.offset</code> (by Ido Rosenthal).</li>
<li>Fixed docs (by Christian Oliff).</li>
</ul>
<h2>8.4.28</h2>
<ul>
<li>Fixed <code>Root.source.end</code> for better source map (by Romain Menke).</li>
<li>Fixed <code>Result.root</code> types when <code>process()</code> has no parser.</li>
</ul>
<h2>8.4.27</h2>
<ul>
<li>Fixed <code>Container</code> clone methods types.</li>
</ul>
<h2>8.4.26</h2>
<ul>
<li>Fixed clone methods types.</li>
</ul>
<h2>8.4.25</h2>
<ul>
<li>Improve stringify performance (by Romain Menke).</li>
<li>Fixed docs (by <a href="https://github.com/vikaskaliramna07"><code>@​vikaskaliramna07</code></a>).</li>
</ul>
<h2>8.4.24</h2>
<ul>
<li>Fixed <code>Plugin</code> types.</li>
</ul>
<h2>8.4.23</h2>
<ul>
<li>Fixed warnings in TypeDoc.</li>
</ul>
<h2>8.4.22</h2>
<ul>
<li>Fixed TypeScript support with <code>node16</code> (by Remco Haszing).</li>
</ul>
<h2>8.4.21</h2>
<ul>
<li>Fixed <code>Input#error</code> types (by Aleks Hudochenkov).</li>
</ul>
<h2>8.4.20</h2>
<ul>
<li>Fixed source map generation for childless at-rules like <code>@layer</code>.</li>
</ul>
<h2>8.4.19</h2>
<ul>
<li>Fixed whitespace preserving after AST transformations (by Romain Menke).</li>
</ul>
<h2>8.4.18</h2>
<ul>
<li>Fixed an error on <code>absolute: true</code> with empty <code>sourceContent</code> (by Rene Haas).</li>
</ul>
<h2>8.4.17</h2>
<ul>
<li>Fixed <code>Node.before()</code> unexpected behavior (by Romain Menke).</li>
<li>Added TOC to docs (by Mikhail Dedov).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/postcss/postcss/commit/90208de8805dd762596c0028b8637ffbed23e371"><code>90208de</code></a> Release 8.4.31 version</li>
<li><a href="https://github.com/postcss/postcss/commit/58cc860b4c1707510c9cd1bc1fa30b423a9ad6c5"><code>58cc860</code></a> Fix carrier return parsing</li>
<li><a href="https://github.com/postcss/postcss/commit/4fff8e4cdc237619df1d73a444c0a8329701c1e2"><code>4fff8e4</code></a> Improve pnpm test output</li>
<li><a href="https://github.com/postcss/postcss/commit/cd43ed123274a92ebc13a1e8cccf1d65b8198f84"><code>cd43ed1</code></a> Update dependencies</li>
<li><a href="https://github.com/postcss/postcss/commit/caa916bdcbf66c51321574e2dde112ab13e8b306"><code>caa916b</code></a> Update dependencies</li>
<li><a href="https://github.com/postcss/postcss/commit/8972f76923e921a3c9655822382039b31b1c8e1a"><code>8972f76</code></a> Typo</li>
<li><a href="https://github.com/postcss/postcss/commit/11a5286f781d2a637f2c545c5e9cd661055acaab"><code>11a5286</code></a> Typo</li>
<li><a href="https://github.com/postcss/postcss/commit/45c55017776fc61f7815d1ea8e92d5291ca5d6c8"><code>45c5501</code></a> Release 8.4.30 version</li>
<li><a href="https://github.com/postcss/postcss/commit/bc3c341f589f9c15f1b56838a33d908374e537e0"><code>bc3c341</code></a> Update linter</li>
<li><a href="https://github.com/postcss/postcss/commit/b2be58a2eb788d12474ee1335f8ecdb9fa6225aa"><code>b2be58a</code></a> Merge pull request <a href="https://redirect.github.com/postcss/postcss/issues/1881">#1881</a> from romainmenke/improve-sourcemap-performance--phil...</li>
<li>Additional commits viewable in <a href="https://github.com/postcss/postcss/compare/8.4.16...8.4.31">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=postcss&package-manager=npm_and_yarn&previous-version=8.4.16&new-version=8.4.31)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-10-04 05:41:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2735" class=".btn">#2735</a>
            </td>
            <td>
                <b>
                    feat(cactus-example-electricity-trade): use openapi ethereum connector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Refactor electricity trade sample to use openapi ethereum connector instead of ethereum-socketio.
- Sample still uses offline signing from cmd-socketio-server
- Handle case in ethereum connector where receipt doesn't contain status.
- Add sawtooth test-ledger script to wait until docker is fully started before proceeding forward.
- Remove periodicExecuter from sample app (didn't work and not used

**Pull Request Requirements**
[ ] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
[ ] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
[ ] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information.

**Character Limit**
[ ] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
[ ] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-03 15:11:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2734" class=".btn">#2734</a>
            </td>
            <td>
                <b>
                    ci(dast-nuclei): fix Could not run nuclei: no valid templates were found
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2590

**Pull Request Requirements**
[ ] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
[ ] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
[ ] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information.

**Character Limit**
[ ] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
[ ] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-03 07:45:58 +0000 UTC
    </div>
</div>

