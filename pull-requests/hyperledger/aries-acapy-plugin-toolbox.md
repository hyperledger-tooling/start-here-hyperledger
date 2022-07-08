---
layout: default
title: aries-acapy-plugin-toolbox
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-acapy-plugin-toolbox
---

# aries-acapy-plugin-toolbox <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-acapy-plugin-toolbox){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/133" class=".btn">#133</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump lxml from 4.8.0 to 4.9.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [lxml](https://github.com/lxml/lxml) from 4.8.0 to 4.9.1.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/lxml/lxml/blob/master/CHANGES.txt">lxml's changelog</a>.</em></p>
<blockquote>
<h1>4.9.1 (2022-07-01)</h1>
<h2>Bugs fixed</h2>
<ul>
<li>A crash was resolved when using <code>iterwalk()</code> (or <code>canonicalize()</code>)
after parsing certain incorrect input.  Note that <code>iterwalk()</code> can crash
on <em>valid</em> input parsed with the same parser <em>after</em> failing to parse the
incorrect input.</li>
</ul>
<h1>4.9.0 (2022-06-01)</h1>
<h2>Bugs fixed</h2>
<ul>
<li>GH#341: The mixin inheritance order in <code>lxml.html</code> was corrected.
Patch by xmo-odoo.</li>
</ul>
<h2>Other changes</h2>
<ul>
<li>
<p>Built with Cython 0.29.30 to adapt to changes in Python 3.11 and 3.12.</p>
</li>
<li>
<p>Wheels include zlib 1.2.12, libxml2 2.9.14 and libxslt 1.1.35
(libxml2 2.9.12+ and libxslt 1.1.34 on Windows).</p>
</li>
<li>
<p>GH#343: Windows-AArch64 build support in Visual Studio.
Patch by Steve Dower.</p>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/lxml/lxml/commit/d01872ccdf7e1e5e825b6c6292b43e7d27ae5fc4"><code>d01872c</code></a> Prevent parse failure in new test from leaking into later test runs.</li>
<li><a href="https://github.com/lxml/lxml/commit/d65e63229e8958bc08344a85cd3f09ceeef933c3"><code>d65e632</code></a> Prepare release of lxml 4.9.1.</li>
<li><a href="https://github.com/lxml/lxml/commit/86368e9cf70a0ad23cccd5ee32de847149af0c6f"><code>86368e9</code></a> Fix a crash when incorrect parser input occurs together with usages of iterwa...</li>
<li><a href="https://github.com/lxml/lxml/commit/50c276412880c1a3dde8a6d6c909e3ed8ef47e43"><code>50c2764</code></a> Delete unused Travis CI config and reference in docs (<a href="https://github-redirect.dependabot.com/lxml/lxml/issues/345">GH-345</a>)</li>
<li><a href="https://github.com/lxml/lxml/commit/8f0bf2d158f2dd3f98d410c8a38fcd536fd11b53"><code>8f0bf2d</code></a> Try to speed up the musllinux AArch64 build by splitting the different CPytho...</li>
<li><a href="https://github.com/lxml/lxml/commit/b9f7074430594b95824059eef931dfbb27a7645e"><code>b9f7074</code></a> Remove debug print from test.</li>
<li><a href="https://github.com/lxml/lxml/commit/b224e0f69dde58425d1077e07d193d19d3f803a9"><code>b224e0f</code></a> Try to install 'xz' in wheel builds, if available, since it's now needed to e...</li>
<li><a href="https://github.com/lxml/lxml/commit/897ebfa002fe5ec773ffe8851721047fedcc6928"><code>897ebfa</code></a> Update macOS deployment target version from 10.14 to 10.15 since 10.14 starts...</li>
<li><a href="https://github.com/lxml/lxml/commit/853c9e9cbf1c82d1ad3c096362372a048108905e"><code>853c9e9</code></a> Prepare release of 4.9.0.</li>
<li><a href="https://github.com/lxml/lxml/commit/d3f77e678a8394559331d27257714e8aa4b082f2"><code>d3f77e6</code></a> Add a test for <a href="https://bugs.launchpad.net/lxml/+bug/1965070">https://bugs.launchpad.net/lxml/+bug/1965070</a> leaving out the a...</li>
<li>Additional commits viewable in <a href="https://github.com/lxml/lxml/compare/lxml-4.8.0...lxml-4.9.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=lxml&package-manager=pip&previous-version=4.8.0&new-version=4.9.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugin-toolbox/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 21:33:23 +0000 UTC
    </div>
</div>

