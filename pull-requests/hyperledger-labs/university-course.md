---
layout: default
title: university-course
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/university-course
---

# university-course <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/university-course){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/university-course/pull/82" class=".btn">#82</a>
            </td>
            <td>
                <b>
                    chore(deps): bump shell-quote from 1.7.2 to 1.7.3 in /support/Lab06/b4s/organization/university/user-interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [shell-quote](https://github.com/substack/node-shell-quote) from 1.7.2 to 1.7.3.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/substack/node-shell-quote/blob/master/CHANGELOG.md">shell-quote's changelog</a>.</em></p>
<blockquote>
<h2>1.7.3</h2>
<ul>
<li>Fix a security issue where the regex for windows drive letters allowed some shell meta-characters
to escape the quoting rules. (CVE-2021-42740)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/substack/node-shell-quote/commit/6a8a899c62a58a30fb128a7079f02826ed4faee0"><code>6a8a899</code></a> 1.7.3</li>
<li><a href="https://github.com/substack/node-shell-quote/commit/5799416ed454aa4ec9afafc895b4e31760ea1abe"><code>5799416</code></a> fix for security issue with windows drive letter regex</li>
<li><a href="https://github.com/substack/node-shell-quote/commit/c7de931fa4ed0975ea9756983c88334fe4b8cde5"><code>c7de931</code></a> Add security.md</li>
<li><a href="https://github.com/substack/node-shell-quote/commit/414853f1fd98553368ce7507cd26ebae88d71b46"><code>414853f</code></a> Update readme.markdown (<a href="https://github-redirect.dependabot.com/substack/node-shell-quote/issues/43">#43</a>)</li>
<li><a href="https://github.com/substack/node-shell-quote/commit/0fc4a978131ab68cace9c9a57cee245b6b70e595"><code>0fc4a97</code></a> use Github Actions (<a href="https://github-redirect.dependabot.com/substack/node-shell-quote/issues/42">#42</a>)</li>
<li>See full diff in <a href="https://github.com/substack/node-shell-quote/compare/v1.7.2...1.7.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=shell-quote&package-manager=npm_and_yarn&previous-version=1.7.2&new-version=1.7.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/university-course/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-23 05:11:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/university-course/pull/81" class=".btn">#81</a>
            </td>
            <td>
                <b>
                    chore(deps): bump async from 3.2.0 to 3.2.4 in /support/Lab06/chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [async](https://github.com/caolan/async) from 3.2.0 to 3.2.4.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/caolan/async/blob/master/CHANGELOG.md">async's changelog</a>.</em></p>
<blockquote>
<h1>v3.2.4</h1>
<ul>
<li>Fix a bug in <code>priorityQueue</code> where it didn't wait for the result. (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1725">#1725</a>)</li>
<li>Fix a bug where <code>unshiftAsync</code> was included in <code>priorityQueue</code>. (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1790">#1790</a>)</li>
</ul>
<h1>v3.2.3</h1>
<ul>
<li>Fix bugs in comment parsing in <code>autoInject</code>. (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1767">#1767</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1780">#1780</a>)</li>
</ul>
<h1>v3.2.2</h1>
<ul>
<li>Fix potential prototype pollution exploit</li>
</ul>
<h1>v3.2.1</h1>
<ul>
<li>Use <code>queueMicrotask</code> if available to the environment (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1761">#1761</a>)</li>
<li>Minor perf improvement in <code>priorityQueue</code> (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1727">#1727</a>)</li>
<li>More examples in documentation (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1726">#1726</a>)</li>
<li>Various doc fixes (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1708">#1708</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1712">#1712</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1717">#1717</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1740">#1740</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1739">#1739</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1749">#1749</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1756">#1756</a>)</li>
<li>Improved test coverage (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1754">#1754</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/caolan/async/commit/f3ab51af76ca87ebe3ec67b3dd6dec4959e04816"><code>f3ab51a</code></a> Version 3.2.4</li>
<li><a href="https://github.com/caolan/async/commit/7ea2cec7398b33a15daf5c3bd9bda6ae78caf297"><code>7ea2cec</code></a> Update built files</li>
<li><a href="https://github.com/caolan/async/commit/bef7befc734e4b712ab6ffc82463cc40c1037056"><code>bef7bef</code></a> update changelog</li>
<li><a href="https://github.com/caolan/async/commit/03eeab36ae5a0454bbf67b881f087692e0b7c7e4"><code>03eeab3</code></a> Bump yargs from 17.4.1 to 17.5.1 (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1843">#1843</a>)</li>
<li><a href="https://github.com/caolan/async/commit/387efcf80f5b2c454effd2a64c75ff3c634ec3bd"><code>387efcf</code></a> Bump eslint from 8.14.0 to 8.17.0 (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1849">#1849</a>)</li>
<li><a href="https://github.com/caolan/async/commit/131225a8c82fda93010b8b82da46e9a23b6b1816"><code>131225a</code></a> Bump karma from 6.3.19 to 6.3.20 (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1844">#1844</a>)</li>
<li><a href="https://github.com/caolan/async/commit/4cfa89cb240d9748d5bfee0656fbed08cf80cc10"><code>4cfa89c</code></a> Bump eslint from 8.14.0 to 8.16.0 (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1845">#1845</a>)</li>
<li><a href="https://github.com/caolan/async/commit/90e940cbb5a051db7c2a28169769f97eef99fdd6"><code>90e940c</code></a> Bump rollup from 2.71.1 to 2.75.5 (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1846">#1846</a>)</li>
<li><a href="https://github.com/caolan/async/commit/dd72cf5f614bcf2b08ae2678f6e8ffbd28136804"><code>dd72cf5</code></a> Bump <code>@​babel/eslint-parser</code> from 7.17.0 to 7.18.2 (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1847">#1847</a>)</li>
<li><a href="https://github.com/caolan/async/commit/4ae026e8da11f817f274f264dd3a9ec7ef3307c5"><code>4ae026e</code></a> Bump babel-minify from 0.5.1 to 0.5.2 (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1848">#1848</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/caolan/async/compare/v3.2.0...v3.2.4">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~hargasinski">hargasinski</a>, a new releaser for async since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=async&package-manager=npm_and_yarn&previous-version=3.2.0&new-version=3.2.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/university-course/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 17:07:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/university-course/pull/80" class=".btn">#80</a>
            </td>
            <td>
                <b>
                    chore(deps): bump async from 3.2.0 to 3.2.4 in /support/Lab05/chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [async](https://github.com/caolan/async) from 3.2.0 to 3.2.4.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/caolan/async/blob/master/CHANGELOG.md">async's changelog</a>.</em></p>
<blockquote>
<h1>v3.2.4</h1>
<ul>
<li>Fix a bug in <code>priorityQueue</code> where it didn't wait for the result. (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1725">#1725</a>)</li>
<li>Fix a bug where <code>unshiftAsync</code> was included in <code>priorityQueue</code>. (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1790">#1790</a>)</li>
</ul>
<h1>v3.2.3</h1>
<ul>
<li>Fix bugs in comment parsing in <code>autoInject</code>. (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1767">#1767</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1780">#1780</a>)</li>
</ul>
<h1>v3.2.2</h1>
<ul>
<li>Fix potential prototype pollution exploit</li>
</ul>
<h1>v3.2.1</h1>
<ul>
<li>Use <code>queueMicrotask</code> if available to the environment (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1761">#1761</a>)</li>
<li>Minor perf improvement in <code>priorityQueue</code> (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1727">#1727</a>)</li>
<li>More examples in documentation (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1726">#1726</a>)</li>
<li>Various doc fixes (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1708">#1708</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1712">#1712</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1717">#1717</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1740">#1740</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1739">#1739</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1749">#1749</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1756">#1756</a>)</li>
<li>Improved test coverage (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1754">#1754</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/caolan/async/commit/f3ab51af76ca87ebe3ec67b3dd6dec4959e04816"><code>f3ab51a</code></a> Version 3.2.4</li>
<li><a href="https://github.com/caolan/async/commit/7ea2cec7398b33a15daf5c3bd9bda6ae78caf297"><code>7ea2cec</code></a> Update built files</li>
<li><a href="https://github.com/caolan/async/commit/bef7befc734e4b712ab6ffc82463cc40c1037056"><code>bef7bef</code></a> update changelog</li>
<li><a href="https://github.com/caolan/async/commit/03eeab36ae5a0454bbf67b881f087692e0b7c7e4"><code>03eeab3</code></a> Bump yargs from 17.4.1 to 17.5.1 (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1843">#1843</a>)</li>
<li><a href="https://github.com/caolan/async/commit/387efcf80f5b2c454effd2a64c75ff3c634ec3bd"><code>387efcf</code></a> Bump eslint from 8.14.0 to 8.17.0 (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1849">#1849</a>)</li>
<li><a href="https://github.com/caolan/async/commit/131225a8c82fda93010b8b82da46e9a23b6b1816"><code>131225a</code></a> Bump karma from 6.3.19 to 6.3.20 (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1844">#1844</a>)</li>
<li><a href="https://github.com/caolan/async/commit/4cfa89cb240d9748d5bfee0656fbed08cf80cc10"><code>4cfa89c</code></a> Bump eslint from 8.14.0 to 8.16.0 (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1845">#1845</a>)</li>
<li><a href="https://github.com/caolan/async/commit/90e940cbb5a051db7c2a28169769f97eef99fdd6"><code>90e940c</code></a> Bump rollup from 2.71.1 to 2.75.5 (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1846">#1846</a>)</li>
<li><a href="https://github.com/caolan/async/commit/dd72cf5f614bcf2b08ae2678f6e8ffbd28136804"><code>dd72cf5</code></a> Bump <code>@​babel/eslint-parser</code> from 7.17.0 to 7.18.2 (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1847">#1847</a>)</li>
<li><a href="https://github.com/caolan/async/commit/4ae026e8da11f817f274f264dd3a9ec7ef3307c5"><code>4ae026e</code></a> Bump babel-minify from 0.5.1 to 0.5.2 (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1848">#1848</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/caolan/async/compare/v3.2.0...v3.2.4">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~hargasinski">hargasinski</a>, a new releaser for async since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=async&package-manager=npm_and_yarn&previous-version=3.2.0&new-version=3.2.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/university-course/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 17:07:39 +0000 UTC
    </div>
</div>

