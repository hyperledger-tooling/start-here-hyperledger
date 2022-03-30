---
layout: default
title: aries-toolbox
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-toolbox
---

# aries-toolbox <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-toolbox){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-toolbox/pull/282" class=".btn">#282</a>
            </td>
            <td>
                <b>
                    feat: remove intermittently problematic console logs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Micah Peltier <micah6_8@yahoo.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 15:16:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-toolbox/pull/281" class=".btn">#281</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump electron from 12.2.3 to 13.6.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [electron](https://github.com/electron/electron) from 12.2.3 to 13.6.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/electron/electron/releases">electron's releases</a>.</em></p>
<blockquote>
<h2>electron v13.6.6</h2>
<h1>Release Notes for v13.6.6</h1>
<h2>Fixes</h2>
<ul>
<li>Fixed a JavaScript exception from webContents if render frame was disposed in WebFrameMain, resets the value of <code>render_frame_disposed_</code> after updating render frame host. <a href="https://github-redirect.dependabot.com/electron/electron/pull/32130">#32130</a> <!-- raw HTML omitted -->(Also in <a href="https://github-redirect.dependabot.com/electron/electron/pull/31425">14</a>, <a href="https://github-redirect.dependabot.com/electron/electron/pull/31426">15</a>, <a href="https://github-redirect.dependabot.com/electron/electron/pull/31427">16</a>)<!-- raw HTML omitted --></li>
<li>No Notes. <a href="https://github-redirect.dependabot.com/electron/electron/pull/32241">#32241</a> <!-- raw HTML omitted -->(Also in <a href="https://github-redirect.dependabot.com/electron/electron/pull/32242">14</a>, <a href="https://github-redirect.dependabot.com/electron/electron/pull/32245">15</a>, <a href="https://github-redirect.dependabot.com/electron/electron/pull/32243">16</a>, <a href="https://github-redirect.dependabot.com/electron/electron/pull/32244">17</a>)<!-- raw HTML omitted --></li>
</ul>
<h2>Other Changes</h2>
<ul>
<li>Backported fix for CVE-2021-4056. <a href="https://github-redirect.dependabot.com/electron/electron/pull/32237">#32237</a></li>
<li>Backported fix for CVE-2021-4057. <a href="https://github-redirect.dependabot.com/electron/electron/pull/32234">#32234</a></li>
<li>Backported fix for CVE-2021-4102. <a href="https://github-redirect.dependabot.com/electron/electron/pull/32194">#32194</a></li>
</ul>
<h2>electron v13.6.3</h2>
<h1>Release Notes for v13.6.3</h1>
<h2>Fixes</h2>
<ul>
<li>Fixed window frame glitch when calling <code>setContentProtection</code>. <a href="https://github-redirect.dependabot.com/electron/electron/pull/31829">#31829</a> <!-- raw HTML omitted -->(Also in <a href="https://github-redirect.dependabot.com/electron/electron/pull/31831">14</a>, <a href="https://github-redirect.dependabot.com/electron/electron/pull/31830">15</a>, <a href="https://github-redirect.dependabot.com/electron/electron/pull/31832">16</a>)<!-- raw HTML omitted --></li>
<li>Generate valid config.gypi file in Node.js headers. <a href="https://github-redirect.dependabot.com/electron/electron/pull/31989">#31989</a> <!-- raw HTML omitted -->(Also in <a href="https://github-redirect.dependabot.com/electron/electron/pull/31443">14</a>, <a href="https://github-redirect.dependabot.com/electron/electron/pull/31442">15</a>, <a href="https://github-redirect.dependabot.com/electron/electron/pull/31441">16</a>)<!-- raw HTML omitted --></li>
</ul>
<h2>Other Changes</h2>
<ul>
<li>Backported fix for CVE-2021-38005. <a href="https://github-redirect.dependabot.com/electron/electron/pull/31921">#31921</a></li>
<li>Backported fix for CVE-2021-38007. <a href="https://github-redirect.dependabot.com/electron/electron/pull/31912">#31912</a></li>
<li>Backported fix for CVE-2021-38011. <a href="https://github-redirect.dependabot.com/electron/electron/pull/31901">#31901</a></li>
</ul>
<h2>electron v13.6.2</h2>
<h1>Release Notes for v13.6.2</h1>
<h2>Fixes</h2>
<ul>
<li>Fixed an issue where <code>Content-Disposition</code> filenames would be incorrectly truncated at the first comma for a filename attachment which contained one. <a href="https://github-redirect.dependabot.com/electron/electron/pull/31691">#31691</a> <!-- raw HTML omitted -->(Also in <a href="https://github-redirect.dependabot.com/electron/electron/pull/31692">14</a>, <a href="https://github-redirect.dependabot.com/electron/electron/pull/31693">15</a>, <a href="https://github-redirect.dependabot.com/electron/electron/pull/31694">16</a>)<!-- raw HTML omitted --></li>
<li>Fixed an issue which caused print settings to not work properly when printing silently. <a href="https://github-redirect.dependabot.com/electron/electron/pull/31618">#31618</a> <!-- raw HTML omitted -->(Also in <a href="https://github-redirect.dependabot.com/electron/electron/pull/31617">14</a>, <a href="https://github-redirect.dependabot.com/electron/electron/pull/31616">15</a>, <a href="https://github-redirect.dependabot.com/electron/electron/pull/31615">16</a>)<!-- raw HTML omitted --></li>
</ul>
<h2>Other Changes</h2>
<ul>
<li>Backported fix for CVE-2021-37998. <a href="https://github-redirect.dependabot.com/electron/electron/pull/31678">#31678</a></li>
<li>Backported fix for CVE-2021-38001. <a href="https://github-redirect.dependabot.com/electron/electron/pull/31673">#31673</a></li>
<li>Backported fix for CVE-2021-38002. <a href="https://github-redirect.dependabot.com/electron/electron/pull/31671">#31671</a></li>
<li>Backported fix for CVE-2021-38003. <a href="https://github-redirect.dependabot.com/electron/electron/pull/31665">#31665</a></li>
<li>Backported fix for chromium:1252858. <a href="https://github-redirect.dependabot.com/electron/electron/pull/31682">#31682</a></li>
</ul>
<h2>electron v13.6.1</h2>
<h1>Release Notes for v13.6.1</h1>
<h2>Fixes</h2>
<ul>
<li>Fixed an issue where <code>MediaMetadata</code> did not work properly. <a href="https://github-redirect.dependabot.com/electron/electron/pull/31532">#31532</a> <!-- raw HTML omitted -->(Also in <a href="https://github-redirect.dependabot.com/electron/electron/pull/31533">14</a>, <a href="https://github-redirect.dependabot.com/electron/electron/pull/31534">15</a>, <a href="https://github-redirect.dependabot.com/electron/electron/pull/31535">16</a>)<!-- raw HTML omitted --></li>
<li>Fixed black window when screen capturing a content-protected BrowserWindow on Windows 10. <a href="https://github-redirect.dependabot.com/electron/electron/pull/31550">#31550</a> <!-- raw HTML omitted -->(Also in <a href="https://github-redirect.dependabot.com/electron/electron/pull/31551">14</a>, <a href="https://github-redirect.dependabot.com/electron/electron/pull/31385">15</a>, <a href="https://github-redirect.dependabot.com/electron/electron/pull/31386">16</a>)<!-- raw HTML omitted --></li>
</ul>
<h2>Other Changes</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/electron/electron/commit/776ee483306730531aa22dcdc67d6e08bd6571ce"><code>776ee48</code></a> Bump v13.6.6</li>
<li><a href="https://github.com/electron/electron/commit/8283f19403951dd0af7fe3a9de57879c9a2eccbb"><code>8283f19</code></a> fix: reset render_frame_disposed_ after render frame host change (<a href="https://github-redirect.dependabot.com/electron/electron/issues/32130">#32130</a>)</li>
<li><a href="https://github.com/electron/electron/commit/316f0bc8452b8d1810c9d35d23b083f7bfb41254"><code>316f0bc</code></a> chore: cherry-pick 2b978fb482 from chromium (<a href="https://github-redirect.dependabot.com/electron/electron/issues/32234">#32234</a>)</li>
<li><a href="https://github.com/electron/electron/commit/9b94d70194d1d4598dafa2b214704ac486b3728e"><code>9b94d70</code></a> chore: cherry-pick 04a58fedd5 from v8 (<a href="https://github-redirect.dependabot.com/electron/electron/issues/32237">#32237</a>)</li>
<li><a href="https://github.com/electron/electron/commit/ab94340567cc50002d578f9c8e2bd883cd2984e5"><code>ab94340</code></a> fix: check for single bluetooth listener (<a href="https://github-redirect.dependabot.com/electron/electron/issues/32241">#32241</a>)</li>
<li><a href="https://github.com/electron/electron/commit/ca112e2e4dde8da52cac5be84952272102c731ec"><code>ca112e2</code></a> chore: cherry-pick 418c276ef228 from v8 (<a href="https://github-redirect.dependabot.com/electron/electron/issues/32194">#32194</a>)</li>
<li><a href="https://github.com/electron/electron/commit/fd4b311d7e5dfdc5ee33b81379b57db8e5354ed9"><code>fd4b311</code></a> Bump v13.6.5</li>
<li><a href="https://github.com/electron/electron/commit/a22cfb6bef20c2367a1e140e766f3fc03c952574"><code>a22cfb6</code></a> Bump v13.6.4</li>
<li><a href="https://github.com/electron/electron/commit/bc669916bd9cf686adf5924caa9ba77d609aadcf"><code>bc66991</code></a> Revert &quot;Bump v13.6.4&quot; (<a href="https://github-redirect.dependabot.com/electron/electron/issues/32229">#32229</a>)</li>
<li><a href="https://github.com/electron/electron/commit/4067ec626317d974f3bc3a5166876389f5e92934"><code>4067ec6</code></a> Bump v13.6.4</li>
<li>Additional commits viewable in <a href="https://github.com/electron/electron/compare/v12.2.3...v13.6.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=electron&package-manager=npm_and_yarn&previous-version=12.2.3&new-version=13.6.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-toolbox/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-25 19:24:48 +0000 UTC
    </div>
</div>

