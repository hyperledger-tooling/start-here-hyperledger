---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2961" class=".btn">#2961</a>
            </td>
            <td>
                <b>
                    feat: update context getDIDs() with didComm V2 format
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                Also update new Authcrypt packer to return FromKey in Unpack() as it's needed in the framework to fetch DID connections.

Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-26 15:36:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2959" class=".btn">#2959</a>
            </td>
            <td>
                <b>
                    fix: rewrite util/time to save a time string instead of using zero-counting logic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes issues in parsing acapy time strings, generalizing the previous solution to allow any input document to be processed (eg, verify proof) without reformatting time values.

Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-25 21:35:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2958" class=".btn">#2958</a>
            </td>
            <td>
                <b>
                    chore(deps): bump codecov/codecov-action from 2.0.2 to 2.0.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [codecov/codecov-action](https://github.com/codecov/codecov-action) from 2.0.2 to 2.0.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/codecov/codecov-action/releases">codecov/codecov-action's releases</a>.</em></p>
<blockquote>
<h2>v2.0.3</h2>
<h2>2.0.3</h2>
<h3>Fixes</h3>
<ul>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/464">#464</a> Fix wrong link in the readme</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/485">#485</a> fix: Add override OS and linux default to platform</li>
</ul>
<h3>Dependencies</h3>
<ul>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/447">#447</a> build(deps): bump openpgp from 5.0.0-4 to 5.0.0-5</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/458">#458</a> build(deps-dev): bump eslint from 7.31.0 to 7.32.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/465">#465</a> build(deps-dev): bump <code>@​typescript-eslint/eslint-plugin</code> from 4.28.4 to 4.29.1</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/466">#466</a> build(deps-dev): bump <code>@​typescript-eslint/parser</code> from 4.28.4 to 4.29.1</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/468">#468</a> build(deps-dev): bump <code>@​types/jest</code> from 26.0.24 to 27.0.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/470">#470</a> build(deps-dev): bump <code>@​types/node</code> from 16.4.0 to 16.6.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/472">#472</a> build(deps): bump path-parse from 1.0.6 to 1.0.7</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/473">#473</a> build(deps-dev): bump <code>@​types/jest</code> from 27.0.0 to 27.0.1</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/478">#478</a> build(deps-dev): bump <code>@​typescript-eslint/parser</code> from 4.29.1 to 4.29.2</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/479">#479</a> build(deps-dev): bump <code>@​typescript-eslint/eslint-plugin</code> from 4.29.1 to 4.29.2</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/481">#481</a> build(deps-dev): bump <code>@​types/node</code> from 16.6.0 to 16.6.2</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/483">#483</a> build(deps-dev): bump <code>@​vercel/ncc</code> from 0.29.0 to 0.29.2</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/484">#484</a> build(deps): bump <code>@​actions/core</code> from 1.4.0 to 1.5.0</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/codecov/codecov-action/blob/master/CHANGELOG.md">codecov/codecov-action's changelog</a>.</em></p>
<blockquote>
<h2>2.0.3</h2>
<h3>Fixes</h3>
<ul>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/464">#464</a> Fix wrong link in the readme</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/485">#485</a> fix: Add override OS and linux default to platform</li>
</ul>
<h3>Dependencies</h3>
<ul>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/447">#447</a> build(deps): bump openpgp from 5.0.0-4 to 5.0.0-5</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/458">#458</a> build(deps-dev): bump eslint from 7.31.0 to 7.32.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/465">#465</a> build(deps-dev): bump <code>@​typescript-eslint/eslint-plugin</code> from 4.28.4 to 4.29.1</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/466">#466</a> build(deps-dev): bump <code>@​typescript-eslint/parser</code> from 4.28.4 to 4.29.1</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/468">#468</a> build(deps-dev): bump <code>@​types/jest</code> from 26.0.24 to 27.0.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/470">#470</a> build(deps-dev): bump <code>@​types/node</code> from 16.4.0 to 16.6.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/472">#472</a> build(deps): bump path-parse from 1.0.6 to 1.0.7</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/473">#473</a> build(deps-dev): bump <code>@​types/jest</code> from 27.0.0 to 27.0.1</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/478">#478</a> build(deps-dev): bump <code>@​typescript-eslint/parser</code> from 4.29.1 to 4.29.2</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/479">#479</a> build(deps-dev): bump <code>@​typescript-eslint/eslint-plugin</code> from 4.29.1 to 4.29.2</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/481">#481</a> build(deps-dev): bump <code>@​types/node</code> from 16.6.0 to 16.6.2</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/483">#483</a> build(deps-dev): bump <code>@​vercel/ncc</code> from 0.29.0 to 0.29.2</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/484">#484</a> build(deps): bump <code>@​actions/core</code> from 1.4.0 to 1.5.0</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/codecov/codecov-action/commit/5a8bb4701eca7ba3673f21664b887f652c58d0a3"><code>5a8bb47</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/485">#485</a> from codecov/alternate-os</li>
<li><a href="https://github.com/codecov/codecov-action/commit/3e9a2814f275c203e54e7d52a37d6510f7b927c0"><code>3e9a281</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/481">#481</a> from codecov/dependabot/npm_and_yarn/types/node-16.6.2</li>
<li><a href="https://github.com/codecov/codecov-action/commit/6feb914f258d64e26a6821b9e5c299734cdf0063"><code>6feb914</code></a> chore: Update CHANGELOG</li>
<li><a href="https://github.com/codecov/codecov-action/commit/9f40d310dd9118c73b76b8f8cb2040347db674bc"><code>9f40d31</code></a> build(deps-dev): bump <code>@​types/node</code> from 16.6.0 to 16.6.2</li>
<li><a href="https://github.com/codecov/codecov-action/commit/c4e74feb726d24e316fe82a00e5b134cc1488a39"><code>c4e74fe</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/483">#483</a> from codecov/dependabot/npm_and_yarn/vercel/ncc-0.29.2</li>
<li><a href="https://github.com/codecov/codecov-action/commit/6ba3fb33c76727f4d10d9155bbd82d3bfe86fbc5"><code>6ba3fb3</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/479">#479</a> from codecov/dependabot/npm_and_yarn/typescript-eslin...</li>
<li><a href="https://github.com/codecov/codecov-action/commit/7efb9be09a656c6f53dfeb11dc4fdd8e4272362d"><code>7efb9be</code></a> build(deps-dev): bump <code>@​typescript-eslint/eslint-plugin</code></li>
<li><a href="https://github.com/codecov/codecov-action/commit/514990d4ef0e7a59fa01d3c0c0f16c8e41fe1e1a"><code>514990d</code></a> build(deps-dev): bump <code>@​vercel/ncc</code> from 0.29.0 to 0.29.2</li>
<li><a href="https://github.com/codecov/codecov-action/commit/cd6db5e3130cd4b4a180ce3d742a97ecfe34061c"><code>cd6db5e</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/484">#484</a> from codecov/dependabot/npm_and_yarn/actions/core-1.5.0</li>
<li><a href="https://github.com/codecov/codecov-action/commit/678cc77a4f5fd03937f21a0f627cc07002d9c99b"><code>678cc77</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/478">#478</a> from codecov/dependabot/npm_and_yarn/typescript-eslin...</li>
<li>Additional commits viewable in <a href="https://github.com/codecov/codecov-action/compare/v2.0.2...v2.0.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=codecov/codecov-action&package-manager=github_actions&previous-version=2.0.2&new-version=2.0.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-25 08:18:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2957" class=".btn">#2957</a>
            </td>
            <td>
                <b>
                    docs: update WACI universal wallet interface reference
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Since WACI interfaces are now updated in universal wallet spec, aries
vcwallet documentations are updated to refer WACI interfaces.

Part of #2433

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-25 01:42:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2956" class=".btn">#2956</a>
            </td>
            <td>
                <b>
                    feat: acapy issue-credential v2 interop support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes & improvements:
- `/kms/import` accepts BLS12381_G2 private keys.
- `/verifiable` commands try to pick verification methods that match
  the requested crypto suite for signing.
- Supports raw base64 fields in proof parsing.
- Supports bbs signature verification through public key verifier
  SignatureVerifier.
- time.Time wrapper handles timestrings without a timezone suffix,
  and will transparently marshal with/without the suffix, as its
  source string was.

Interop tweaks:
- Fixes for handling acapy "peer" DID docs.

Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-23 21:40:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2955" class=".btn">#2955</a>
            </td>
            <td>
                <b>
                    WIP: feat: Present proof v3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrii Soluk <isoluchok@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-23 12:16:50 +0000 UTC
    </div>
</div>

