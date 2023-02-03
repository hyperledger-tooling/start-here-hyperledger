---
layout: default
title: aries-javascript-docs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-javascript-docs
---

# aries-javascript-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-javascript-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-javascript-docs/pull/93" class=".btn">#93</a>
            </td>
            <td>
                <b>
                    build(deps): bump ua-parser-js from 0.7.31 to 0.7.33
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [ua-parser-js](https://github.com/faisalman/ua-parser-js) from 0.7.31 to 0.7.33.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/faisalman/ua-parser-js/blob/master/changelog.md">ua-parser-js's changelog</a>.</em></p>
<blockquote>
<h2>Version 0.7.31 / 1.0.2</h2>
<ul>
<li>Fix OPPO Reno A5 incorrect detection</li>
<li>Fix TypeError Bug</li>
<li>Use AST to extract regexes and verify them with safe-regex</li>
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
<h2>Version 0.7.33 / 1.0.33</h2>
<ul>
<li>Add new browser : Cobalt</li>
<li>Identify Macintosh as an Apple device</li>
<li>Fix ReDoS vulnerability</li>
</ul>
<h1>Version 0.8</h1>
<p>Version 0.8 was created by accident. This version is now deprecated and no longer maintained, please update to version 0.7 / 1.0.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/f2d0db001d87da15de7b9b1df7be9f2eacefd8c5"><code>f2d0db0</code></a> Bump version 0.7.33</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/a6140a17dd0300a35cfc9cff999545f267889411"><code>a6140a1</code></a> Remove unsafe regex in trim() function</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/a88660493568d6144a551424a8139d6c876635f6"><code>a886604</code></a> Fix <a href="https://github-redirect.dependabot.com/faisalman/ua-parser-js/issues/605">#605</a> - Identify Macintosh as Apple device</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/b814bcd79198e730936c82462e2d729eb5423e3c"><code>b814bcd</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/faisalman/ua-parser-js/issues/606">#606</a> from rileyjshaw/patch-1</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/7f71024161399b7aa5d5cd10dba9e059f0218262"><code>7f71024</code></a> Fix documentation</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/c239ac5167abd574a635cb809a2b4fa35810d23b"><code>c239ac5</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/faisalman/ua-parser-js/issues/604">#604</a> from obecerra3/master</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/8d3c2d327cf540ff2c050f1cc67bca8c6f8e4458"><code>8d3c2d3</code></a> Add new browser: Cobalt</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/d11fc47dc9b6acc0f89fc10c120cea08e10cd31a"><code>d11fc47</code></a> Bump version 0.7.32</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/b490110109de586deab96c775c9ef0dfc9c919c4"><code>b490110</code></a> Merge branch 'develop' of github.com:faisalman/ua-parser-js</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/cb5da5ea4b220d5b60fe209e123b7f911d8e0d4a"><code>cb5da5e</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/faisalman/ua-parser-js/issues/600">#600</a> from moekm/develop</li>
<li>Additional commits viewable in <a href="https://github.com/faisalman/ua-parser-js/compare/0.7.31...0.7.33">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ua-parser-js&package-manager=npm_and_yarn&previous-version=0.7.31&new-version=0.7.33)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-javascript-docs/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-27 12:30:14 +0000 UTC
    </div>
</div>

