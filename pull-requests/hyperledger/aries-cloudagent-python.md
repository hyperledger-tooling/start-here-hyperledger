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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2559" class=".btn">#2559</a>
            </td>
            <td>
                <b>
                    refactor: replace multiformats library
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This replaces the multiformats library with a very basic implementation included directly within ACA-Py. Given that the multiformats library has gone stale and my PR has languished, I think this is a good alternative to using that library. The implementation is very simple and currently only supports the minimum currently required by ACA-Py. Expanding the implementation in the future should be trivial.

Fixes #2501 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-19 15:19:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2558" class=".btn">#2558</a>
            </td>
            <td>
                <b>
                    Fix: RevRegEntry Transaction Endorsement
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #2441 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-19 14:32:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2554" class=".btn">#2554</a>
            </td>
            <td>
                <b>
                    fix: taa rough timestamp timezone from datetime
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2553
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-18 18:10:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2552" class=".btn">#2552</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump urllib3 from 2.0.6 to 2.0.7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [urllib3](https://github.com/urllib3/urllib3) from 2.0.6 to 2.0.7.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/releases">urllib3's releases</a>.</em></p>
<blockquote>
<h2>2.0.7</h2>
<ul>
<li>Made body stripped from HTTP requests changing the request method to GET after HTTP 303 &quot;See Other&quot; redirect responses. (GHSA-g4mx-q9vg-27p4)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/blob/main/CHANGES.rst">urllib3's changelog</a>.</em></p>
<blockquote>
<h1>2.0.7 (2023-10-17)</h1>
<ul>
<li>Made body stripped from HTTP requests changing the request method to GET after HTTP 303 &quot;See Other&quot; redirect responses.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/urllib3/urllib3/commit/56f01e088dc006c03d4ee6ea9da4ab810f1ed700"><code>56f01e0</code></a> Release 2.0.7</li>
<li><a href="https://github.com/urllib3/urllib3/commit/4e50fbc5db74e32cabd5ccc1ab81fc103adfe0b3"><code>4e50fbc</code></a> Merge pull request from GHSA-g4mx-q9vg-27p4</li>
<li><a href="https://github.com/urllib3/urllib3/commit/80808b04bfa68fbd099828848c96ee25df185f1d"><code>80808b0</code></a> Fix docs build on Python 3.12 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3144">#3144</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/f28deff1cf162c673b50d88d3552e91bda6d68a8"><code>f28deff</code></a> Add 1.26.17 to the current changelog</li>
<li>See full diff in <a href="https://github.com/urllib3/urllib3/compare/2.0.6...2.0.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=urllib3&package-manager=pip&previous-version=2.0.6&new-version=2.0.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-cloudagent-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-17 21:06:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2551" class=".btn">#2551</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump urllib3 from 2.0.6 to 2.0.7 in /demo/playground/scripts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [urllib3](https://github.com/urllib3/urllib3) from 2.0.6 to 2.0.7.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/releases">urllib3's releases</a>.</em></p>
<blockquote>
<h2>2.0.7</h2>
<ul>
<li>Made body stripped from HTTP requests changing the request method to GET after HTTP 303 &quot;See Other&quot; redirect responses. (GHSA-g4mx-q9vg-27p4)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/blob/main/CHANGES.rst">urllib3's changelog</a>.</em></p>
<blockquote>
<h1>2.0.7 (2023-10-17)</h1>
<ul>
<li>Made body stripped from HTTP requests changing the request method to GET after HTTP 303 &quot;See Other&quot; redirect responses.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/urllib3/urllib3/commit/56f01e088dc006c03d4ee6ea9da4ab810f1ed700"><code>56f01e0</code></a> Release 2.0.7</li>
<li><a href="https://github.com/urllib3/urllib3/commit/4e50fbc5db74e32cabd5ccc1ab81fc103adfe0b3"><code>4e50fbc</code></a> Merge pull request from GHSA-g4mx-q9vg-27p4</li>
<li><a href="https://github.com/urllib3/urllib3/commit/80808b04bfa68fbd099828848c96ee25df185f1d"><code>80808b0</code></a> Fix docs build on Python 3.12 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3144">#3144</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/f28deff1cf162c673b50d88d3552e91bda6d68a8"><code>f28deff</code></a> Add 1.26.17 to the current changelog</li>
<li>See full diff in <a href="https://github.com/urllib3/urllib3/compare/2.0.6...2.0.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=urllib3&package-manager=pip&previous-version=2.0.6&new-version=2.0.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-cloudagent-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-17 21:03:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2550" class=".btn">#2550</a>
            </td>
            <td>
                <b>
                    Feat: Per Tenant Logging
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #2359 
- Derived from work done in #2425 
- Needed to close that PR as the pre-release images in there somehow included legacy code which was removed subsequently.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-17 13:58:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2548" class=".btn">#2548</a>
            </td>
            <td>
                <b>
                    Update .readthedocs.yaml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Another fix to this YAML file. Unfortunately, I can't test it without getting it into main (AFAIK...).  Frustrating...

Errors were dumb in the last try...
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-15 20:16:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2547" class=".btn">#2547</a>
            </td>
            <td>
                <b>
                    Update .readthedocs.yaml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                RTD is broken because (I think) missing section of RTD.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-14 22:56:56 +0000 UTC
    </div>
</div>

