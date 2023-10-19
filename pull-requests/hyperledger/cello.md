---
layout: default
title: cello
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cello
---

# cello <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cello){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/575" class=".btn">#575</a>
            </td>
            <td>
                <b>
                    Bump urllib3 from 1.26.17 to 1.26.18 in /src/api-engine
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [urllib3](https://github.com/urllib3/urllib3) from 1.26.17 to 1.26.18.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/releases">urllib3's releases</a>.</em></p>
<blockquote>
<h2>1.26.18</h2>
<ul>
<li>Made body stripped from HTTP requests changing the request method to GET after HTTP 303 &quot;See Other&quot; redirect responses. (GHSA-g4mx-q9vg-27p4)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/blob/main/CHANGES.rst">urllib3's changelog</a>.</em></p>
<blockquote>
<h1>1.26.18 (2023-10-17)</h1>
<ul>
<li>Made body stripped from HTTP requests changing the request method to GET after HTTP 303 &quot;See Other&quot; redirect responses.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/urllib3/urllib3/commit/9c2c2307dd1d6af504e09aac0326d86ee3597a0b"><code>9c2c230</code></a> Release 1.26.18 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3159">#3159</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/b594c5ceaca38e1ac215f916538fb128e3526a36"><code>b594c5c</code></a> Merge pull request from GHSA-g4mx-q9vg-27p4</li>
<li><a href="https://github.com/urllib3/urllib3/commit/944f0eb134485f41bc531be52de12ba5a37bca73"><code>944f0eb</code></a> [1.26] Use vendored six in urllib3.contrib.securetransport</li>
<li>See full diff in <a href="https://github.com/urllib3/urllib3/compare/1.26.17...1.26.18">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=urllib3&package-manager=pip&previous-version=1.26.17&new-version=1.26.18)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cello/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-18 01:22:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/573" class=".btn">#573</a>
            </td>
            <td>
                <b>
                    Implement Chaincode dashboard
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Implement chaincode dashboard. Add the required buttons to the page.
Use the dummy data for the dev purposes, will be deleted after all
features are finished.

Should be merged after #572 is merged.

Signed-off-by: xichen1 <xichen.pan@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-17 11:19:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/572" class=".btn">#572</a>
            </td>
            <td>
                <b>
                    Add required msgs for Chaincode page
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add required English and Chinese messages for the Chaincode
frontend page.

Signed-off-by: xichen1 <xichen.pan@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-17 09:29:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/571" class=".btn">#571</a>
            </td>
            <td>
                <b>
                    Add option to disable table row selection
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add a prop option in StandardTable component to disable the
row selection in the table.

This is to simplify the table UI and will be used for some tables
of chaincode's sub-page.

To disable the selection, add a `disableSelect` prop to the Stand-
ardTable component.

Signed-off-by: xichen1 <xichen.pan@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-17 08:54:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/570" class=".btn">#570</a>
            </td>
            <td>
                <b>
                    [issue-#569]Modify logo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Modify logo

Close #569 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-14 03:09:37 +0000 UTC
    </div>
</div>

