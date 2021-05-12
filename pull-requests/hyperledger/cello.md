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
                PR <a href="https://github.com/hyperledger/cello/pull/241" class=".btn">#241</a>
            </td>
            <td>
                <b>
                    Bump nodemailer from 4.7.0 to 6.4.16 in /build_image/dockerhub/v0.9.0/user-dashboard
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [nodemailer](https://github.com/nodemailer/nodemailer) from 4.7.0 to 6.4.16.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/nodemailer/nodemailer/blob/master/CHANGELOG.md">nodemailer's changelog</a>.</em></p>
<blockquote>
<h2>6.4.16 2020-11-12</h2>
<ul>
<li>Applied updated prettier formating rules</li>
</ul>
<h2>6.4.15 2020-11-06</h2>
<ul>
<li>Minor changes in header key casing</li>
</ul>
<h2>6.4.14 2020-10-14</h2>
<ul>
<li>Disabled postinstall script</li>
</ul>
<h2>6.4.13 2020-10-02</h2>
<ul>
<li>Fix normalizeHeaderKey method for single node messages</li>
</ul>
<h2>6.4.12 2020-09-30</h2>
<ul>
<li>Better handling of attachment filenames that include quote symbols</li>
<li>Includes all information from the oath2 error response in the error message (Normal Gaussian) [1787f227]</li>
</ul>
<h2>6.4.11 2020-07-29</h2>
<ul>
<li>Fixed escape sequence handling in address parsing</li>
</ul>
<h2>6.4.10 2020-06-17</h2>
<ul>
<li>Fixed RFC822 output for MailComposer when using invalid content-type value. Mostly relevant if message attachments have stragne content-type values set.</li>
</ul>
<h2>6.4.7 2020-05-28</h2>
<ul>
<li>Always set charset=utf-8 for Content-Type headers</li>
<li>Catch error whn using invalid crypto.sign input</li>
</ul>
<h2>6.4.6 2020-03-20</h2>
<ul>
<li>fix: <code>requeueAttempts=n</code> should requeue <code>n</code> times (Patrick Malouin) [a27ed2f7]</li>
</ul>
<h2>6.4.4 2020-03-01</h2>
<ul>
<li>Add <code>options.forceAuth</code> for SMTP (Patrick Malouin) [a27ed2f7]</li>
</ul>
<h2>6.4.3 2020-02-22</h2>
<ul>
<li>Added an option to specify max number of requeues when connection closes unexpectedly (Igor Sechyn) [8a927f5a]</li>
</ul>
<h2>6.4.2 2019-12-11</h2>
<ul>
<li>Fixed bug where array item was used with a potentially empty array</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/nodemailer/nodemailer/commit/ba31c64c910d884579875c52d57ac45acc47aa54"><code>ba31c64</code></a> v6.4.16</li>
<li><a href="https://github.com/nodemailer/nodemailer/commit/7e7b2b23ed9a56ce60245bf1c7a444e5981a259b"><code>7e7b2b2</code></a> v6.4.15</li>
<li><a href="https://github.com/nodemailer/nodemailer/commit/fca2041bdf33e4a6cb61929abb2503fa4e630219"><code>fca2041</code></a> Update CHANGELOG.md</li>
<li><a href="https://github.com/nodemailer/nodemailer/commit/b4ccfa347a805d17c1d0fc5e719c2fb6cdc435e8"><code>b4ccfa3</code></a> Oups</li>
<li><a href="https://github.com/nodemailer/nodemailer/commit/24b93bf75f946b138fcad663effababd4a328972"><code>24b93bf</code></a> Add ethereal.email to  well-known/services.json</li>
<li><a href="https://github.com/nodemailer/nodemailer/commit/0f132fa0e5b65b105bfebc9a123515bd0217a15a"><code>0f132fa</code></a> doc: make the code a little more accessible with some code comments.</li>
<li><a href="https://github.com/nodemailer/nodemailer/commit/1815badec2ca1cf496a9fb728e0e941e8e16b65b"><code>1815bad</code></a> v6.4.14</li>
<li><a href="https://github.com/nodemailer/nodemailer/commit/dd26ddd9857280897a4e54ef16f037dfe8c62151"><code>dd26ddd</code></a> v6.4.13</li>
<li><a href="https://github.com/nodemailer/nodemailer/commit/455cfbe02658aeee6932ef845676c9de13dfb544"><code>455cfbe</code></a> v6.4.12</li>
<li><a href="https://github.com/nodemailer/nodemailer/commit/1787f227b34e6cb3a124fa5204ae89364a7c9d6b"><code>1787f22</code></a> Includes all information from the oath2 error response in the error message (...</li>
<li>Additional commits viewable in <a href="https://github.com/nodemailer/nodemailer/compare/v4.7.0...v6.4.16">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=nodemailer&package-manager=npm_and_yarn&previous-version=4.7.0&new-version=6.4.16)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cello/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-12 01:12:34 +0000 UTC
    </div>
</div>

