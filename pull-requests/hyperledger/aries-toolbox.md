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
                PR <a href="https://github.com/hyperledger/aries-toolbox/pull/319" class=".btn">#319</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump got and electron
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [got](https://github.com/sindresorhus/got) to 11.8.6 and updates ancestor dependency [electron](https://github.com/electron/electron). These dependencies need to be updated together.

Updates `got` from 11.8.3 to 11.8.6
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sindresorhus/got/releases">got's releases</a>.</em></p>
<blockquote>
<h2>v11.8.6</h2>
<ul>
<li>Destroy request object after successful response</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v11.8.5...v11.8.6">https://github.com/sindresorhus/got/compare/v11.8.5...v11.8.6</a></p>
<h2>v11.8.5</h2>
<ul>
<li>Backport security fix <a href="https://github.com/sindresorhus/got/commit/861ccd9ac2237df762a9e2beed7edd88c60782dc">https://github.com/sindresorhus/got/commit/861ccd9ac2237df762a9e2beed7edd88c60782dc</a>
<ul>
<li><a href="https://nvd.nist.gov/vuln/detail/CVE-2022-33987">CVE-2022-33987</a></li>
</ul>
</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v11.8.4...v11.8.5">https://github.com/sindresorhus/got/compare/v11.8.4...v11.8.5</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sindresorhus/got/commit/2b1482ca847867cbf24abde4d68e8063611e50d1"><code>2b1482c</code></a> 11.8.6</li>
<li><a href="https://github.com/sindresorhus/got/commit/2d1497e71288995100c6d90eaee3c9e5b38039e0"><code>2d1497e</code></a> Destroy request object after successful response (<a href="https://redirect.github.com/sindresorhus/got/issues/2187">#2187</a>)</li>
<li><a href="https://github.com/sindresorhus/got/commit/5e17bb748c260b02e4cf716c2f4079a1c6a7481e"><code>5e17bb7</code></a> 11.8.5</li>
<li><a href="https://github.com/sindresorhus/got/commit/bce8ce7d528a675bd5a8d996e110b73674e290d2"><code>bce8ce7</code></a> Backport 861ccd9ac2237df762a9e2beed7edd88c60782dc</li>
<li><a href="https://github.com/sindresorhus/got/commit/8ced19215603f3eda25a9f5dce390f1b152fe9a3"><code>8ced192</code></a> Fix build</li>
<li><a href="https://github.com/sindresorhus/got/commit/670eb04b5b01622f489277d6fb1dd04a41d3cb51"><code>670eb04</code></a> 11.8.4</li>
<li><a href="https://github.com/sindresorhus/got/commit/20f29fe3726a4ddd104f557456dbd5275685e879"><code>20f29fe</code></a> Backport <a href="https://redirect.github.com/sindresorhus/got/issues/1543">#1543</a>: Initialize globalResponse in case of ignored HTTPError (<a href="https://redirect.github.com/sindresorhus/got/issues/2017">#2017</a>)</li>
<li>See full diff in <a href="https://github.com/sindresorhus/got/compare/v11.8.3...v11.8.6">compare view</a></li>
</ul>
</details>
<br />

Updates `electron` from 13.6.6 to 23.2.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/electron/electron/releases">electron's releases</a>.</em></p>
<blockquote>
<h2>electron v23.2.1</h2>
<h1>Release Notes for v23.2.1</h1>
<h2>Fixes</h2>
<ul>
<li>Fixed an issue where calling <code>port.postMessage</code> in <code>MessagePortMain</code> with some invalid parameters could cause a crash. <a href="https://redirect.github.com/electron/electron/pull/37724">#37724</a> <!-- raw HTML omitted -->(Also in <a href="https://redirect.github.com/electron/electron/pull/37725">22</a>, <a href="https://redirect.github.com/electron/electron/pull/37726">24</a>)<!-- raw HTML omitted --></li>
<li>Fixed canceling of bluetooth requests when no devices are returned. <a href="https://redirect.github.com/electron/electron/pull/37720">#37720</a> <!-- raw HTML omitted -->(Also in <a href="https://redirect.github.com/electron/electron/pull/37717">24</a>)<!-- raw HTML omitted --></li>
</ul>
<h2>Other Changes</h2>
<ul>
<li>Security: backported fix for CVE-2023-1213. <a href="https://redirect.github.com/electron/electron/pull/37708">#37708</a></li>
<li>Updated Chromium to 110.0.5481.208. <a href="https://redirect.github.com/electron/electron/pull/37645">#37645</a></li>
</ul>
<h2>electron v23.2.0</h2>
<h1>Release Notes for v23.2.0</h1>
<h2>Features</h2>
<ul>
<li>Added the <code>enableLocalEcho</code> flag to the session handler <code>ses.setDisplayMediaRequestHandler()</code> callback for allowing remote audio input to be echoed in the local output stream when <code>audio</code> is a <code>WebFrameMain</code>. <a href="https://redirect.github.com/electron/electron/pull/37529">#37529</a> <!-- raw HTML omitted -->(Also in <a href="https://redirect.github.com/electron/electron/pull/37528">24</a>)<!-- raw HTML omitted --></li>
</ul>
<h2>Fixes</h2>
<ul>
<li>Fixed an issue where <code>BroadcastChannel</code> did not work correctly when <code>contextIsolation: false</code>. <a href="https://redirect.github.com/electron/electron/pull/37444">#37444</a> <!-- raw HTML omitted -->(Also in <a href="https://redirect.github.com/electron/electron/pull/37443">24</a>)<!-- raw HTML omitted --></li>
<li>Fixed an issue with potential dock icon duplication on macOS. <a href="https://redirect.github.com/electron/electron/pull/37624">#37624</a> <!-- raw HTML omitted -->(Also in <a href="https://redirect.github.com/electron/electron/pull/37623">22</a>, <a href="https://redirect.github.com/electron/electron/pull/37625">24</a>)<!-- raw HTML omitted --></li>
<li>Fixed issue with BrowserWindow not updating after call to previewFile. <a href="https://redirect.github.com/electron/electron/pull/37577">#37577</a> <!-- raw HTML omitted -->(Also in <a href="https://redirect.github.com/electron/electron/pull/37576">22</a>, <a href="https://redirect.github.com/electron/electron/pull/37578">24</a>)<!-- raw HTML omitted --></li>
<li>Improved error messages on <code>session.cookies.set</code> failure. <a href="https://redirect.github.com/electron/electron/pull/37596">#37596</a> <!-- raw HTML omitted -->(Also in <a href="https://redirect.github.com/electron/electron/pull/37595">22</a>, <a href="https://redirect.github.com/electron/electron/pull/37597">24</a>)<!-- raw HTML omitted --></li>
</ul>
<h2>electron v23.1.4</h2>
<h1>Release Notes for v23.1.4</h1>
<h2>Fixes</h2>
<ul>
<li>Fixed an issue where unhandled rejections could cause duplicate logs in some cases. <a href="https://redirect.github.com/electron/electron/pull/37501">#37501</a> <!-- raw HTML omitted -->(Also in <a href="https://redirect.github.com/electron/electron/pull/37502">22</a>, <a href="https://redirect.github.com/electron/electron/pull/37500">24</a>)<!-- raw HTML omitted --></li>
</ul>
<h2>Other Changes</h2>
<ul>
<li>Updated Chromium to 110.0.5481.192. <a href="https://redirect.github.com/electron/electron/pull/37533">#37533</a></li>
</ul>
<h2>electron v23.1.3</h2>
<h1>Release Notes for v23.1.3</h1>
<h2>Fixes</h2>
<ul>
<li>Fixed WebUSB on ARM64 macs. <a href="https://redirect.github.com/electron/electron/pull/37521">#37521</a> <!-- raw HTML omitted -->(Also in <a href="https://redirect.github.com/electron/electron/pull/37522">24</a>)<!-- raw HTML omitted --></li>
<li>Fixed a crash on capturing sources when using desktopCapturer API on Wayland. <a href="https://redirect.github.com/electron/electron/pull/37526">#37526</a></li>
</ul>
<h2>Other Changes</h2>
<ul>
<li>Updated Chromium to 110.0.5481.179. <a href="https://redirect.github.com/electron/electron/pull/37471">#37471</a></li>
</ul>
<h2>electron v23.1.2</h2>
<h1>Release Notes for v23.1.2</h1>
<h2>Fixes</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/electron/electron/commit/96ee0b7c36763b4abeddd1f3818147e97467542a"><code>96ee0b7</code></a> docs: updated package.json content and electron version in build first app gu...</li>
<li><a href="https://github.com/electron/electron/commit/9e4d81fb0b76ef88606ecd4b29fffde98b995d24"><code>9e4d81f</code></a> fix: allow cancelling of bluetooth requests (<a href="https://redirect.github.com/electron/electron/issues/37720">#37720</a>)</li>
<li><a href="https://github.com/electron/electron/commit/9bcb5dc9f7848b7f00bb746375197760060704c4"><code>9bcb5dc</code></a> chore: generator objects can't be sent over the context bridge (<a href="https://redirect.github.com/electron/electron/issues/37729">#37729</a>)</li>
<li><a href="https://github.com/electron/electron/commit/62540b9120d979e7f95c7fa26edb2ebbfc5606da"><code>62540b9</code></a> fix: crash in <code>MessagePortMain</code> with some <code>postMessage</code> params (<a href="https://redirect.github.com/electron/electron/issues/37724">#37724</a>)</li>
<li><a href="https://github.com/electron/electron/commit/ee9484e05c0dff15ee8b46e8d55df684bc41dd6b"><code>ee9484e</code></a> docs: fixup incorrect value for disabling sandbox (<a href="https://redirect.github.com/electron/electron/issues/37721">#37721</a>)</li>
<li><a href="https://github.com/electron/electron/commit/3adb49a8319bf43f6991e685635cf6fd40aa4aac"><code>3adb49a</code></a> ci: fixup gn check to actually run gn check (<a href="https://redirect.github.com/electron/electron/issues/37680">#37680</a>)</li>
<li><a href="https://github.com/electron/electron/commit/6da4c2f12a8d04a0e952b4a7b14fcc026db52b62"><code>6da4c2f</code></a> chore: cherry-pick 6da1a8953313 from angle (<a href="https://redirect.github.com/electron/electron/issues/37708">#37708</a>)</li>
<li><a href="https://github.com/electron/electron/commit/75ddfcc0e242840ebc7907813e268b94f18f26a9"><code>75ddfcc</code></a> docs: change MSDN links to new Microsoft docs (<a href="https://redirect.github.com/electron/electron/issues/37706">#37706</a>)</li>
<li><a href="https://github.com/electron/electron/commit/4e692e2211ff6c877f9c4284bb138bb1650c4b59"><code>4e692e2</code></a> ci: update appveyor image to e-110.0.5481.208 (<a href="https://redirect.github.com/electron/electron/issues/37685">#37685</a>)</li>
<li><a href="https://github.com/electron/electron/commit/e508ef2b8c2297a7ea4cf4f5928dfe350f7fc193"><code>e508ef2</code></a> chore: bump chromium to 110.0.5481.208 (23-x-y) (<a href="https://redirect.github.com/electron/electron/issues/37645">#37645</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/electron/electron/compare/v13.6.6...v23.2.1">compare view</a></li>
</ul>
</details>
<br />


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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-toolbox/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-03 20:21:28 +0000 UTC
    </div>
</div>

