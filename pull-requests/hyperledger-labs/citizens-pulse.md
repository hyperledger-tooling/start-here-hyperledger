---
layout: default
title: citizens-pulse
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/citizens-pulse
---

# citizens-pulse <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/citizens-pulse){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/citizens-pulse/pull/22" class=".btn">#22</a>
            </td>
            <td>
                <b>
                    Bump moment from 2.27.0 to 2.29.2 in /webui
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [moment](https://github.com/moment/moment) from 2.27.0 to 2.29.2.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/moment/moment/blob/develop/CHANGELOG.md">moment's changelog</a>.</em></p>
<blockquote>
<h3>2.29.2 <a href="https://gist.github.com/ichernev/1904b564f6679d9aac1ae08ce13bc45c">See full changelog</a></h3>
<ul>
<li>Release Apr 3 2022</li>
</ul>
<p>Address <a href="https://github.com/advisories/GHSA-8hfj-j24r-96c4">https://github.com/advisories/GHSA-8hfj-j24r-96c4</a></p>
<h3>2.29.1 <a href="https://gist.github.com/marwahaha/cc478ba01a1292ab4bd4e861d164d99b">See full changelog</a></h3>
<ul>
<li>Release Oct 6, 2020</li>
</ul>
<p>Updated deprecation message, bugfix in hi locale</p>
<h3>2.29.0 <a href="https://gist.github.com/marwahaha/b0111718641a6461800066549957ec14">See full changelog</a></h3>
<ul>
<li>Release Sept 22, 2020</li>
</ul>
<p>New locales (es-mx, bn-bd).
Minor bugfixes and locale improvements.
More tests.
Moment is in maintenance mode. Read more at this link:
<a href="https://momentjs.com/docs/#/-project-status/">https://momentjs.com/docs/#/-project-status/</a></p>
<h3>2.28.0 <a href="https://gist.github.com/marwahaha/028fd6c2b2470b2804857cfd63c0e94f">See full changelog</a></h3>
<ul>
<li>Release Sept 13, 2020</li>
</ul>
<p>Fix bug where .format() modifies original instance, and locale updates</p>
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
<li>Additional commits viewable in <a href="https://github.com/moment/moment/compare/2.27.0...2.29.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=moment&package-manager=npm_and_yarn&previous-version=2.27.0&new-version=2.29.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/citizens-pulse/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-09 14:30:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/citizens-pulse/pull/21" class=".btn">#21</a>
            </td>
            <td>
                <b>
                    Archive lab.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Archived labs are read-only, and they can be moved back out of the archives, if there is interest in reviving them.
    
Signed-off-by: Tracy Kuhrt <tracy.a.kuhrt@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-06 18:16:56 +0000 UTC
    </div>
</div>

