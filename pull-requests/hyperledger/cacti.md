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
                PR <a href="https://github.com/hyperledger/cacti/pull/3237" class=".btn">#3237</a>
            </td>
            <td>
                <b>
                    feat(ledger-browser): refactor eth dashboard page
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                - Refactor ETH app dashboard using MUI components.
- Fix ERC20 details page rendering.
- Add block and transaction list components that use common `UITableListing`.
- Add global notifications that will be displayed in a snackbar.

Depends on #3207

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

**Pull Request Requirements**
- [ ] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [ ] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [ ] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [ ] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [ ] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-25 12:03:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3236" class=".btn">#3236</a>
            </td>
            <td>
                <b>
                    ci: mitigate script injection attack in test_weaver-pre-release.yaml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes the script injection attack mentioned here: https://hackerone.com/reports/2471956

Check sample attack run here: https://github.com/sandeepnRES/cacti/actions/runs/8830394750/job/24243428274?pr=23
from PR on my fork: https://github.com/sandeepnRES/cacti/pull/23

Source for the solution: https://docs.github.com/en/actions/security-guides/security-hardening-for-github-actions#example-of-a-script-injection-attack
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-25 09:45:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3235" class=".btn">#3235</a>
            </td>
            <td>
                <b>
                    build(connector-stellar): add skeleton for future Stellar connector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. The diff is already quite large so I've decided to start with a smaller
pull request that is easier to review. Basic functionality is missing from
the connector because of the latter.
2. The build is confirmed to be working, so is code generation and tests.
3. We don't yet have a `StellarTestLedger` class in the test-utils package
and so we can't yet implement end to end testing but once that gets added
we'll be ready to go.
4. For now the public-api.ts and the index.ts and index.web.ts files are
not exporting anything so that we adhere to semantic versioning principles
in that we won't be doing any breaking changes with the sub-sequent pull
requests since there was nothing exported and nothing is unbreakable.

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
        Created At 2024-04-25 01:12:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3232" class=".btn">#3232</a>
            </td>
            <td>
                <b>
                    build(deps): bump gh-pages from 2.2.0 to 5.0.0 in /weaver/docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [gh-pages](https://github.com/tschaub/gh-pages) from 2.2.0 to 5.0.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/tschaub/gh-pages/releases">gh-pages's releases</a>.</em></p>
<blockquote>
<h2>v5.0.0</h2>
<p>Potentially breaking change: the <code>publish</code> method now always returns a promise.  Previously, it did not return a promise in some error cases.  This should not impact most users.</p>
<p>Updates to the development dependencies required a minimum Node version of 14 for the tests.  The library should still work on Node 12, but tests are no longer run in CI for version 12.  A future major version of the library may drop support for version 12 altogether.</p>
<h2>What's Changed</h2>
<ul>
<li>Assorted updates by <a href="https://github.com/tschaub"><code>@​tschaub</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/452">tschaub/gh-pages#452</a></li>
<li>Update README to clarify project site configuration requirements with tools like CRA, webpack, Vite, etc. by <a href="https://github.com/Nezteb"><code>@​Nezteb</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/445">tschaub/gh-pages#445</a></li>
<li>Bump actions/checkout from 2 to 3 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/453">tschaub/gh-pages#453</a></li>
<li>Bump actions/setup-node from 1 to 3 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/455">tschaub/gh-pages#455</a></li>
<li>Bump email-addresses from 3.0.1 to 5.0.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/454">tschaub/gh-pages#454</a></li>
<li>Bump async from 2.6.4 to 3.2.4 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/459">tschaub/gh-pages#459</a></li>
<li>Remove quotation marks by <a href="https://github.com/Vicropht"><code>@​Vicropht</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/438">tschaub/gh-pages#438</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/Nezteb"><code>@​Nezteb</code></a> made their first contribution in <a href="https://redirect.github.com/tschaub/gh-pages/pull/445">tschaub/gh-pages#445</a></li>
<li><a href="https://github.com/Vicropht"><code>@​Vicropht</code></a> made their first contribution in <a href="https://redirect.github.com/tschaub/gh-pages/pull/438">tschaub/gh-pages#438</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/tschaub/gh-pages/compare/v4.0.0...v5.0.0">https://github.com/tschaub/gh-pages/compare/v4.0.0...v5.0.0</a></p>
<h2>v4.0.0</h2>
<p>This release doesn't include any breaking changes, but due to updated development dependencies, tests are no longer run on Node 10.</p>
<h2>What's Changed</h2>
<ul>
<li>Bump minimist from 1.2.5 to 1.2.6 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/423">tschaub/gh-pages#423</a></li>
<li>Bump async from 2.6.1 to 2.6.4 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/427">tschaub/gh-pages#427</a></li>
<li>Bump path-parse from 1.0.6 to 1.0.7 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/431">tschaub/gh-pages#431</a></li>
<li>Bump ansi-regex from 3.0.0 to 3.0.1 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/430">tschaub/gh-pages#430</a></li>
<li>Updated dev dependencies and formatting by <a href="https://github.com/tschaub"><code>@​tschaub</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/432">tschaub/gh-pages#432</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/tschaub/gh-pages/compare/v3.2.3...v4.0.0">https://github.com/tschaub/gh-pages/compare/v3.2.3...v4.0.0</a></p>
<h2>v3.2.3</h2>
<ul>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/398">#398</a> - Update glob-parent (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/395">#395</a> - Switch from filenamify-url to filenamify (<a href="https://github.com/tw0517tw"><code>@​tw0517tw</code></a>)</li>
</ul>
<h2>v3.0.0</h2>
<p>Breaking changes:</p>
<p>None really.  But tests are no longer run on Node &lt; 10.  Development dependencies were updated to address security warnings, and this meant tests could no longer be run on Node 6 or 8.  If you still use these Node versions, you may still be able to use this library, but be warned that tests are no longer run on these versions.</p>
<p>All changes:</p>
<ul>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/357">#357</a> - Dev dependency updates (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/333">#333</a> - Update readme with command line options (<a href="https://github.com/Victoire44"><code>@​Victoire44</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/356">#356</a> - Test as a GitHub action (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/355">#355</a> - feat(beforeAdd): allow custom script before git add (<a href="https://github.com/Xiphe"><code>@​Xiphe</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/336">#336</a> - Fix remove not working properly (<a href="https://github.com/sunghwan2789"><code>@​sunghwan2789</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/328">#328</a> - Update .travis.yml (<a href="https://github.com/XhmikosR"><code>@​XhmikosR</code></a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/tschaub/gh-pages/blob/main/changelog.md">gh-pages's changelog</a>.</em></p>
<blockquote>
<h2>v5.0.0</h2>
<p>Potentially breaking change: the <code>publish</code> method now always returns a promise.  Previously, it did not return a promise in some error cases.  This should not impact most users.</p>
<p>Updates to the development dependencies required a minimum Node version of 14 for the tests.  The library should still work on Node 12, but tests are no longer run in CI for version 12.  A future major version of the library may drop support for version 12 altogether.</p>
<ul>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/438">#438</a> - Remove quotation marks (<a href="https://github.com/Vicropht"><code>@​Vicropht</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/459">#459</a> - Bump async from 2.6.4 to 3.2.4 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/454">#454</a> - Bump email-addresses from 3.0.1 to 5.0.0 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/455">#455</a> - Bump actions/setup-node from 1 to 3 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/453">#453</a> - Bump actions/checkout from 2 to 3 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/445">#445</a> - Update README to clarify project site configuration requirements with tools like CRA, webpack, Vite, etc. (<a href="https://github.com/Nezteb"><code>@​Nezteb</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/452">#452</a> - Assorted updates (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
</ul>
<h2>v4.0.0</h2>
<p>This release doesn't include any breaking changes, but due to updated development dependencies, tests are no longer run on Node 10.</p>
<ul>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/432">#432</a> - Updated dev dependencies and formatting (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/430">#430</a> - Bump ansi-regex from 3.0.0 to 3.0.1 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/431">#431</a> - Bump path-parse from 1.0.6 to 1.0.7 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/427">#427</a> - Bump async from 2.6.1 to 2.6.4 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/423">#423</a> - Bump minimist from 1.2.5 to 1.2.6 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
</ul>
<h2>v3.2.3</h2>
<ul>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/398">#398</a> - Update glob-parent (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/395">#395</a> - Switch from filenamify-url to filenamify (<a href="https://github.com/tw0517tw"><code>@​tw0517tw</code></a>)</li>
</ul>
<h2>v3.2.2</h2>
<ul>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/396">#396</a> - Revert &quot;security(deps): bump filenamify-url to 2.1.1&quot; (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
</ul>
<h2>v3.2.1</h2>
<ul>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/393">#393</a> - security(deps): bump filenamify-url to 2.1.1 (<a href="https://github.com/AviVahl"><code>@​AviVahl</code></a>)</li>
</ul>
<h2>v3.2.0</h2>
<p>This release updates a few development dependencies and adds a bit of documentation.</p>
<ul>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/391">#391</a> - Update dev dependencies (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/375">#375</a> - Add note about domain problem (<a href="https://github.com/demee"><code>@​demee</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/390">#390</a> - Fix little typo in the README (<a href="https://github.com/cizordj"><code>@​cizordj</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/388">#388</a> - Bump hosted-git-info from 2.8.8 to 2.8.9 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/387">#387</a> - Bump y18n from 4.0.0 to 4.0.3 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/378">#378</a> - Add GitHub Actions tips to readme.md (<a href="https://github.com/mickelsonmichael"><code>@​mickelsonmichael</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/386">#386</a> - Bump lodash from 4.17.14 to 4.17.21 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tschaub/gh-pages/commit/f729b97ab9b60121ff36853bfcfd6d716f43ac69"><code>f729b97</code></a> 5.0.0</li>
<li><a href="https://github.com/tschaub/gh-pages/commit/51534c798c20449826abebb0bd58b9e9ab04e20e"><code>51534c7</code></a> Log changes</li>
<li><a href="https://github.com/tschaub/gh-pages/commit/ace063b81fd3e74467671749c0e60ece1601f292"><code>ace063b</code></a> Merge pull request <a href="https://redirect.github.com/tschaub/gh-pages/issues/438">#438</a> from Vicropht/patch-1</li>
<li><a href="https://github.com/tschaub/gh-pages/commit/58e54be6248d33a283ddb5c6b335d342424956cc"><code>58e54be</code></a> Merge pull request <a href="https://redirect.github.com/tschaub/gh-pages/issues/459">#459</a> from tschaub/dependabot/npm_and_yarn/async-3.2.4</li>
<li><a href="https://github.com/tschaub/gh-pages/commit/2189df392e42e4fa5c4a5f2b9978d068adf084b0"><code>2189df3</code></a> Bump async from 2.6.4 to 3.2.4</li>
<li><a href="https://github.com/tschaub/gh-pages/commit/051846ed1c1ce657549170f985bbd0d1975b6a9f"><code>051846e</code></a> Merge pull request <a href="https://redirect.github.com/tschaub/gh-pages/issues/454">#454</a> from tschaub/dependabot/npm_and_yarn/email-addresses-...</li>
<li><a href="https://github.com/tschaub/gh-pages/commit/5c91c678c510b1f232e3c81753103d10f415431c"><code>5c91c67</code></a> Merge pull request <a href="https://redirect.github.com/tschaub/gh-pages/issues/455">#455</a> from tschaub/dependabot/github_actions/actions/setup-...</li>
<li><a href="https://github.com/tschaub/gh-pages/commit/fe0ad832548b3042814e53c9fe7417c32474da20"><code>fe0ad83</code></a> Merge pull request <a href="https://redirect.github.com/tschaub/gh-pages/issues/453">#453</a> from tschaub/dependabot/github_actions/actions/checko...</li>
<li><a href="https://github.com/tschaub/gh-pages/commit/b89287d04677be890a09ac4a699876e5884e245a"><code>b89287d</code></a> Merge pull request <a href="https://redirect.github.com/tschaub/gh-pages/issues/445">#445</a> from Nezteb/patch-1</li>
<li><a href="https://github.com/tschaub/gh-pages/commit/e890bd180ca99287f3be62033c64904a5bf39e7a"><code>e890bd1</code></a> Bump email-addresses from 3.0.1 to 5.0.0</li>
<li>Additional commits viewable in <a href="https://github.com/tschaub/gh-pages/compare/v2.2.0...v5.0.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=gh-pages&package-manager=npm_and_yarn&previous-version=2.2.0&new-version=5.0.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-23 00:20:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3231" class=".btn">#3231</a>
            </td>
            <td>
                <b>
                    build(deps): bump rustls from 0.21.9 to 0.21.11 in /packages/cactus-core-api
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [rustls](https://github.com/rustls/rustls) from 0.21.9 to 0.21.11.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/rustls/rustls/commit/7b8d1dbc1e666dc4d83640c64e96d257d39cfda4"><code>7b8d1db</code></a> Prepare 0.21.11</li>
<li><a href="https://github.com/rustls/rustls/commit/ebcb4782f23b4edf9b10a7065d9e8d4362439d9c"><code>ebcb478</code></a> complete_io: bail out if progress is impossible</li>
<li><a href="https://github.com/rustls/rustls/commit/20f35dfb6d3c353294c562723d4cb6639a8bd01b"><code>20f35df</code></a> Regression test for <code>complete_io</code> infinite loop bug</li>
<li><a href="https://github.com/rustls/rustls/commit/2f2aae15a4293639669291ab2b257835a2d4bdca"><code>2f2aae1</code></a> Don't specially handle unauthenticated close_notify alerts</li>
<li><a href="https://github.com/rustls/rustls/commit/e163587b985c894a6ce651992b91eb6897edde8b"><code>e163587</code></a> Don't deny warnings from nightly clippy</li>
<li><a href="https://github.com/rustls/rustls/commit/9f864874cff7d977cccd4204463ea34fd161a2fe"><code>9f86487</code></a> server::handy: fix new nightly clippy lint</li>
<li><a href="https://github.com/rustls/rustls/commit/7e0e8ab599a19c2a733be294aaf91eeb6fdebaaa"><code>7e0e8ab</code></a> Correct assorted clippy warnings in test code</li>
<li><a href="https://github.com/rustls/rustls/commit/3587d98f4ea434495facc0688b8b07313cb02e4a"><code>3587d98</code></a> Apply clippy suggestions from Rust 1.72</li>
<li><a href="https://github.com/rustls/rustls/commit/d082e837b34c0605b1851e45c421c91c1d15391c"><code>d082e83</code></a> Address <code>clippy::redundant_static_lifetimes</code></li>
<li><a href="https://github.com/rustls/rustls/commit/5e7a06ca457a6fe67dfbb57193f55138be7ef611"><code>5e7a06c</code></a> Address <code>clippy::slow_vector_initialization</code></li>
<li>Additional commits viewable in <a href="https://github.com/rustls/rustls/compare/v/0.21.9...v/0.21.11">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=rustls&package-manager=cargo&previous-version=0.21.9&new-version=0.21.11)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-19 20:01:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3230" class=".btn">#3230</a>
            </td>
            <td>
                <b>
                    build(deps): bump rustls from 0.21.10 to 0.21.11 in /weaver/common/protos-rs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [rustls](https://github.com/rustls/rustls) from 0.21.10 to 0.21.11.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/rustls/rustls/commit/7b8d1dbc1e666dc4d83640c64e96d257d39cfda4"><code>7b8d1db</code></a> Prepare 0.21.11</li>
<li><a href="https://github.com/rustls/rustls/commit/ebcb4782f23b4edf9b10a7065d9e8d4362439d9c"><code>ebcb478</code></a> complete_io: bail out if progress is impossible</li>
<li><a href="https://github.com/rustls/rustls/commit/20f35dfb6d3c353294c562723d4cb6639a8bd01b"><code>20f35df</code></a> Regression test for <code>complete_io</code> infinite loop bug</li>
<li><a href="https://github.com/rustls/rustls/commit/2f2aae15a4293639669291ab2b257835a2d4bdca"><code>2f2aae1</code></a> Don't specially handle unauthenticated close_notify alerts</li>
<li><a href="https://github.com/rustls/rustls/commit/e163587b985c894a6ce651992b91eb6897edde8b"><code>e163587</code></a> Don't deny warnings from nightly clippy</li>
<li><a href="https://github.com/rustls/rustls/commit/9f864874cff7d977cccd4204463ea34fd161a2fe"><code>9f86487</code></a> server::handy: fix new nightly clippy lint</li>
<li><a href="https://github.com/rustls/rustls/commit/7e0e8ab599a19c2a733be294aaf91eeb6fdebaaa"><code>7e0e8ab</code></a> Correct assorted clippy warnings in test code</li>
<li><a href="https://github.com/rustls/rustls/commit/3587d98f4ea434495facc0688b8b07313cb02e4a"><code>3587d98</code></a> Apply clippy suggestions from Rust 1.72</li>
<li><a href="https://github.com/rustls/rustls/commit/d082e837b34c0605b1851e45c421c91c1d15391c"><code>d082e83</code></a> Address <code>clippy::redundant_static_lifetimes</code></li>
<li><a href="https://github.com/rustls/rustls/commit/5e7a06ca457a6fe67dfbb57193f55138be7ef611"><code>5e7a06c</code></a> Address <code>clippy::slow_vector_initialization</code></li>
<li>Additional commits viewable in <a href="https://github.com/rustls/rustls/compare/v/0.21.10...v/0.21.11">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=rustls&package-manager=cargo&previous-version=0.21.10&new-version=0.21.11)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-19 19:51:56 +0000 UTC
    </div>
</div>

