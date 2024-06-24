---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3062" class=".btn">#3062</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump markupsafe from 2.0.1 to 2.1.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [markupsafe](https://github.com/pallets/markupsafe) from 2.0.1 to 2.1.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pallets/markupsafe/releases">markupsafe's releases</a>.</em></p>
<blockquote>
<h2>2.1.5</h2>
<p>This is a fix release for the 2.1.x feature release branch. It fixes bugs but does not otherwise change behavior and should not result in breaking changes.</p>
<p>Fixes a regression in <code>striptags</code> behavior from 2.14. Spaces are now collapsed correctly.</p>
<ul>
<li>Changes: <a href="https://markupsafe.palletsprojects.com/en/2.1.x/changes/#version-2-1-5">https://markupsafe.palletsprojects.com/en/2.1.x/changes/#version-2-1-5</a></li>
<li>Milestone: <a href="https://github.com/pallets/markupsafe/milestone/12?closed=1">https://github.com/pallets/markupsafe/milestone/12?closed=1</a></li>
<li>PyPI: <a href="https://pypi.org/project/MarkupSafe/2.1.5/">https://pypi.org/project/MarkupSafe/2.1.5/</a></li>
</ul>
<h2>2.1.4</h2>
<p>This is a fix release for the 2.1.x feature release branch. It fixes bugs but does not otherwise change behavior and should not result in breaking changes.</p>
<ul>
<li>
<p>Improves performance of the <code>Markup.striptags</code> method for large input.</p>
</li>
<li>
<p>Changes: <a href="https://markupsafe.palletsprojects.com/en/2.1.x/changes/#version-2-1-4">https://markupsafe.palletsprojects.com/en/2.1.x/changes/#version-2-1-4</a></p>
</li>
<li>
<p>Milestone: <a href="https://github.com/pallets/markupsafe/milestone/11?closed=1">https://github.com/pallets/markupsafe/milestone/11?closed=1</a></p>
</li>
<li>
<p>PyPI: <a href="https://pypi.org/project/MarkupSafe/2.1.4/">https://pypi.org/project/MarkupSafe/2.1.4/</a></p>
</li>
</ul>
<h2>2.1.3</h2>
<p>This is a fix release for the 2.1.x feature branch.</p>
<ul>
<li>Changes: <a href="https://markupsafe.palletsprojects.com/en/2.1.x/changes/#version-2-1-3">https://markupsafe.palletsprojects.com/en/2.1.x/changes/#version-2-1-3</a></li>
<li>Milestone: <a href="https://github.com/pallets/markupsafe/milestone/9?closed=1">https://github.com/pallets/markupsafe/milestone/9?closed=1</a></li>
</ul>
<h2>2.1.2</h2>
<p>This is the first release to provide wheels for Python 3.11. An SLSA provenance file is also generated, and is available to download from the GitHub release page.</p>
<ul>
<li>Changes: <a href="https://markupsafe.palletsprojects.com/en/2.1.x/changes/#version-2-1-2">https://markupsafe.palletsprojects.com/en/2.1.x/changes/#version-2-1-2</a></li>
<li>Milestone: <a href="https://github.com/pallets/markupsafe/milestone/8?closed=1">https://github.com/pallets/markupsafe/milestone/8?closed=1</a></li>
</ul>
<h2>2.1.1</h2>
<ul>
<li>Changes: <a href="https://markupsafe.palletsprojects.com/en/2.1.x/changes/#version-2-1-1">https://markupsafe.palletsprojects.com/en/2.1.x/changes/#version-2-1-1</a></li>
<li>Milestone: <a href="https://github.com/pallets/markupsafe/milestone/7?closed=1">https://github.com/pallets/markupsafe/milestone/7?closed=1</a></li>
</ul>
<h2>2.1.0</h2>
<ul>
<li>Changes: <a href="https://markupsafe.palletsprojects.com/en/2.1.x/changes/#version-2-1-0">https://markupsafe.palletsprojects.com/en/2.1.x/changes/#version-2-1-0</a></li>
<li>Milestone: <a href="https://github.com/pallets/markupsafe/milestone/5">https://github.com/pallets/markupsafe/milestone/5</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pallets/markupsafe/blob/main/CHANGES.rst">markupsafe's changelog</a>.</em></p>
<blockquote>
<h2>Version 2.1.5</h2>
<p>Released 2024-02-02</p>
<ul>
<li>Fix <code>striptags</code> not collapsing spaces. :issue:<code>417</code></li>
</ul>
<h2>Version 2.1.4</h2>
<p>Released 2024-01-19</p>
<ul>
<li>Don't use regular expressions for <code>striptags</code>, avoiding a performance
issue. :pr:<code>413</code></li>
</ul>
<h2>Version 2.1.3</h2>
<p>Released 2023-06-02</p>
<ul>
<li>Implement <code>format_map</code>, <code>casefold</code>, <code>removeprefix</code>, and <code>removesuffix</code>
methods. :issue:<code>370</code></li>
<li>Fix static typing for basic <code>str</code> methods on <code>Markup</code>. :issue:<code>358</code></li>
<li>Use <code>Self</code> for annotating return types. :pr:<code>379</code></li>
</ul>
<h2>Version 2.1.2</h2>
<p>Released 2023-01-17</p>
<ul>
<li>Fix <code>striptags</code> not stripping tags containing newlines.
:issue:<code>310</code></li>
</ul>
<h2>Version 2.1.1</h2>
<p>Released 2022-03-14</p>
<ul>
<li>Avoid ambiguous regex matches in <code>striptags</code>. :pr:<code>293</code></li>
</ul>
<h2>Version 2.1.0</h2>
<p>Released 2022-02-17</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pallets/markupsafe/commit/fbba4acd0312826cec9cfe18371c7df07962cb65"><code>fbba4ac</code></a> release version 2.1.5</li>
<li><a href="https://github.com/pallets/markupsafe/commit/c5fa23ba96336160204ed1376d60693b0d65e18d"><code>c5fa23b</code></a> update publish actions</li>
<li><a href="https://github.com/pallets/markupsafe/commit/60a6512315d0ce05e6788808f80be526f2084b3f"><code>60a6512</code></a> striptags collapses spaces correctly (<a href="https://redirect.github.com/pallets/markupsafe/issues/418">#418</a>)</li>
<li><a href="https://github.com/pallets/markupsafe/commit/0b6bee071fbd8d3171fb1ac4fb669baace808438"><code>0b6bee0</code></a> collapse spaces after stripping tags</li>
<li><a href="https://github.com/pallets/markupsafe/commit/73e6a4886564a554c4a19983d29c97f9fc95457d"><code>73e6a48</code></a> start version 2.1.5</li>
<li><a href="https://github.com/pallets/markupsafe/commit/d704bf45a1f77926a669261b394afef38eda2a70"><code>d704bf4</code></a> use pip-compile, dependabot updates (<a href="https://redirect.github.com/pallets/markupsafe/issues/419">#419</a>)</li>
<li><a href="https://github.com/pallets/markupsafe/commit/1f82932e5c5a6e54181308afeb8443df21858ea0"><code>1f82932</code></a> use pip-compile, dependabot updates</li>
<li><a href="https://github.com/pallets/markupsafe/commit/25a640f38297bfdc2ec2c82fe68df4c7613d083a"><code>25a640f</code></a> release version 2.1.4 (<a href="https://redirect.github.com/pallets/markupsafe/issues/414">#414</a>)</li>
<li><a href="https://github.com/pallets/markupsafe/commit/b7cd6523579ea5a08d89799f2a64ec2c2bc45eca"><code>b7cd652</code></a> release version 2.1.4</li>
<li><a href="https://github.com/pallets/markupsafe/commit/3bead8eedcfb434097dc61a18dd4721201df262a"><code>3bead8e</code></a> update cibuildwheel for 3.12 wheels</li>
<li>Additional commits viewable in <a href="https://github.com/pallets/markupsafe/compare/2.0.1...2.1.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=markupsafe&package-manager=pip&previous-version=2.0.1&new-version=2.1.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-24 11:27:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3061" class=".btn">#3061</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump pydevd from 1.5.1 to 1.9.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pydevd](https://github.com/fabioz/PyDev.Debugger) from 1.5.1 to 1.9.2.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/fabioz/PyDev.Debugger/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pydevd&package-manager=pip&previous-version=1.5.1&new-version=1.9.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-24 11:27:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3060" class=".btn">#3060</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump pydevd-pycharm from 193.6015.41 to 193.7288.30
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pydevd-pycharm](https://github.com/JetBrains/intellij-community) from 193.6015.41 to 193.7288.30.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/JetBrains/intellij-community/commits/pycharm/193.7288.30">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pydevd-pycharm&package-manager=pip&previous-version=193.6015.41&new-version=193.7288.30)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-24 11:26:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3059" class=".btn">#3059</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump portalocker from 2.8.2 to 2.10.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [portalocker](https://github.com/wolph/portalocker) from 2.8.2 to 2.10.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/wolph/portalocker/releases">portalocker's releases</a>.</em></p>
<blockquote>
<h2>v2.10.0</h2>
<p>Properly propagating exceptions for NFS read-only lock issues and added support for being able to choose between lockf and flock thanks to <a href="https://github.com/oliver-s-lee"><code>@​oliver-s-lee</code></a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/wolph/portalocker/commit/06d58c4206186c56b009e6a5f3de5aa578d2d353"><code>06d58c4</code></a> Merge branch 'release/2.10.0'</li>
<li><a href="https://github.com/wolph/portalocker/commit/c78d0558814b1c09f0e65692f9b46892b3296164"><code>c78d055</code></a> Incrementing version to v2.10.0</li>
<li><a href="https://github.com/wolph/portalocker/commit/eedc656dfa703f395e016b5b44c62239dc79f0c0"><code>eedc656</code></a> Incrementing version to v2.9.0</li>
<li><a href="https://github.com/wolph/portalocker/commit/57ae4415408cbadde1020ec221325f6b67cbc22c"><code>57ae441</code></a> typing protocols cannot be covered by tests</li>
<li><a href="https://github.com/wolph/portalocker/commit/f3d91afa1923bf77d9b28d1a25bf95da3ea545d2"><code>f3d91af</code></a> type hinting improvements</li>
<li><a href="https://github.com/wolph/portalocker/commit/5cc3aad961bab8353282dfa5659346966ffbe09d"><code>5cc3aad</code></a> made mypy happy</li>
<li><a href="https://github.com/wolph/portalocker/commit/80d40bf5bfcc86bc85b096d7a1531935a7a206e7"><code>80d40bf</code></a> ruff fixes</li>
<li><a href="https://github.com/wolph/portalocker/commit/d7315a5bc4afbdb50da26cb68fec07c229f14fbd"><code>d7315a5</code></a> pyright fixes</li>
<li><a href="https://github.com/wolph/portalocker/commit/561f3c803449148884ee685ca7474091b7f998f4"><code>561f3c8</code></a> increased timeouts for slower platforms</li>
<li><a href="https://github.com/wolph/portalocker/commit/b775cf0e9c811c4de1c494fcd0ab54f3bb9c829f"><code>b775cf0</code></a> fixed tests for linux</li>
<li>Additional commits viewable in <a href="https://github.com/wolph/portalocker/compare/v2.8.2...v2.10.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=portalocker&package-manager=pip&previous-version=2.8.2&new-version=2.10.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-24 11:26:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3058" class=".btn">#3058</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump ruff from 0.4.4 to 0.4.10
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.4.4 to 0.4.10.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.10</h2>
<h2>Changes</h2>
<h3>Parser</h3>
<ul>
<li>Implement re-lexing logic for better error recovery (<a href="https://redirect.github.com/astral-sh/ruff/pull/11845">#11845</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-copyright</code>] Update <code>CPY001</code> to check the first 4096 bytes instead of 1024 (<a href="https://redirect.github.com/astral-sh/ruff/pull/11927">#11927</a>)</li>
<li>[<code>pycodestyle</code>] Update <code>E999</code> to show all syntax errors instead of just the first one (<a href="https://redirect.github.com/astral-sh/ruff/pull/11900">#11900</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Add tracing setup guide to Helix documentation (<a href="https://redirect.github.com/astral-sh/ruff/pull/11883">#11883</a>)</li>
<li>Add tracing setup guide to Neovim documentation (<a href="https://redirect.github.com/astral-sh/ruff/pull/11884">#11884</a>)</li>
<li>Defer notebook cell deletion to avoid an error message (<a href="https://redirect.github.com/astral-sh/ruff/pull/11864">#11864</a>)</li>
</ul>
<h3>Security</h3>
<ul>
<li>Guard against malicious ecosystem comment artifacts (<a href="https://redirect.github.com/astral-sh/ruff/pull/11879">#11879</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/adrinjalali"><code>@​adrinjalali</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/github-actions"><code>@​github-actions</code></a></li>
<li><a href="https://github.com/psychedelicious"><code>@​psychedelicious</code></a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a></li>
<li><a href="https://github.com/snowsignal"><code>@​snowsignal</code></a></li>
<li><a href="https://github.com/zanieb"><code>@​zanieb</code></a></li>
</ul>
<h2>v0.4.9</h2>
<h2>Changes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pylint</code>] Implement <code>consider-dict-items</code> (<code>C0206</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11688">#11688</a>)</li>
<li>[<code>refurb</code>] Implement <code>repeated-global</code> (<code>FURB154</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11187">#11187</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pycodestyle</code>] Adapt fix for <code>E203</code> to work identical to <code>ruff format</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10999">#10999</a>)</li>
</ul>
<h3>Formatter</h3>
<ul>
<li>Fix formatter instability for lines only consisting of zero-width characters (<a href="https://redirect.github.com/astral-sh/ruff/pull/11748">#11748</a>)</li>
</ul>
<h3>Server</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.4.10</h2>
<h3>Parser</h3>
<ul>
<li>Implement re-lexing logic for better error recovery (<a href="https://redirect.github.com/astral-sh/ruff/pull/11845">#11845</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-copyright</code>] Update <code>CPY001</code> to check the first 4096 bytes instead of 1024 (<a href="https://redirect.github.com/astral-sh/ruff/pull/11927">#11927</a>)</li>
<li>[<code>pycodestyle</code>] Update <code>E999</code> to show all syntax errors instead of just the first one (<a href="https://redirect.github.com/astral-sh/ruff/pull/11900">#11900</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Add tracing setup guide to Helix documentation (<a href="https://redirect.github.com/astral-sh/ruff/pull/11883">#11883</a>)</li>
<li>Add tracing setup guide to Neovim documentation (<a href="https://redirect.github.com/astral-sh/ruff/pull/11884">#11884</a>)</li>
<li>Defer notebook cell deletion to avoid an error message (<a href="https://redirect.github.com/astral-sh/ruff/pull/11864">#11864</a>)</li>
</ul>
<h3>Security</h3>
<ul>
<li>Guard against malicious ecosystem comment artifacts (<a href="https://redirect.github.com/astral-sh/ruff/pull/11879">#11879</a>)</li>
</ul>
<h2>0.4.9</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pylint</code>] Implement <code>consider-dict-items</code> (<code>C0206</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11688">#11688</a>)</li>
<li>[<code>refurb</code>] Implement <code>repeated-global</code> (<code>FURB154</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11187">#11187</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pycodestyle</code>] Adapt fix for <code>E203</code> to work identical to <code>ruff format</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10999">#10999</a>)</li>
</ul>
<h3>Formatter</h3>
<ul>
<li>Fix formatter instability for lines only consisting of zero-width characters (<a href="https://redirect.github.com/astral-sh/ruff/pull/11748">#11748</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Add supported commands in server capabilities (<a href="https://redirect.github.com/astral-sh/ruff/pull/11850">#11850</a>)</li>
<li>Use real file path when available in <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11800">#11800</a>)</li>
<li>Improve error message when a command is run on an unavailable document (<a href="https://redirect.github.com/astral-sh/ruff/pull/11823">#11823</a>)</li>
<li>Introduce the <code>ruff.printDebugInformation</code> command (<a href="https://redirect.github.com/astral-sh/ruff/pull/11831">#11831</a>)</li>
<li>Tracing system now respects log level and trace level, with options to log to a file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11747">#11747</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Handle non-printable characters in diff view (<a href="https://redirect.github.com/astral-sh/ruff/pull/11687">#11687</a>)</li>
</ul>
<h3>Bug fixes</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/b54922fd7394c36cdc390fd21aaee99206ebc361"><code>b54922f</code></a> Bump version to v0.4.10 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11953">#11953</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/3f884b4b34b234c91c8af3bc44ef8d18cde7b363"><code>3f884b4</code></a> Avoid running logical line rule logic if not enabled (<a href="https://redirect.github.com/astral-sh/ruff/issues/11951">#11951</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/b456051be8277e11a3bb3aa5625c3f9ebd9b6108"><code>b456051</code></a> [red-knot] Add tracing to Salsa queries (<a href="https://redirect.github.com/astral-sh/ruff/issues/11949">#11949</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/2dfbf118d7aff26c50360767cd0803ad6c4b7abf"><code>2dfbf11</code></a> [red-knot] Extract <code>red_knot_python_semantic</code> crate (<a href="https://redirect.github.com/astral-sh/ruff/issues/11926">#11926</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/ed948eaefbde81695f8a2eb0c0b0c2c21420d092"><code>ed948ea</code></a> Avoid moving back the lexer for triple-quoted fstring (<a href="https://redirect.github.com/astral-sh/ruff/issues/11939">#11939</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/22733cb7c7eda64f535458c4e0cd47c71874d2b2"><code>22733cb</code></a> red-knot(Salsa): Types without refinements (<a href="https://redirect.github.com/astral-sh/ruff/issues/11899">#11899</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/a26bd01be2b673f13cb6c88f4150dd12e5873f55"><code>a26bd01</code></a> Avoid depth counting when detecting indentation (<a href="https://redirect.github.com/astral-sh/ruff/issues/11947">#11947</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/b617d906510ab6ea04e019f73b5aa56fe3692e0a"><code>b617d90</code></a> Update <code>E999</code> to show all syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/issues/11900">#11900</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/cdc7c7144997ca9aa99a6bfae9dd73b4fa53de49"><code>cdc7c71</code></a> Avoid consuming trailing whitespace during re-lexing (<a href="https://redirect.github.com/astral-sh/ruff/issues/11933">#11933</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/ff3bf583b28c455a19571a54cd4a4e2bc024b5b8"><code>ff3bf58</code></a> <code>ruff server</code>: Add tracing setup guide to Neovim documentation (<a href="https://redirect.github.com/astral-sh/ruff/issues/11884">#11884</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.4.4...v0.4.10">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.4.4&new-version=0.4.10)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-24 11:25:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3057" class=".btn">#3057</a>
            </td>
            <td>
                <b>
                    fix: didexchange manager not checking the did-rotate content correctly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                minor error i noticed while browsing acapy code whilst working on aries-vcx: https://github.com/hyperledger/aries-vcx/issues/1226.

if statement was not correcting the correct data, resulting in it always being `true`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-24 01:40:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3056" class=".btn">#3056</a>
            </td>
            <td>
                <b>
                    Add vcdm 2.0 issuance/verification
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Initial attempt at adding VCDM  2.0 issuance with `ED25519Signature2020` proof type.

Will add a couple test cases.

What are opinions regarding if the credential models/schemas should be bundled into the same or have 2 distinct models?

I went with the latter.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-24 01:35:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3051" class=".btn">#3051</a>
            </td>
            <td>
                <b>
                    LTS Release Strategy and corresponding changes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Creating this PR to add the LTS (Long Term Support) Release Strategy for Aca-py releases. This closes https://github.com/hyperledger/aries-cloudagent-python/issues/2993

The following are the summary of changes.

1. Releases section added to Readme
2. LTS Release Strategy document added to docs
3. Snyk container image scanning mode changed to 'monitor' for LTS images
4. Supported Features checklist updated with LTS versions
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-21 13:18:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3050" class=".btn">#3050</a>
            </td>
            <td>
                <b>
                    fix: respond to did:peer:1 with did:peer:4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adjusts the default did method ACA-Py will respond to did:peer:1 with to did:peer:4. This should help the situation reported in #3020.

Marked as draft until I have a chance to test against Credo.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-19 23:34:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3049" class=".btn">#3049</a>
            </td>
            <td>
                <b>
                    Handle failed tails server issuance [Anoncreds]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Handles the scenario where the tails server isn't available during revocation rotation.
- Fixes a bug with the openapi verse expected value for `max_cred_num`
- Refactors the create_credential function
- Removes some TODO's. Most with documentation that I think is good enough.

Keeps the revocation list in a failed state if the revocation registry has never been uploaded to the tails server. During issuance it will check for a failed state and try to upload and finish the revocation list. Issuance will not occur until a successful tails server and connection occurs.

Thought about keeping the revocation registry definition itself in a failed state but seemed to make sense to have it this way so the registry will still handle the full registry scenario.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-19 21:26:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3048" class=".btn">#3048</a>
            </td>
            <td>
                <b>
                    :adhesive_bandage: add exception handling to wallet-upgrade check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Simple fix for non-critical issue.

Currently, if something goes wrong with the `check_for_wallet_upgrades_in_progress` method, then startup will be aborted. This PR just adds a try-except block, such that the exception is logged and startup can proceed.

Relates to #3030
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-19 13:37:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3046" class=".btn">#3046</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump the pip group with 2 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group with 2 updates: [requests](https://github.com/psf/requests) and [urllib3](https://github.com/urllib3/urllib3).

Updates `requests` from 2.31.0 to 2.32.2
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/releases">requests's releases</a>.</em></p>
<blockquote>
<h2>v2.32.2</h2>
<h2>2.32.2 (2024-05-21)</h2>
<p><strong>Deprecations</strong></p>
<ul>
<li>
<p>To provide a more stable migration for custom HTTPAdapters impacted
by the CVE changes in 2.32.0, we've renamed <code>_get_connection</code> to
a new public API, <code>get_connection_with_tls_context</code>. Existing custom
HTTPAdapters will need to migrate their code to use this new API.
<code>get_connection</code> is considered deprecated in all versions of Requests&gt;=2.32.0.</p>
<p>A minimal (2-line) example has been provided in the linked PR to ease
migration, but we strongly urge users to evaluate if their custom adapter
is subject to the same issue described in CVE-2024-35195. (<a href="https://redirect.github.com/psf/requests/issues/6710">#6710</a>)</p>
</li>
</ul>
<h2>v2.32.1</h2>
<h2>2.32.1 (2024-05-20)</h2>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Add missing test certs to the sdist distributed on PyPI.</li>
</ul>
<h2>v2.32.0</h2>
<h2>2.32.0 (2024-05-20)</h2>
<h2>🐍 PYCON US 2024 EDITION 🐍</h2>
<p><strong>Security</strong></p>
<ul>
<li>Fixed an issue where setting <code>verify=False</code> on the first request from a
Session will cause subsequent requests to the <em>same origin</em> to also ignore
cert verification, regardless of the value of <code>verify</code>.
(<a href="https://github.com/psf/requests/security/advisories/GHSA-9wx4-h78v-vm56">https://github.com/psf/requests/security/advisories/GHSA-9wx4-h78v-vm56</a>)</li>
</ul>
<p><strong>Improvements</strong></p>
<ul>
<li><code>verify=True</code> now reuses a global SSLContext which should improve
request time variance between first and subsequent requests. It should
also minimize certificate load time on Windows systems when using a Python
version built with OpenSSL 3.x. (<a href="https://redirect.github.com/psf/requests/issues/6667">#6667</a>)</li>
<li>Requests now supports optional use of character detection
(<code>chardet</code> or <code>charset_normalizer</code>) when repackaged or vendored.
This enables <code>pip</code> and other projects to minimize their vendoring
surface area. The <code>Response.text()</code> and <code>apparent_encoding</code> APIs
will default to <code>utf-8</code> if neither library is present. (<a href="https://redirect.github.com/psf/requests/issues/6702">#6702</a>)</li>
</ul>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Fixed bug in length detection where emoji length was incorrectly
calculated in the request content-length. (<a href="https://redirect.github.com/psf/requests/issues/6589">#6589</a>)</li>
<li>Fixed deserialization bug in JSONDecodeError. (<a href="https://redirect.github.com/psf/requests/issues/6629">#6629</a>)</li>
<li>Fixed bug where an extra leading <code>/</code> (path separator) could lead
urllib3 to unnecessarily reparse the request URI. (<a href="https://redirect.github.com/psf/requests/issues/6644">#6644</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/blob/main/HISTORY.md">requests's changelog</a>.</em></p>
<blockquote>
<h2>2.32.2 (2024-05-21)</h2>
<p><strong>Deprecations</strong></p>
<ul>
<li>
<p>To provide a more stable migration for custom HTTPAdapters impacted
by the CVE changes in 2.32.0, we've renamed <code>_get_connection</code> to
a new public API, <code>get_connection_with_tls_context</code>. Existing custom
HTTPAdapters will need to migrate their code to use this new API.
<code>get_connection</code> is considered deprecated in all versions of Requests&gt;=2.32.0.</p>
<p>A minimal (2-line) example has been provided in the linked PR to ease
migration, but we strongly urge users to evaluate if their custom adapter
is subject to the same issue described in CVE-2024-35195. (<a href="https://redirect.github.com/psf/requests/issues/6710">#6710</a>)</p>
</li>
</ul>
<h2>2.32.1 (2024-05-20)</h2>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Add missing test certs to the sdist distributed on PyPI.</li>
</ul>
<h2>2.32.0 (2024-05-20)</h2>
<p><strong>Security</strong></p>
<ul>
<li>Fixed an issue where setting <code>verify=False</code> on the first request from a
Session will cause subsequent requests to the <em>same origin</em> to also ignore
cert verification, regardless of the value of <code>verify</code>.
(<a href="https://github.com/psf/requests/security/advisories/GHSA-9wx4-h78v-vm56">https://github.com/psf/requests/security/advisories/GHSA-9wx4-h78v-vm56</a>)</li>
</ul>
<p><strong>Improvements</strong></p>
<ul>
<li><code>verify=True</code> now reuses a global SSLContext which should improve
request time variance between first and subsequent requests. It should
also minimize certificate load time on Windows systems when using a Python
version built with OpenSSL 3.x. (<a href="https://redirect.github.com/psf/requests/issues/6667">#6667</a>)</li>
<li>Requests now supports optional use of character detection
(<code>chardet</code> or <code>charset_normalizer</code>) when repackaged or vendored.
This enables <code>pip</code> and other projects to minimize their vendoring
surface area. The <code>Response.text()</code> and <code>apparent_encoding</code> APIs
will default to <code>utf-8</code> if neither library is present. (<a href="https://redirect.github.com/psf/requests/issues/6702">#6702</a>)</li>
</ul>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Fixed bug in length detection where emoji length was incorrectly
calculated in the request content-length. (<a href="https://redirect.github.com/psf/requests/issues/6589">#6589</a>)</li>
<li>Fixed deserialization bug in JSONDecodeError. (<a href="https://redirect.github.com/psf/requests/issues/6629">#6629</a>)</li>
<li>Fixed bug where an extra leading <code>/</code> (path separator) could lead
urllib3 to unnecessarily reparse the request URI. (<a href="https://redirect.github.com/psf/requests/issues/6644">#6644</a>)</li>
</ul>
<p><strong>Deprecations</strong></p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/psf/requests/commit/88dce9d854797c05d0ff296b70e0430535ef8aaf"><code>88dce9d</code></a> v2.32.2</li>
<li><a href="https://github.com/psf/requests/commit/c98e4d133ef29c46a9b68cd783087218a8075e05"><code>c98e4d1</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6710">#6710</a> from nateprewitt/api_rename</li>
<li><a href="https://github.com/psf/requests/commit/92075b330a30b9883f466a43d3f7566ab849f91b"><code>92075b3</code></a> Add deprecation warning</li>
<li><a href="https://github.com/psf/requests/commit/aa1461b68aa73e2f6ec0e78c8853b635c76fd099"><code>aa1461b</code></a> Move _get_connection to get_connection_with_tls_context</li>
<li><a href="https://github.com/psf/requests/commit/970e8cec988421bd43da57350723b05c8ce8dc7e"><code>970e8ce</code></a> v2.32.1</li>
<li><a href="https://github.com/psf/requests/commit/d6ebc4a2f1f68b7e355fb7e4dd5ffc0845547f9f"><code>d6ebc4a</code></a> v2.32.0</li>
<li><a href="https://github.com/psf/requests/commit/9a40d1277807f0a4f26c9a37eea8ec90faa8aadc"><code>9a40d12</code></a> Avoid reloading root certificates to improve concurrent performance (<a href="https://redirect.github.com/psf/requests/issues/6667">#6667</a>)</li>
<li><a href="https://github.com/psf/requests/commit/0c030f78d24f29a459dbf39b28b4cc765e2153d7"><code>0c030f7</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6702">#6702</a> from nateprewitt/no_char_detection</li>
<li><a href="https://github.com/psf/requests/commit/555b870eb19d497ddb67042645420083ec8efb02"><code>555b870</code></a> Allow character detection dependencies to be optional in post-packaging steps</li>
<li><a href="https://github.com/psf/requests/commit/d6dded3f00afcf56a7e866cb0732799045301eb0"><code>d6dded3</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6700">#6700</a> from franekmagiera/update-redirect-to-invalid-uri-test</li>
<li>Additional commits viewable in <a href="https://github.com/psf/requests/compare/v2.31.0...v2.32.2">compare view</a></li>
</ul>
</details>
<br />

Updates `urllib3` from 2.2.1 to 2.2.2
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/releases">urllib3's releases</a>.</em></p>
<blockquote>
<h2>2.2.2</h2>
<h2>🚀 urllib3 is fundraising for HTTP/2 support</h2>
<p><a href="https://sethmlarson.dev/urllib3-is-fundraising-for-http2-support">urllib3 is raising ~$40,000 USD</a> to release HTTP/2 support and ensure long-term sustainable maintenance of the project after a sharp decline in financial support for 2023. If your company or organization uses Python and would benefit from HTTP/2 support in Requests, pip, cloud SDKs, and thousands of other projects <a href="https://opencollective.com/urllib3">please consider contributing financially</a> to ensure HTTP/2 support is developed sustainably and maintained for the long-haul.</p>
<p>Thank you for your support.</p>
<h2>Changes</h2>
<ul>
<li>Added the <code>Proxy-Authorization</code> header to the list of headers to strip from requests when redirecting to a different host. As before, different headers can be set via <code>Retry.remove_headers_on_redirect</code>.</li>
<li>Allowed passing negative integers as <code>amt</code> to read methods of <code>http.client.HTTPResponse</code> as an alternative to <code>None</code>. (<a href="https://redirect.github.com/urllib3/urllib3/issues/3122">#3122</a>)</li>
<li>Fixed return types representing copying actions to use <code>typing.Self</code>. (<a href="https://redirect.github.com/urllib3/urllib3/issues/3363">#3363</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/urllib3/urllib3/compare/2.2.1...2.2.2">https://github.com/urllib3/urllib3/compare/2.2.1...2.2.2</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/blob/main/CHANGES.rst">urllib3's changelog</a>.</em></p>
<blockquote>
<h1>2.2.2 (2024-06-17)</h1>
<ul>
<li>Added the <code>Proxy-Authorization</code> header to the list of headers to strip from requests when redirecting to a different host. As before, different headers can be set via <code>Retry.remove_headers_on_redirect</code>.</li>
<li>Allowed passing negative integers as <code>amt</code> to read methods of <code>http.client.HTTPResponse</code> as an alternative to <code>None</code>. (<code>[#3122](https://github.com/urllib3/urllib3/issues/3122) &lt;https://github.com/urllib3/urllib3/issues/3122&gt;</code>__)</li>
<li>Fixed return types representing copying actions to use <code>typing.Self</code>. (<code>[#3363](https://github.com/urllib3/urllib3/issues/3363) &lt;https://github.com/urllib3/urllib3/issues/3363&gt;</code>__)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/urllib3/urllib3/commit/27e2a5c5a7ab6a517252cc8dcef3ffa6ffb8f61a"><code>27e2a5c</code></a> Release 2.2.2 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3406">#3406</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/accff72ecc2f6cf5a76d9570198a93ac7c90270e"><code>accff72</code></a> Merge pull request from GHSA-34jh-p97f-mpxf</li>
<li><a href="https://github.com/urllib3/urllib3/commit/34be4a57e59eb7365bcc37d52e9f8271b5b8d0d3"><code>34be4a5</code></a> Pin CFFI to a new release candidate instead of a Git commit (<a href="https://redirect.github.com/urllib3/urllib3/issues/3398">#3398</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/da410581b6b3df73da976b5ce5eb20a4bd030437"><code>da41058</code></a> Bump browser-actions/setup-chrome from 1.6.0 to 1.7.1 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3399">#3399</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/b07a669bd970d69847801148286b726f0570b625"><code>b07a669</code></a> Bump github/codeql-action from 2.13.4 to 3.25.6 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3396">#3396</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/b8589ec9f8c4da91511e601b632ac06af7e7c10e"><code>b8589ec</code></a> Measure coverage with v4 of artifact actions (<a href="https://redirect.github.com/urllib3/urllib3/issues/3394">#3394</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/f3bdc5585111429e22c81b5fb26c3ec164d98b81"><code>f3bdc55</code></a> Allow triggering CI manually (<a href="https://redirect.github.com/urllib3/urllib3/issues/3391">#3391</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/52392654b30183129cf3ec06010306f517d9c146"><code>5239265</code></a> Fix HTTP version in debug log (<a href="https://redirect.github.com/urllib3/urllib3/issues/3316">#3316</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/b34619f94ece0c40e691a5aaf1304953d88089de"><code>b34619f</code></a> Bump actions/checkout to 4.1.4 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3387">#3387</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/9961d14de7c920091d42d42ed76d5d479b80064d"><code>9961d14</code></a> Bump browser-actions/setup-chrome from 1.5.0 to 1.6.0 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3386">#3386</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/urllib3/urllib3/compare/2.2.1...2.2.2">compare view</a></li>
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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore <dependency name> major version` will close this group update PR and stop Dependabot creating any more for the specific dependency's major version (unless you unignore this specific dependency's major version or upgrade to it yourself)
- `@dependabot ignore <dependency name> minor version` will close this group update PR and stop Dependabot creating any more for the specific dependency's minor version (unless you unignore this specific dependency's minor version or upgrade to it yourself)
- `@dependabot ignore <dependency name>` will close this group update PR and stop Dependabot creating any more for the specific dependency (unless you unignore this specific dependency or upgrade to it yourself)
- `@dependabot unignore <dependency name>` will remove all of the ignore conditions of the specified dependency
- `@dependabot unignore <dependency name> <ignore condition>` will remove the ignore condition of the specified dependency and ignore conditions
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-cloudagent-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 22:18:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3045" class=".btn">#3045</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump urllib3 from 2.2.1 to 2.2.2 in /demo/playground/examples in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /demo/playground/examples with 1 update: [urllib3](https://github.com/urllib3/urllib3).

Updates `urllib3` from 2.2.1 to 2.2.2
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/releases">urllib3's releases</a>.</em></p>
<blockquote>
<h2>2.2.2</h2>
<h2>🚀 urllib3 is fundraising for HTTP/2 support</h2>
<p><a href="https://sethmlarson.dev/urllib3-is-fundraising-for-http2-support">urllib3 is raising ~$40,000 USD</a> to release HTTP/2 support and ensure long-term sustainable maintenance of the project after a sharp decline in financial support for 2023. If your company or organization uses Python and would benefit from HTTP/2 support in Requests, pip, cloud SDKs, and thousands of other projects <a href="https://opencollective.com/urllib3">please consider contributing financially</a> to ensure HTTP/2 support is developed sustainably and maintained for the long-haul.</p>
<p>Thank you for your support.</p>
<h2>Changes</h2>
<ul>
<li>Added the <code>Proxy-Authorization</code> header to the list of headers to strip from requests when redirecting to a different host. As before, different headers can be set via <code>Retry.remove_headers_on_redirect</code>.</li>
<li>Allowed passing negative integers as <code>amt</code> to read methods of <code>http.client.HTTPResponse</code> as an alternative to <code>None</code>. (<a href="https://redirect.github.com/urllib3/urllib3/issues/3122">#3122</a>)</li>
<li>Fixed return types representing copying actions to use <code>typing.Self</code>. (<a href="https://redirect.github.com/urllib3/urllib3/issues/3363">#3363</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/urllib3/urllib3/compare/2.2.1...2.2.2">https://github.com/urllib3/urllib3/compare/2.2.1...2.2.2</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/blob/main/CHANGES.rst">urllib3's changelog</a>.</em></p>
<blockquote>
<h1>2.2.2 (2024-06-17)</h1>
<ul>
<li>Added the <code>Proxy-Authorization</code> header to the list of headers to strip from requests when redirecting to a different host. As before, different headers can be set via <code>Retry.remove_headers_on_redirect</code>.</li>
<li>Allowed passing negative integers as <code>amt</code> to read methods of <code>http.client.HTTPResponse</code> as an alternative to <code>None</code>. (<code>[#3122](https://github.com/urllib3/urllib3/issues/3122) &lt;https://github.com/urllib3/urllib3/issues/3122&gt;</code>__)</li>
<li>Fixed return types representing copying actions to use <code>typing.Self</code>. (<code>[#3363](https://github.com/urllib3/urllib3/issues/3363) &lt;https://github.com/urllib3/urllib3/issues/3363&gt;</code>__)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/urllib3/urllib3/commit/27e2a5c5a7ab6a517252cc8dcef3ffa6ffb8f61a"><code>27e2a5c</code></a> Release 2.2.2 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3406">#3406</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/accff72ecc2f6cf5a76d9570198a93ac7c90270e"><code>accff72</code></a> Merge pull request from GHSA-34jh-p97f-mpxf</li>
<li><a href="https://github.com/urllib3/urllib3/commit/34be4a57e59eb7365bcc37d52e9f8271b5b8d0d3"><code>34be4a5</code></a> Pin CFFI to a new release candidate instead of a Git commit (<a href="https://redirect.github.com/urllib3/urllib3/issues/3398">#3398</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/da410581b6b3df73da976b5ce5eb20a4bd030437"><code>da41058</code></a> Bump browser-actions/setup-chrome from 1.6.0 to 1.7.1 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3399">#3399</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/b07a669bd970d69847801148286b726f0570b625"><code>b07a669</code></a> Bump github/codeql-action from 2.13.4 to 3.25.6 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3396">#3396</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/b8589ec9f8c4da91511e601b632ac06af7e7c10e"><code>b8589ec</code></a> Measure coverage with v4 of artifact actions (<a href="https://redirect.github.com/urllib3/urllib3/issues/3394">#3394</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/f3bdc5585111429e22c81b5fb26c3ec164d98b81"><code>f3bdc55</code></a> Allow triggering CI manually (<a href="https://redirect.github.com/urllib3/urllib3/issues/3391">#3391</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/52392654b30183129cf3ec06010306f517d9c146"><code>5239265</code></a> Fix HTTP version in debug log (<a href="https://redirect.github.com/urllib3/urllib3/issues/3316">#3316</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/b34619f94ece0c40e691a5aaf1304953d88089de"><code>b34619f</code></a> Bump actions/checkout to 4.1.4 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3387">#3387</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/9961d14de7c920091d42d42ed76d5d479b80064d"><code>9961d14</code></a> Bump browser-actions/setup-chrome from 1.5.0 to 1.6.0 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3386">#3386</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/urllib3/urllib3/compare/2.2.1...2.2.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=urllib3&package-manager=pip&previous-version=2.2.1&new-version=2.2.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot ignore <dependency name> major version` will close this group update PR and stop Dependabot creating any more for the specific dependency's major version (unless you unignore this specific dependency's major version or upgrade to it yourself)
- `@dependabot ignore <dependency name> minor version` will close this group update PR and stop Dependabot creating any more for the specific dependency's minor version (unless you unignore this specific dependency's minor version or upgrade to it yourself)
- `@dependabot ignore <dependency name>` will close this group update PR and stop Dependabot creating any more for the specific dependency (unless you unignore this specific dependency or upgrade to it yourself)
- `@dependabot unignore <dependency name>` will remove all of the ignore conditions of the specified dependency
- `@dependabot unignore <dependency name> <ignore condition>` will remove the ignore condition of the specified dependency and ignore conditions
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-cloudagent-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 22:17:22 +0000 UTC
    </div>
</div>

