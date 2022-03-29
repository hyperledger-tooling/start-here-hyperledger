---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1948" class=".btn">#1948</a>
            </td>
            <td>
                <b>
                    fix(security): ensure node-forge > 1.3.0 for CVE-2022-24772
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">Security</span><span class="chip">P1</span>
            </td>
            <td>
                This is a temporary fix until our direct dependencies get patched
which we can update for ourselves. In the meantime this will force
the (currently considered) secure versions of node-forge to be used.
 
Fixes #1947

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>   

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-23 18:05:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1946" class=".btn">#1946</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump electron from 13.3.0 to 13.6.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [electron](https://github.com/electron/electron) from 13.3.0 to 13.6.6.
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
<li>Additional commits viewable in <a href="https://github.com/electron/electron/compare/v13.3.0...v13.6.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=electron&package-manager=npm_and_yarn&previous-version=13.3.0&new-version=13.6.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cactus/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-23 08:11:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1944" class=".btn">#1944</a>
            </td>
            <td>
                <b>
                    fix(deps): force minimist >=1.2.6 for CVE-2021-44906
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">Security</span><span class="chip">P1</span>
            </td>
            <td>
                Ensures that yarn will only install 1.2.6 or newer versions for
minimist.

The proper fix would be to have the dependencies issue releases
which upgrade their own (transitive) dependencies of minimist
so that we don't have to explicitly force it here, but at the time
of this writing these upgrades in our direct dependencies are just
not available yet.

Fixes #1943

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-23 04:54:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1942" class=".btn">#1942</a>
            </td>
            <td>
                <b>
                    replaced rocketchat with discord
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Replaced the old rocketchat link with the new discord link
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-22 19:09:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1940" class=".btn">#1940</a>
            </td>
            <td>
                <b>
                    feat(keychain-aws-sm): bootstrap readme.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Commit to be reviewed

feat(keychain-aws-sm): bootstrap readme.md

	Primary Changes
	-----------------------
	1. Updated the README.md located at packages/cactus-plugin-keychain-aws-sm/README.md
	2. The aws secret manager plugin now includes the prometheus metrics exporter integration
	3. OpenApi spec now has api endpoint for getting the prometheus metrics

Fixes #968

Signed-off-by: jagpreetsinghsasan <jagpreet.singh.sasan@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-22 10:19:58 +0000 UTC
    </div>
</div>

