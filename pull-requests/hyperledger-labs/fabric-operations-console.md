---
layout: default
title: fabric-operations-console
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-operations-console
---

# fabric-operations-console <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-operations-console){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/180" class=".btn">#180</a>
            </td>
            <td>
                <b>
                    Create channel wizard osnadmin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- New feature

#### Description
Extends create channel wizard to support channels via channel participation APIs using osnadmin features in Fabric.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-15 19:29:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/179" class=".btn">#179</a>
            </td>
            <td>
                <b>
                    Changes as per 2.5.3 images
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ketul Shah shah.ketul@ibm.com

#### Type of change
<!--- What type of change? Pick one option and delete the others. -->
- Test update

#### Description
<!--- Describe your changes in detail, including motivation. -->
1. Added one explicit wait in 8-InstallInstantiate1xSmartContract.feature
2. Updated "2.2" to "2.4.3" to be selected from Fabric dropdown as per 2.5.3 images


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-14 14:40:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/178" class=".btn">#178</a>
            </td>
            <td>
                <b>
                    Bump moment from 2.29.1 to 2.29.2 in /packages/apollo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [moment](https://github.com/moment/moment) from 2.29.1 to 2.29.2.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/moment/moment/blob/develop/CHANGELOG.md">moment's changelog</a>.</em></p>
<blockquote>
<h3>2.29.2 <a href="https://gist.github.com/ichernev/1904b564f6679d9aac1ae08ce13bc45c">See full changelog</a></h3>
<ul>
<li>Release Apr 3 2022</li>
</ul>
<p>Address <a href="https://github.com/advisories/GHSA-8hfj-j24r-96c4">https://github.com/advisories/GHSA-8hfj-j24r-96c4</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/moment/moment/commit/75e2ac573e8cd62086a6bc6dc1b8d271e2804391"><code>75e2ac5</code></a> Build 2.29.2</li>
<li><a href="https://github.com/moment/moment/commit/5a2987758edc7d413d1248737d9d0d1b65a70450"><code>5a29877</code></a> Bump version to 2.29.2</li>
<li><a href="https://github.com/moment/moment/commit/4fd847b7a8c7065d88ba0a64b727660190dd45d7"><code>4fd847b</code></a> Update changelog for 2.29.2</li>
<li><a href="https://github.com/moment/moment/commit/4211bfc8f15746be4019bba557e29a7ba83d54c5"><code>4211bfc</code></a> [bugfix] Avoid loading path-looking locales from fs</li>
<li><a href="https://github.com/moment/moment/commit/f2a813afcfd0dd6e63812ea74c46ecc627f6a6a6"><code>f2a813a</code></a> [misc] Fix indentation (according to prettier)</li>
<li><a href="https://github.com/moment/moment/commit/7a10de889de64c2519f894a84a98030bec5022d9"><code>7a10de8</code></a> [test] Avoid hours around DST</li>
<li><a href="https://github.com/moment/moment/commit/e96809208c9d1b1bbe22d605e76985770024de42"><code>e968092</code></a> [locale] ar-ly: fix locale name (<a href="https://github-redirect.dependabot.com/moment/moment/issues/5828">#5828</a>)</li>
<li><a href="https://github.com/moment/moment/commit/53d7ee6ad8c60c891571c7085db91831bbc095b4"><code>53d7ee6</code></a> [misc] fix builds (<a href="https://github-redirect.dependabot.com/moment/moment/issues/5836">#5836</a>)</li>
<li><a href="https://github.com/moment/moment/commit/52019f1dda47c3e598aaeaa4ac89d5a574641604"><code>52019f1</code></a> [misc] Specify length of toArray return type (<a href="https://github-redirect.dependabot.com/moment/moment/issues/5766">#5766</a>)</li>
<li><a href="https://github.com/moment/moment/commit/0dcaaa689d02dde824029b09ab6aa64ff351ee2e"><code>0dcaaa6</code></a> [locale] tr: update translation of Monday and Saturday (<a href="https://github-redirect.dependabot.com/moment/moment/issues/5756">#5756</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/moment/moment/compare/2.29.1...2.29.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=moment&package-manager=npm_and_yarn&previous-version=2.29.1&new-version=2.29.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-operations-console/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-09 12:49:19 +0000 UTC
    </div>
</div>

