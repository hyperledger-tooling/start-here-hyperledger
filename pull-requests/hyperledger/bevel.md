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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1917" class=".btn">#1917</a>
            </td>
            <td>
                <b>
                    Bump minimist from 0.2.1 to 1.2.6 in /platforms/r3-corda/images/networkmap/website
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [minimist](https://github.com/substack/minimist) from 0.2.1 to 1.2.6.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/substack/minimist/commit/7efb22a518b53b06f5b02a1038a88bd6290c2846"><code>7efb22a</code></a> 1.2.6</li>
<li><a href="https://github.com/substack/minimist/commit/ef88b9325f77b5ee643ccfc97e2ebda577e4c4e2"><code>ef88b93</code></a> security notice for additional prototype pollution issue</li>
<li><a href="https://github.com/substack/minimist/commit/c2b981977fa834b223b408cfb860f933c9811e4d"><code>c2b9819</code></a> isConstructorOrProto adapted from PR</li>
<li><a href="https://github.com/substack/minimist/commit/bc8ecee43875261f4f17eb20b1243d3ed15e70eb"><code>bc8ecee</code></a> test from prototype pollution PR</li>
<li><a href="https://github.com/substack/minimist/commit/aeb3e27dae0412de5c0494e9563a5f10c82cc7a9"><code>aeb3e27</code></a> 1.2.5</li>
<li><a href="https://github.com/substack/minimist/commit/278677b171d956b46613a158c6c486c3ef979b20"><code>278677b</code></a> 1.2.4</li>
<li><a href="https://github.com/substack/minimist/commit/4cf1354839cb972e38496d35e12f806eea92c11f"><code>4cf1354</code></a> security notice</li>
<li><a href="https://github.com/substack/minimist/commit/1043d212c3caaf871966e710f52cfdf02f9eea4b"><code>1043d21</code></a> additional test for constructor prototype pollution</li>
<li><a href="https://github.com/substack/minimist/commit/6457d7440a47f329c12c4a5abfbce211c4235b93"><code>6457d74</code></a> 1.2.3</li>
<li><a href="https://github.com/substack/minimist/commit/38a4d1caead72ef99e824bb420a2528eec03d9ab"><code>38a4d1c</code></a> even more aggressive checks for protocol pollution</li>
<li>Additional commits viewable in <a href="https://github.com/substack/minimist/compare/0.2.1...1.2.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=minimist&package-manager=npm_and_yarn&previous-version=0.2.1&new-version=1.2.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-04-12 08:40:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1916" class=".btn">#1916</a>
            </td>
            <td>
                <b>
                    Bump minimist from 1.2.5 to 1.2.6 in /platforms/r3-corda/images/doorman/website
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [minimist](https://github.com/substack/minimist) from 1.2.5 to 1.2.6.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/substack/minimist/commit/7efb22a518b53b06f5b02a1038a88bd6290c2846"><code>7efb22a</code></a> 1.2.6</li>
<li><a href="https://github.com/substack/minimist/commit/ef88b9325f77b5ee643ccfc97e2ebda577e4c4e2"><code>ef88b93</code></a> security notice for additional prototype pollution issue</li>
<li><a href="https://github.com/substack/minimist/commit/c2b981977fa834b223b408cfb860f933c9811e4d"><code>c2b9819</code></a> isConstructorOrProto adapted from PR</li>
<li><a href="https://github.com/substack/minimist/commit/bc8ecee43875261f4f17eb20b1243d3ed15e70eb"><code>bc8ecee</code></a> test from prototype pollution PR</li>
<li>See full diff in <a href="https://github.com/substack/minimist/compare/1.2.5...1.2.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=minimist&package-manager=npm_and_yarn&previous-version=1.2.5&new-version=1.2.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-04-12 08:40:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1915" class=".btn">#1915</a>
            </td>
            <td>
                <b>
                    Bump minimist from 1.2.5 to 1.2.6 in /examples/supplychain-app/besu/express_nodeJS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [minimist](https://github.com/substack/minimist) from 1.2.5 to 1.2.6.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/substack/minimist/commit/7efb22a518b53b06f5b02a1038a88bd6290c2846"><code>7efb22a</code></a> 1.2.6</li>
<li><a href="https://github.com/substack/minimist/commit/ef88b9325f77b5ee643ccfc97e2ebda577e4c4e2"><code>ef88b93</code></a> security notice for additional prototype pollution issue</li>
<li><a href="https://github.com/substack/minimist/commit/c2b981977fa834b223b408cfb860f933c9811e4d"><code>c2b9819</code></a> isConstructorOrProto adapted from PR</li>
<li><a href="https://github.com/substack/minimist/commit/bc8ecee43875261f4f17eb20b1243d3ed15e70eb"><code>bc8ecee</code></a> test from prototype pollution PR</li>
<li>See full diff in <a href="https://github.com/substack/minimist/compare/1.2.5...1.2.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=minimist&package-manager=npm_and_yarn&previous-version=1.2.5&new-version=1.2.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-04-12 08:40:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1914" class=".btn">#1914</a>
            </td>
            <td>
                <b>
                    Bump minimist from 1.2.5 to 1.2.6 in /examples/supplychain-app/quorum/express_nodeJS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [minimist](https://github.com/substack/minimist) from 1.2.5 to 1.2.6.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/substack/minimist/commit/7efb22a518b53b06f5b02a1038a88bd6290c2846"><code>7efb22a</code></a> 1.2.6</li>
<li><a href="https://github.com/substack/minimist/commit/ef88b9325f77b5ee643ccfc97e2ebda577e4c4e2"><code>ef88b93</code></a> security notice for additional prototype pollution issue</li>
<li><a href="https://github.com/substack/minimist/commit/c2b981977fa834b223b408cfb860f933c9811e4d"><code>c2b9819</code></a> isConstructorOrProto adapted from PR</li>
<li><a href="https://github.com/substack/minimist/commit/bc8ecee43875261f4f17eb20b1243d3ed15e70eb"><code>bc8ecee</code></a> test from prototype pollution PR</li>
<li>See full diff in <a href="https://github.com/substack/minimist/compare/1.2.5...1.2.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=minimist&package-manager=npm_and_yarn&previous-version=1.2.5&new-version=1.2.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-04-12 08:40:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1913" class=".btn">#1913</a>
            </td>
            <td>
                <b>
                    Bump minimist from 1.2.5 to 1.2.6 in /examples/supplychain-app/quorum/smartContracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [minimist](https://github.com/substack/minimist) from 1.2.5 to 1.2.6.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/substack/minimist/commit/7efb22a518b53b06f5b02a1038a88bd6290c2846"><code>7efb22a</code></a> 1.2.6</li>
<li><a href="https://github.com/substack/minimist/commit/ef88b9325f77b5ee643ccfc97e2ebda577e4c4e2"><code>ef88b93</code></a> security notice for additional prototype pollution issue</li>
<li><a href="https://github.com/substack/minimist/commit/c2b981977fa834b223b408cfb860f933c9811e4d"><code>c2b9819</code></a> isConstructorOrProto adapted from PR</li>
<li><a href="https://github.com/substack/minimist/commit/bc8ecee43875261f4f17eb20b1243d3ed15e70eb"><code>bc8ecee</code></a> test from prototype pollution PR</li>
<li>See full diff in <a href="https://github.com/substack/minimist/compare/1.2.5...1.2.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=minimist&package-manager=npm_and_yarn&previous-version=1.2.5&new-version=1.2.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-04-12 08:40:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1912" class=".btn">#1912</a>
            </td>
            <td>
                <b>
                    Bump logback-core from 1.2.3 to 1.2.9 in /platforms/r3-corda/images/doorman
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">java</span>
            </td>
            <td>
                Bumps logback-core from 1.2.3 to 1.2.9.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ch.qos.logback:logback-core&package-manager=maven&previous-version=1.2.3&new-version=1.2.9)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-04-12 08:39:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1911" class=".btn">#1911</a>
            </td>
            <td>
                <b>
                    Bump minimist from 1.2.5 to 1.2.6 in /examples/supplychain-app/fabric/express_nodeJs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [minimist](https://github.com/substack/minimist) from 1.2.5 to 1.2.6.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/substack/minimist/commit/7efb22a518b53b06f5b02a1038a88bd6290c2846"><code>7efb22a</code></a> 1.2.6</li>
<li><a href="https://github.com/substack/minimist/commit/ef88b9325f77b5ee643ccfc97e2ebda577e4c4e2"><code>ef88b93</code></a> security notice for additional prototype pollution issue</li>
<li><a href="https://github.com/substack/minimist/commit/c2b981977fa834b223b408cfb860f933c9811e4d"><code>c2b9819</code></a> isConstructorOrProto adapted from PR</li>
<li><a href="https://github.com/substack/minimist/commit/bc8ecee43875261f4f17eb20b1243d3ed15e70eb"><code>bc8ecee</code></a> test from prototype pollution PR</li>
<li>See full diff in <a href="https://github.com/substack/minimist/compare/1.2.5...1.2.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=minimist&package-manager=npm_and_yarn&previous-version=1.2.5&new-version=1.2.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-04-12 08:39:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1910" class=".btn">#1910</a>
            </td>
            <td>
                <b>
                    Bump minimist from 1.2.5 to 1.2.6 in /examples/supplychain-app/corda/express_nodeJS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [minimist](https://github.com/substack/minimist) from 1.2.5 to 1.2.6.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/substack/minimist/commit/7efb22a518b53b06f5b02a1038a88bd6290c2846"><code>7efb22a</code></a> 1.2.6</li>
<li><a href="https://github.com/substack/minimist/commit/ef88b9325f77b5ee643ccfc97e2ebda577e4c4e2"><code>ef88b93</code></a> security notice for additional prototype pollution issue</li>
<li><a href="https://github.com/substack/minimist/commit/c2b981977fa834b223b408cfb860f933c9811e4d"><code>c2b9819</code></a> isConstructorOrProto adapted from PR</li>
<li><a href="https://github.com/substack/minimist/commit/bc8ecee43875261f4f17eb20b1243d3ed15e70eb"><code>bc8ecee</code></a> test from prototype pollution PR</li>
<li>See full diff in <a href="https://github.com/substack/minimist/compare/1.2.5...1.2.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=minimist&package-manager=npm_and_yarn&previous-version=1.2.5&new-version=1.2.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-04-12 08:39:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1909" class=".btn">#1909</a>
            </td>
            <td>
                <b>
                    Bump logback-core from 1.2.3 to 1.2.9 in /platforms/r3-corda/images/networkmap
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">java</span>
            </td>
            <td>
                Bumps logback-core from 1.2.3 to 1.2.9.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ch.qos.logback:logback-core&package-manager=maven&previous-version=1.2.3&new-version=1.2.9)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-04-12 08:39:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1906" class=".btn">#1906</a>
            </td>
            <td>
                <b>
                    Bump minimist from 1.2.5 to 1.2.6 in /examples/supplychain-app/fabric/chaincode_rest_server/rest-server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [minimist](https://github.com/substack/minimist) from 1.2.5 to 1.2.6.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/substack/minimist/commit/7efb22a518b53b06f5b02a1038a88bd6290c2846"><code>7efb22a</code></a> 1.2.6</li>
<li><a href="https://github.com/substack/minimist/commit/ef88b9325f77b5ee643ccfc97e2ebda577e4c4e2"><code>ef88b93</code></a> security notice for additional prototype pollution issue</li>
<li><a href="https://github.com/substack/minimist/commit/c2b981977fa834b223b408cfb860f933c9811e4d"><code>c2b9819</code></a> isConstructorOrProto adapted from PR</li>
<li><a href="https://github.com/substack/minimist/commit/bc8ecee43875261f4f17eb20b1243d3ed15e70eb"><code>bc8ecee</code></a> test from prototype pollution PR</li>
<li>See full diff in <a href="https://github.com/substack/minimist/compare/1.2.5...1.2.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=minimist&package-manager=npm_and_yarn&previous-version=1.2.5&new-version=1.2.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-04-11 18:53:08 +0000 UTC
    </div>
</div>

