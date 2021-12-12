---
layout: default
title: bevel
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/bevel
---

# bevel <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/bevel){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1778" class=".btn">#1778</a>
            </td>
            <td>
                <b>
                    fixed typo in shared role setup README
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: kaverikhaneja <kaveri.khaneja@accenture.com>

**Changelog**
- Fixed a typographical error in a README file.

 

**Reviewed by**
@sownak @jagpreetsinghsasan @suvajit-sarkar 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 15:59:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1777" class=".btn">#1777</a>
            </td>
            <td>
                <b>
                    [skip ci] Updated code to use new project name
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Roy,Sownak <sownak.roy@accenture.com>

**Changelog**
- Update name references to Hyperledger Bevel

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 13:05:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1776" class=".btn">#1776</a>
            </td>
            <td>
                <b>
                    Bump vertx-web from 3.5.1 to 3.5.4 in /platforms/r3-corda/images/doorman
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">java</span>
            </td>
            <td>
                Bumps vertx-web from 3.5.1 to 3.5.4.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=io.vertx:vertx-web&package-manager=maven&previous-version=3.5.1&new-version=3.5.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 10:12:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1775" class=".btn">#1775</a>
            </td>
            <td>
                <b>
                    Bump vertx-core from 3.5.1 to 3.5.4 in /platforms/r3-corda/images/doorman
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">java</span>
            </td>
            <td>
                Bumps [vertx-core](https://github.com/eclipse/vert.x) from 3.5.1 to 3.5.4.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/eclipse-vertx/vert.x/commit/771b499b0f1fa94e648d895f042643ba2fe74c03"><code>771b499</code></a> Releasing 3.5.4</li>
<li><a href="https://github.com/eclipse-vertx/vert.x/commit/269a583330695d1418a4f5578f7169350b2e1332"><code>269a583</code></a> CVE-2018-12541: When a WebSocket upgrade has a body &gt; 8192 send an appropriat...</li>
<li><a href="https://github.com/eclipse-vertx/vert.x/commit/616a034d59a8fcdb264b4bfcf3ec34bd83175ab0"><code>616a034</code></a> Use public visibiliy for converters as ceylon needs it internally</li>
<li><a href="https://github.com/eclipse-vertx/vert.x/commit/0d67ff6028fe27b48503821feb1c403451efed0c"><code>0d67ff6</code></a> Test to check whether travis builds or not while there is no travis descriptor</li>
<li><a href="https://github.com/eclipse-vertx/vert.x/commit/fcef6562ba9284957401021c416b5c80490d413b"><code>fcef656</code></a> Fixes <a href="https://github-redirect.dependabot.com/eclipse/vert.x/issues/2619">#2619</a>: properly handle plus signs when resolving paths (<a href="https://github-redirect.dependabot.com/eclipse/vert.x/issues/2623">#2623</a>)</li>
<li><a href="https://github.com/eclipse-vertx/vert.x/commit/83e94f672730dd8c5a6cc751c191d77882a88e87"><code>83e94f6</code></a> RecordParser: Limit the record size (<a href="https://github-redirect.dependabot.com/eclipse/vert.x/issues/2635">#2635</a>)</li>
<li><a href="https://github.com/eclipse-vertx/vert.x/commit/20c2669ec281f6174726d0a13c3dbb328269acce"><code>20c2669</code></a> HttpServerResponse content headers improvements - fixes <a href="https://github-redirect.dependabot.com/eclipse/vert.x/issues/2630">#2630</a> - fixes <a href="https://github-redirect.dependabot.com/eclipse/vert.x/issues/2607">#2607</a></li>
<li><a href="https://github.com/eclipse-vertx/vert.x/commit/e1f6fedf8f7fed348293ded845d7618f619bc339"><code>e1f6fed</code></a> VertxHttpHeaders#add(CharSequence,CharSequence) does not used AsciiString cac...</li>
<li><a href="https://github.com/eclipse-vertx/vert.x/commit/a9a7fb0c094efbf3a1464ccb7ed6bd3250c3aa33"><code>a9a7fb0</code></a> Get the list of enabled cipher suite for testing from the JDK</li>
<li><a href="https://github.com/eclipse-vertx/vert.x/commit/254808c8a233841503436278e5f69f54174f2961"><code>254808c</code></a> Improve the ALPN detection to work on latest JDK 11 - fixes <a href="https://github-redirect.dependabot.com/eclipse/vert.x/issues/2625">#2625</a></li>
<li>Additional commits viewable in <a href="https://github.com/eclipse/vert.x/compare/3.5.1...3.5.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=io.vertx:vertx-core&package-manager=maven&previous-version=3.5.1&new-version=3.5.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 10:06:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1774" class=".btn">#1774</a>
            </td>
            <td>
                <b>
                    [skip ci] End of Sprint merge
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Merge for end of sprint
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 09:19:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1773" class=".btn">#1773</a>
            </td>
            <td>
                <b>
                    [skip ci] Updated docs with new project name
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Roy,Sownak <sownak.roy@accenture.com>

**Changelog**
- Update references to Hyperledger Bevel
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 08:04:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1772" class=".btn">#1772</a>
            </td>
            <td>
                <b>
                    [skip ci] Merge latest from main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Merge from main
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-07 11:29:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1771" class=".btn">#1771</a>
            </td>
            <td>
                <b>
                    New project name
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**
- Update Readme and image names to Hyperledger Bevel

**Reviewed by**
@tkuhrt


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-06 15:44:56 +0000 UTC
    </div>
</div>

