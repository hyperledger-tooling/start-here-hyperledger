---
layout: default
title: aries-framework-javascript-ext
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript-ext
---

# aries-framework-javascript-ext <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript-ext){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript-ext/pull/104" class=".btn">#104</a>
            </td>
            <td>
                <b>
                    chore: release @aries-framework/rest 0.8.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">autorelease: pending</span>
            </td>
            <td>
                :robot: I have created a release \*beep\* \*boop\*
---
### [0.8.1](https://www.github.com/hyperledger/aries-framework-javascript-ext/compare/rest-v0.8.0...rest-v0.8.1) (2022-03-09)


### Features

* **rest:** added multi use param to create invitation ([#100](https://www.github.com/hyperledger/aries-framework-javascript-ext/issues/100)) ([d00f11d](https://www.github.com/hyperledger/aries-framework-javascript-ext/commit/d00f11d78e9f65de3907bd6bf94dd6c38e2ddc3b))
---


This PR was generated with [Release Please](https://github.com/googleapis/release-please). See [documentation](https://github.com/googleapis/release-please#release-please).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-09 09:57:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript-ext/pull/103" class=".btn">#103</a>
            </td>
            <td>
                <b>
                    build(deps): bump urijs from 1.19.8 to 1.19.10
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [urijs](https://github.com/medialize/URI.js) from 1.19.8 to 1.19.10.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/medialize/URI.js/releases">urijs's releases</a>.</em></p>
<blockquote>
<h2>1.19.10 (March 5th 2022)</h2>
<ul>
<li><strong>SECURITY</strong> fixing <a href="http://medialize.github.io/URI.js/docs.html#static-parse"><code>URI.parse()</code></a> handle excessive colons in protocol delimiter - disclosed by <a href="https://github.com/huydoppa">huydoppa</a> via <a href="https://huntr.dev/">https://huntr.dev/</a></li>
</ul>
<h2>1.19.9 (March 3rd 2022)</h2>
<ul>
<li><strong>SECURITY</strong> fixing <a href="http://medialize.github.io/URI.js/docs.html#static-parse"><code>URI.parse()</code></a> handle leading whitespace - disclosed by <a href="https://github.com/p0cas">p0cas</a> via <a href="https://huntr.dev/">https://huntr.dev/</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/medialize/URI.js/blob/gh-pages/CHANGELOG.md">urijs's changelog</a>.</em></p>
<blockquote>
<h3>1.19.10 (March 5th 2022)</h3>
<ul>
<li><strong>SECURITY</strong> fixing <a href="http://medialize.github.io/URI.js/docs.html#static-parse"><code>URI.parse()</code></a> handle excessive colons in protocol delimiter - disclosed by <a href="https://github.com/huydoppa">huydoppa</a> via <a href="https://huntr.dev/">https://huntr.dev/</a></li>
</ul>
<h3>1.19.9 (March 3rd 2022)</h3>
<ul>
<li><strong>SECURITY</strong> fixing <a href="http://medialize.github.io/URI.js/docs.html#static-parse"><code>URI.parse()</code></a> handle leading whitespace - disclosed by <a href="https://github.com/p0cas">p0cas</a> via <a href="https://huntr.dev/">https://huntr.dev/</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/medialize/URI.js/commit/926b2aa1099f177f82d0a998da4b43e69fe56ec8"><code>926b2aa</code></a> chore(build): bumping to version 1.19.10</li>
<li><a href="https://github.com/medialize/URI.js/commit/a8166fe02f3af6dc1b2b888dcbb807155aad9509"><code>a8166fe</code></a> fix(parse): handle excessive colons in scheme delimiter</li>
<li><a href="https://github.com/medialize/URI.js/commit/01920b5cda87d5dd726eab43d6e7f3ce34a2fd52"><code>01920b5</code></a> chore(build): bumping to version 1.19.9</li>
<li><a href="https://github.com/medialize/URI.js/commit/86d10523a6f6e8dc4300d99d671335ee362ad316"><code>86d1052</code></a> fix(parse): remove leading whitespace</li>
<li>See full diff in <a href="https://github.com/medialize/URI.js/compare/v1.19.8...v1.19.10">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=urijs&package-manager=npm_and_yarn&previous-version=1.19.8&new-version=1.19.10)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-javascript-ext/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-08 23:41:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript-ext/pull/102" class=".btn">#102</a>
            </td>
            <td>
                <b>
                    build: bump feature as patch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Only breaking changes will trigger minor releases now

Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-08 22:51:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript-ext/pull/100" class=".btn">#100</a>
            </td>
            <td>
                <b>
                    feat(rest): added multi use param to create invitation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jan <60812202+janrtvld@users.noreply.github.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-08 09:45:10 +0000 UTC
    </div>
</div>

