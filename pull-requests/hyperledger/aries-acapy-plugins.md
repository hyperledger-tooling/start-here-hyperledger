---
layout: default
title: aries-acapy-plugins
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-acapy-plugins
---

# aries-acapy-plugins <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-acapy-plugins){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/419" class=".btn">#419</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump pytest-ruff from 0.1.1 to 0.3.2 in /connection_update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-ruff](https://github.com/businho/pytest-ruff) from 0.1.1 to 0.3.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/businho/pytest-ruff/releases">pytest-ruff's releases</a>.</em></p>
<blockquote>
<h2>Cleaner test error output</h2>
<p>Full stack trace is not relevant for us, it was removed in <a href="https://redirect.github.com/businho/pytest-ruff/issues/18">#18</a>. Thanks to <a href="https://github.com/lexi-k"><code>@​lexi-k</code></a>.</p>
<h2>Add support to pytest 8.1.x</h2>
<p>No release notes provided.</p>
<h2>Support old pytest versions</h2>
<p>No release notes provided.</p>
<h2>Fix previous messed up release</h2>
<p>It makes <code>--ruff</code> and <code>--ruff-format</code> work independently and make the plugin work again.</p>
<h2>Support ruff format and respect exclude config</h2>
<p>No release notes provided.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/businho/pytest-ruff/commit/cb1685eacf28dc25bda0dcd6f4bc43705e1cf13a"><code>cb1685e</code></a> Stop printing whole pytest traceback on error (<a href="https://redirect.github.com/businho/pytest-ruff/issues/18">#18</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/9efc242a519f8c7648bc732a170079864b592521"><code>9efc242</code></a> fix: pytest 8.1 compat (<a href="https://redirect.github.com/businho/pytest-ruff/issues/16">#16</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/41ec4c4cc327aa3c5f86f466025dc53bee29304d"><code>41ec4c4</code></a> Silence some deprecation warnings for Python 3.14</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/ef9d0e0bc173dac03f1af954f9a9d3574203a64e"><code>ef9d0e0</code></a> Fail tests with warnings</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/37b8e736063f61ca4b5118ac499ee63fb3943b17"><code>37b8e73</code></a> Support old pytests (<a href="https://redirect.github.com/businho/pytest-ruff/issues/13">#13</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/463bb48aed573d28b63b00e81f317ffcf0c2cbf9"><code>463bb48</code></a> Fix cov (<a href="https://redirect.github.com/businho/pytest-ruff/issues/14">#14</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/8a6a5a32602cd4936029ddae1bda4ce899b8d98f"><code>8a6a5a3</code></a> Run tox with 3.12 and drop 3.7</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/1ef9b2244f6dc63be9fefeef909092e4cf50c9a1"><code>1ef9b22</code></a> Merge pull request <a href="https://redirect.github.com/businho/pytest-ruff/issues/10">#10</a> from cclauss/patch-1</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/951ece4fff3c07d9be59ab1dcb64bf7e7ad49130"><code>951ece4</code></a> Upgrade GitHub Actions and add Python 3.12</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/2098829cfb8f95c2885c6dec3e229ed3092e2c1e"><code>2098829</code></a> Merge pull request <a href="https://redirect.github.com/businho/pytest-ruff/issues/8">#8</a> from skellys/fix/fix_v0_2</li>
<li>Additional commits viewable in <a href="https://github.com/businho/pytest-ruff/compare/v0.1.1...v0.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-ruff&package-manager=pip&previous-version=0.1.1&new-version=0.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-03 04:20:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/418" class=".btn">#418</a>
            </td>
            <td>
                <b>
                    Release workflows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Opening this as a new PR again. I had to do work on my forked main branch and when I rebased it forced closed the old PR's.  
https://github.com/hyperledger/aries-acapy-plugins/pull/391
https://github.com/hyperledger/aries-acapy-plugins/pull/387

I think I addressed all the comments. 

Some of the bash scripting is pretty gross but I tried to comment and document it well.

I had to fix some tests and I upgraded the anoncreds library as well. This is where the changes unrelated to the workflows came from. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-02 21:20:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/417" class=".btn">#417</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump ejs from 3.1.9 to 3.1.10 in /oid4vci/demo/frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [ejs](https://github.com/mde/ejs) from 3.1.9 to 3.1.10.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/mde/ejs/releases">ejs's releases</a>.</em></p>
<blockquote>
<h2>v3.1.10</h2>
<p>Version 3.1.10</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/mde/ejs/commit/d3f807dea9ce904e20a47a661f2310ce9134dc2a"><code>d3f807d</code></a> Version 3.1.10</li>
<li><a href="https://github.com/mde/ejs/commit/9ee26dde5d7015d9c0e2ff87314cabeac5247c02"><code>9ee26dd</code></a> Mocha TDD</li>
<li><a href="https://github.com/mde/ejs/commit/e469741dca7df2eb400199e1cdb74621e3f89aa5"><code>e469741</code></a> Basic pollution protection</li>
<li><a href="https://github.com/mde/ejs/commit/715e9507fa3e6122dc6430fe0f25a6e6ded300c1"><code>715e950</code></a> Merge pull request <a href="https://redirect.github.com/mde/ejs/issues/756">#756</a> from Jeffrey-mu/main</li>
<li><a href="https://github.com/mde/ejs/commit/cabe3146ad964a1e98db7742abf435906ca79406"><code>cabe314</code></a> Include advanced usage examples</li>
<li><a href="https://github.com/mde/ejs/commit/29b076cdbbf3eb1b4323b33299ab6d79391b2c33"><code>29b076c</code></a> Added header</li>
<li><a href="https://github.com/mde/ejs/commit/11503c79af882e3635b513d57c7f1813792eb127"><code>11503c7</code></a> Merge branch 'main' of github.com:mde/ejs into main</li>
<li><a href="https://github.com/mde/ejs/commit/7690404e2fc1688756938e4d2fc19e0fac77d736"><code>7690404</code></a> Added security banner to README</li>
<li><a href="https://github.com/mde/ejs/commit/f47d7aedd51a983e4f73045f962b1209096b5800"><code>f47d7ae</code></a> Update SECURITY.md</li>
<li><a href="https://github.com/mde/ejs/commit/828cea1687e3db459ab09d2f405d2444c7580b90"><code>828cea1</code></a> Update SECURITY.md</li>
<li>Additional commits viewable in <a href="https://github.com/mde/ejs/compare/v3.1.9...v3.1.10">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ejs&package-manager=npm_and_yarn&previous-version=3.1.9&new-version=3.1.10)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-02 15:37:58 +0000 UTC
    </div>
</div>

