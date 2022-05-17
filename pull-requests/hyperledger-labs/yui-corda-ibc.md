---
layout: default
title: yui-corda-ibc
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/yui-corda-ibc
---

# yui-corda-ibc <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/yui-corda-ibc){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-corda-ibc/pull/31" class=".btn">#31</a>
            </td>
            <td>
                <b>
                    build(deps): bump babel from 2.9.0 to 2.9.1 in /docsrc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [babel](https://github.com/python-babel/babel) from 2.9.0 to 2.9.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/python-babel/babel/releases">babel's releases</a>.</em></p>
<blockquote>
<h2>Version 2.9.1</h2>
<h1>Bugfixes</h1>
<ul>
<li>The internal locale-data loading functions now validate the name of the locale file to be loaded and only allow files within Babel's data directory.  Thank you to Chris Lyne of Tenable, Inc. for discovering the issue!</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/python-babel/babel/blob/master/CHANGES.rst">babel's changelog</a>.</em></p>
<blockquote>
<h2>Version 2.9.1</h2>
<p>Bugfixes</p>
<pre><code>
* The internal locale-data loading functions now validate the name of the locale file to be loaded and only
  allow files within Babel's data directory.  Thank you to Chris Lyne of Tenable, Inc. for discovering the issue!
</code></pre>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/python-babel/babel/commit/a99fa2474c808b51ebdabea18db871e389751559"><code>a99fa24</code></a> Use 2.9.0's setup.py for 2.9.1</li>
<li><a href="https://github.com/python-babel/babel/commit/60b33e083801109277cb068105251e76d0b7c14e"><code>60b33e0</code></a> Become 2.9.1</li>
<li><a href="https://github.com/python-babel/babel/commit/412015ef642bfcc0d8ba8f4d05cdbb6aac98d9b3"><code>412015e</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/python-babel/babel/issues/782">#782</a> from python-babel/locale-basename</li>
<li><a href="https://github.com/python-babel/babel/commit/5caf717ceca4bd235552362b4fbff88983c75d8c"><code>5caf717</code></a> Disallow special filenames on Windows</li>
<li><a href="https://github.com/python-babel/babel/commit/3a700b5b8b53606fd98ef8294a56f9510f7290f8"><code>3a700b5</code></a> Run locale identifiers through <code>os.path.basename()</code></li>
<li><a href="https://github.com/python-babel/babel/commit/5afe2b2f11dcdd6090c00231d342c2e9cd1bdaab"><code>5afe2b2</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/python-babel/babel/issues/754">#754</a> from python-babel/github-ci</li>
<li><a href="https://github.com/python-babel/babel/commit/58de8342f865df88697a4a166191e880e3c84d82"><code>58de834</code></a> Replace Travis + Appveyor with GitHub Actions (WIP)</li>
<li><a href="https://github.com/python-babel/babel/commit/d1bbc08e845d03d8e1f0dfa0e04983d755f39cb5"><code>d1bbc08</code></a> import_cldr: use logging; add -q option</li>
<li><a href="https://github.com/python-babel/babel/commit/156b7fb9f377ccf58c71cf01dc69fb10c7b69314"><code>156b7fb</code></a> Quiesce CLDR download progress bar if requested (or not a TTY)</li>
<li><a href="https://github.com/python-babel/babel/commit/613dc1700f91c3d40b081948c0dd6023d8ece057"><code>613dc17</code></a> Make the import warnings about unsupported number systems less verbose</li>
<li>Additional commits viewable in <a href="https://github.com/python-babel/babel/compare/v2.9.0...v2.9.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=babel&package-manager=pip&previous-version=2.9.0&new-version=2.9.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-corda-ibc/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-17 03:28:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-corda-ibc/pull/30" class=".btn">#30</a>
            </td>
            <td>
                <b>
                    build(deps): bump urllib3 from 1.26.4 to 1.26.5 in /docsrc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [urllib3](https://github.com/urllib3/urllib3) from 1.26.4 to 1.26.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/releases">urllib3's releases</a>.</em></p>
<blockquote>
<h2>1.26.5</h2>
<p>:warning: <strong>IMPORTANT: urllib3 v2.0 will drop support for Python 2</strong>: <a href="https://urllib3.readthedocs.io/en/latest/v2-roadmap.html">Read more in the v2.0 Roadmap</a></p>
<ul>
<li>Fixed deprecation warnings emitted in Python 3.10.</li>
<li>Updated vendored <code>six</code> library to 1.16.0.</li>
<li>Improved performance of URL parser when splitting the authority component.</li>
</ul>
<p><strong>If you or your organization rely on urllib3 consider supporting us via <a href="https://github.com/sponsors/urllib3">GitHub Sponsors</a></strong></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/blob/main/CHANGES.rst">urllib3's changelog</a>.</em></p>
<blockquote>
<h1>1.26.5 (2021-05-26)</h1>
<ul>
<li>Fixed deprecation warnings emitted in Python 3.10.</li>
<li>Updated vendored <code>six</code> library to 1.16.0.</li>
<li>Improved performance of URL parser when splitting
the authority component.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/urllib3/urllib3/commit/d1616473df94b94f0f5ad19d2a6608cfe93b7cdf"><code>d161647</code></a> Release 1.26.5</li>
<li><a href="https://github.com/urllib3/urllib3/commit/2d4a3fee6de2fa45eb82169361918f759269b4ec"><code>2d4a3fe</code></a> Improve performance of sub-authority splitting in URL</li>
<li><a href="https://github.com/urllib3/urllib3/commit/2698537d52f8ff1f0bbb1d45cf018b118e91f637"><code>2698537</code></a> Update vendored six to 1.16.0</li>
<li><a href="https://github.com/urllib3/urllib3/commit/07bed791e9c391d8bf12950f76537dc3c6f90550"><code>07bed79</code></a> Fix deprecation warnings for Python 3.10 ssl module</li>
<li><a href="https://github.com/urllib3/urllib3/commit/d725a9b56bb8baf87c9e6eee0e9edf010034b63b"><code>d725a9b</code></a> Add Python 3.10 to GitHub Actions</li>
<li><a href="https://github.com/urllib3/urllib3/commit/339ad34c677c98fd9ad008de1d8bbeb9dbf34381"><code>339ad34</code></a> Use pytest==6.2.4 on Python 3.10+</li>
<li><a href="https://github.com/urllib3/urllib3/commit/f271c9c3149e20d7feffb6429b135bbb6c09ddf4"><code>f271c9c</code></a> Apply latest Black formatting</li>
<li><a href="https://github.com/urllib3/urllib3/commit/1884878aac87ef0494b282e940c32c24ee917d52"><code>1884878</code></a> [1.26] Properly proxy EOF on the SSLTransport test suite</li>
<li>See full diff in <a href="https://github.com/urllib3/urllib3/compare/1.26.4...1.26.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=urllib3&package-manager=pip&previous-version=1.26.4&new-version=1.26.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-corda-ibc/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-17 03:28:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-corda-ibc/pull/29" class=".btn">#29</a>
            </td>
            <td>
                <b>
                    Repair flows test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-13 03:52:57 +0000 UTC
    </div>
</div>

