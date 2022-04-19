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
                PR <a href="https://github.com/hyperledger/bevel/pull/1920" class=".btn">#1920</a>
            </td>
            <td>
                <b>
                    [fabric] Change or add ImagePullPolicy to be IfNotPresent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: mgCepeda <marina.gomez.cepeda@accenture.com>

**Changelog**

- Update ca, operations_console, orderernode, zkkafka, peernode charts. Added or changed field, imagePullPolicy: IfNotPresent

 

**Reviewed by**
@suvajit-sarkar
@jagpreetsinghsasan

 

**Linked issue**
#1882 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-19 09:10:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1919" class=".btn">#1919</a>
            </td>
            <td>
                <b>
                    [chore] merge develop to main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**
- decoupling ansible for create certs for besu
- Update tessera version for quorum
- remove downloading complete quorum repo for geth and bootnode
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-14 08:42:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1918" class=".btn">#1918</a>
            </td>
            <td>
                <b>
                    Bump urijs from 1.19.10 to 1.19.11 in /examples/supplychain-app/fabric/chaincode_rest_server/rest-server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [urijs](https://github.com/medialize/URI.js) from 1.19.10 to 1.19.11.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/medialize/URI.js/releases">urijs's releases</a>.</em></p>
<blockquote>
<h2>1.19.11 (April 3rd 2022)</h2>
<ul>
<li><strong>SECURITY</strong> fixing <a href="http://medialize.github.io/URI.js/docs.html#static-parse"><code>URI.parse()</code></a> handle excessive slashes in scheme-relative URLs - disclosed by <a href="https://github.com/zeyu2001">zeyu2001</a> via <a href="https://huntr.dev/">https://huntr.dev/</a></li>
<li><strong>SECURITY</strong> fixing <a href="http://medialize.github.io/URI.js/docs.html#static-parse"><code>URI.parse()</code></a> remove <code>\r</code> (CR), <code>\n</code>, (LF) <code>\t</code> (TAB) - disclosed by <a href="https://github.com/haxatron">haxatron</a> via <a href="https://huntr.dev/">https://huntr.dev/</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/medialize/URI.js/blob/gh-pages/CHANGELOG.md">urijs's changelog</a>.</em></p>
<blockquote>
<h3>1.19.11 (April 3rd 2022)</h3>
<ul>
<li><strong>SECURITY</strong> fixing <a href="http://medialize.github.io/URI.js/docs.html#static-parse"><code>URI.parse()</code></a> handle excessive slashes in scheme-relative URLs - disclosed by <a href="https://github.com/zeyu2001">zeyu2001</a> via <a href="https://huntr.dev/">https://huntr.dev/</a></li>
<li><strong>SECURITY</strong> fixing <a href="http://medialize.github.io/URI.js/docs.html#static-parse"><code>URI.parse()</code></a> remove <code>\r</code> (CR), <code>\n</code>, (LF) <code>\t</code> (TAB) - disclosed by <a href="https://github.com/haxatron">haxatron</a> via <a href="https://huntr.dev/">https://huntr.dev/</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/medialize/URI.js/commit/b655c1b972111ade9f181b02374305942e68e30a"><code>b655c1b</code></a> chore(build): bumping to version 1.19.11</li>
<li><a href="https://github.com/medialize/URI.js/commit/b0c9796aa1a95a85f40924fb18b1e5da3dc8ffae"><code>b0c9796</code></a> fix(parse): handle CR,LF,TAB</li>
<li><a href="https://github.com/medialize/URI.js/commit/88805fd3da03bd7a5e60947adb49d182011f1277"><code>88805fd</code></a> fix(parse): handle excessive slashes in scheme-relative URLs</li>
<li>See full diff in <a href="https://github.com/medialize/URI.js/compare/v1.19.10...v1.19.11">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=urijs&package-manager=npm_and_yarn&previous-version=1.19.10&new-version=1.19.11)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-04-13 00:17:02 +0000 UTC
    </div>
</div>

