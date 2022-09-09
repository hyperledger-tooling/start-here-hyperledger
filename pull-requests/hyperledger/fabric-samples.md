---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/828" class=".btn">#828</a>
            </td>
            <td>
                <b>
                    Bump passport from 0.4.1 to 0.6.0 in /asset-transfer-basic/rest-api-typescript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [passport](https://github.com/jaredhanson/passport) from 0.4.1 to 0.6.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/jaredhanson/passport/blob/master/CHANGELOG.md">passport's changelog</a>.</em></p>
<blockquote>
<h2>[0.6.0] - 2022-05-20</h2>
<h3>Added</h3>
<ul>
<li><code>authenticate()</code>, <code>req#login</code>, and <code>req#logout</code> accept a
<code>keepSessionInfo: true</code> option to keep session information after regenerating
the session.</li>
</ul>
<h3>Changed</h3>
<ul>
<li><code>req#login()</code> and <code>req#logout()</code> regenerate the the session and clear session
information by default.</li>
<li><code>req#logout()</code> is now an asynchronous function and requires a callback
function as the last argument.</li>
</ul>
<h3>Security</h3>
<ul>
<li>Improved robustness against session fixation attacks in cases where there is
physical access to the same system or the application is susceptible to
cross-site scripting (XSS).</li>
</ul>
<h2>[0.5.3] - 2022-05-16</h2>
<h3>Fixed</h3>
<ul>
<li><code>initialize()</code> middleware extends request with <code>login()</code>, <code>logIn()</code>,
<code>logout()</code>, <code>logOut()</code>, <code>isAuthenticated()</code>, and <code>isUnauthenticated()</code> functions
again, reverting change from 0.5.1.</li>
</ul>
<h2>[0.5.2] - 2021-12-16</h2>
<h3>Fixed</h3>
<ul>
<li>Introduced a compatibility layer for strategies that depend directly on
<code>passport@0.4.x</code> or earlier (such as <code>passport-azure-ad</code>), which were
broken by the removal of private variables in <code>passport@0.5.1</code>.</li>
</ul>
<h2>[0.5.1] - 2021-12-15</h2>
<h3>Added</h3>
<ul>
<li>Informative error message in session strategy if session support is not
available.</li>
</ul>
<h3>Changed</h3>
<ul>
<li><code>authenticate()</code> middleware, rather than <code>initialize()</code> middleware, extends
request with <code>login()</code>, <code>logIn()</code>, <code>logout()</code>, <code>logOut()</code>, <code>isAuthenticated()</code>,
and <code>isUnauthenticated()</code> functions.</li>
</ul>
<h2>[0.5.0] - 2021-09-23</h2>
<h3>Changed</h3>
<ul>
<li><code>initialize()</code> middleware extends request with <code>login()</code>, <code>logIn()</code>,
<code>logout()</code>, <code>logOut()</code>, <code>isAuthenticated()</code>, and <code>isUnauthenticated()</code>
functions.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jaredhanson/passport/commit/c33067bc5aa81a6dd827076d810bf788bb6acac7"><code>c33067b</code></a> 0.6.0</li>
<li><a href="https://github.com/jaredhanson/passport/commit/3052bb4717673b88a27981f6bc91a1f585889e5c"><code>3052bb4</code></a> Update changelog.</li>
<li><a href="https://github.com/jaredhanson/passport/commit/42630cbd1ffd44d146ff96f0a4be6f3c12f81d75"><code>42630cb</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/jaredhanson/passport/issues/900">#900</a> from jaredhanson/fix-fixation</li>
<li><a href="https://github.com/jaredhanson/passport/commit/8dd79fe5f3f414435c4e0561fc925fb7ab6c8efb"><code>8dd79fe</code></a> Use utils-merge rather than Object.assign for compatibility.</li>
<li><a href="https://github.com/jaredhanson/passport/commit/4f6bd5b254454d3f61c3236e8f1dd33472704fd3"><code>4f6bd5b</code></a> Change keepSessionData to keepSessionData.</li>
<li><a href="https://github.com/jaredhanson/passport/commit/46756e56db671a822490f3d6c103a33a6691047d"><code>46756e5</code></a> Silence verbose logging.</li>
<li><a href="https://github.com/jaredhanson/passport/commit/987b1918a2c5056531bbd325a2ff888a3595b2df"><code>987b191</code></a> Add tests.</li>
<li><a href="https://github.com/jaredhanson/passport/commit/f8a175f1145c4efdffa7e4c511a642f608e11c0f"><code>f8a175f</code></a> Add tests.</li>
<li><a href="https://github.com/jaredhanson/passport/commit/29a90d68dd5d4bc807bc658cfe49fba968b34d7d"><code>29a90d6</code></a> No need to guard callback existence.</li>
<li><a href="https://github.com/jaredhanson/passport/commit/bfba8a1ab44b658f745e33e3484b389f0751cdc0"><code>bfba8a1</code></a> Add tests.</li>
<li>Additional commits viewable in <a href="https://github.com/jaredhanson/passport/compare/v0.4.1...v0.6.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=passport&package-manager=npm_and_yarn&previous-version=0.4.1&new-version=0.6.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-09 12:33:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/827" class=".btn">#827</a>
            </td>
            <td>
                <b>
                    Fix test network chaincode deploy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Correctly check for installed chaincode and enable the same chaincode to be deployed on different channels

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-09 09:36:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/826" class=".btn">#826</a>
            </td>
            <td>
                <b>
                    Sample application to add a golang version to commercial-paper
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Fang Yuan <wojiushifangyuanlove@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-08 07:34:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/825" class=".btn">#825</a>
            </td>
            <td>
                <b>
                    Update chaincode/abstore, add parameter judgment when the transaction ma…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …kes payment.

Signed-off-by: yjwxfq <yjwxfq@163.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-08 02:50:34 +0000 UTC
    </div>
</div>

