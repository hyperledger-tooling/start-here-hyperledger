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
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/10" class=".btn">#10</a>
            </td>
            <td>
                <b>
                    fix: allow merge commits
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
        Created At 2023-10-19 13:48:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/9" class=".btn">#9</a>
            </td>
            <td>
                <b>
                    Add MAINTAINERS.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I basically just copied this from aca-py. I'm not sure if there is extra info that can be removed. I removed the `toc` and go-ext` scopes. The rest seemed like they could stay.

I added Jason Sherman and Daniel Bluhm as Admin's and that is it.

Maybe Stephan Curran and Ry Jones would like to be added?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-17 21:23:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/8" class=".btn">#8</a>
            </td>
            <td>
                <b>
                    Bump urllib3 from 2.0.6 to 2.0.7 in /basicmessage_storage
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-17 21:07:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/7" class=".btn">#7</a>
            </td>
            <td>
                <b>
                    Bump urllib3 from 2.0.6 to 2.0.7 in /basicmessage_storage/integration
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-17 21:06:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/5" class=".btn">#5</a>
            </td>
            <td>
                <b>
                    Advance repo - Add plugin, testing, update script
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds another plugin `connection_update`, testing for current plugins, documentation updates and a script for common dependency and file management.

Only one additional plugin was added so far. Others are being worked on but the testing has been a bit of a learning process and I want plugins to be added that are adequately tested. Some of the plugins I want to add have a lot more logic that will be more difficult testing. 

Reading the root README might be a good way to understand the entire context.

----

When I was adding my first plugin to the repo I realized that we want to have isolated environments for development and testing and that quickly things were going to be difficult to manage. 

To combat this I decided to create a base empty plugin `default-empty-plugin` and a script `updater.sh` which updates the existing plugins and populates common files from it. I'm only sure the script works on linux systems currently. Some of the text commands possibly won't work on mac OS.

I tried to update the README as well as I could to make it clear how to add an existing plugin or create a new one from scratch. It is quite easy but instructions can be hard.

I'm not super happy with the naming I chose. I might change it if I can think of something better.

One of the next important steps might be getting all the tests for each plugin running in the CI/CD pipeline. 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-17 16:40:16 +0000 UTC
    </div>
</div>

