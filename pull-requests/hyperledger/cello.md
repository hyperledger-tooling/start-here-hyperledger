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
                PR <a href="https://github.com/hyperledger/cello/pull/329" class=".btn">#329</a>
            </td>
            <td>
                <b>
                    Bump sqlparse from 0.4.1 to 0.4.2 in /src/api-engine
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [sqlparse](https://github.com/andialbrecht/sqlparse) from 0.4.1 to 0.4.2.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/andialbrecht/sqlparse/blob/master/CHANGELOG">sqlparse's changelog</a>.</em></p>
<blockquote>
<h2>Release 0.4.2 (Sep 10, 2021)</h2>
<p>Notable Changes</p>
<ul>
<li>IMPORTANT: This release fixes a security vulnerability in the
strip comments filter. In this filter a regular expression that was
vulnerable to ReDOS (Regular Expression Denial of Service) was
used. See the security advisory for details: <a href="https://github.com/andialbrecht/sqlparse/security/advisories/GHSA-p5w8-wqhj-9hhf">https://github.com/andialbrecht/sqlparse/security/advisories/GHSA-p5w8-wqhj-9hhf</a>
The vulnerability was discovered by <a href="https://github.com/erik-krogh"><code>@​erik-krogh</code></a> and <a href="https://github.com/yoff"><code>@​yoff</code></a> from
GitHub Security Lab (GHSL). Thanks for reporting!</li>
</ul>
<p>Enhancements</p>
<ul>
<li>Add ELSIF as keyword (issue584).</li>
<li>Add CONFLICT and ON_ERROR_STOP keywords (pr595, by j-martin).</li>
</ul>
<p>Bug Fixes</p>
<ul>
<li>Fix parsing of backticks (issue588).</li>
<li>Fix parsing of scientific number (issue399).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/b1f76f6fa9763ee0f1d3a3870f05565abf1314e8"><code>b1f76f6</code></a> Update changelog.</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/3eec44e52233c68ea8299a16b36ec7f2ad0c2fe3"><code>3eec44e</code></a> Update Changelog and bump version.</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/8238a9e450ed1524e40cb3a8b0b3c00606903aeb"><code>8238a9e</code></a> Optimize regular expression for identifying line breaks in comments.</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/e66046785b816e5c2d22f101f36faefd19c4a771"><code>e660467</code></a> Fix parsing of scientific numbers (fixes <a href="https://github-redirect.dependabot.com/andialbrecht/sqlparse/issues/399">#399</a>).</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/23d29933ddc4272b495d36e0e32d3eaf0c3ef76d"><code>23d2993</code></a> Update authors and changelog.</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/acc2810d1275154c4e93debe82d319e15c507d61"><code>acc2810</code></a> keyword, add ON_ERROR_STOP</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/282bcf1048c472e3eddd83a331f8d4e857a2c5eb"><code>282bcf1</code></a> keyword, add CONFLICT to postgres keywords</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/63885dd5f1be3fe519fceb0a21f1f87fdc6aa973"><code>63885dd</code></a> Add ELSIF as keyword (fixes <a href="https://github-redirect.dependabot.com/andialbrecht/sqlparse/issues/584">#584</a>).</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/e575ae2c37359ab51b23ce44ccda4bb9bbfd3a5f"><code>e575ae2</code></a> Fix parsing of backticks (fixes <a href="https://github-redirect.dependabot.com/andialbrecht/sqlparse/issues/588">#588</a>).</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/fe39072fc24e879034fb1e439fb0a47c7c66d4a2"><code>fe39072</code></a> Switch back to development mode.</li>
<li>Additional commits viewable in <a href="https://github.com/andialbrecht/sqlparse/compare/0.4.1...0.4.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=sqlparse&package-manager=pip&previous-version=0.4.1&new-version=0.4.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-09-10 18:56:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/328" class=".btn">#328</a>
            </td>
            <td>
                <b>
                    Implemented channel creating operation with peer channel cli.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Create a channel for the current user, and then add all peer nodes from
the org to the channel. Finally, set the first peer node as the anchor
peer.

Signed-off-by: Yuanmao Zhu <zhu.yuanmao18@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-10 05:09:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/327" class=".btn">#327</a>
            </td>
            <td>
                <b>
                    [#issue-326] cmdlinelib feature of approveformyorg && queryapproved f…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …unctions

implement the cmdlinelib feature of approveformyorg && queryapproved functions

Close #issue-326

Signed-off-by: tianxuanhong <523713078@qq.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 00:41:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/325" class=".btn">#325</a>
            </td>
            <td>
                <b>
                    create channel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                *first,update configtx.yaml.
*then,create channel.tx.

Signed-off-by: XuHugo <xq-310@163.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-08 15:04:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/324" class=".btn">#324</a>
            </td>
            <td>
                <b>
                    [#issue-319] There is a risk of obtaining expired information
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If the file has already been created. Then an exception occurs, at which point the file is not deleted, and the next time the function is called, the information continues to be written to the file, causing the user to get an exception.

Perhaps using files is not a good method;

Close #issue-319

Signed-off-by: zhaoshihong <523713078@qq.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-06 12:22:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/323" class=".btn">#323</a>
            </td>
            <td>
                <b>
                    [#issue-322]Modify the agent,network and node list to display abnorma…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …l problems

Modify the agent,network and node list to display abnormal problems

Signed-off-by: fengyang_sy <fengyang.09186@h3c.com>

Close #322 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-05 00:44:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/321" class=".btn">#321</a>
            </td>
            <td>
                <b>
                    [#issue-320] lifecycle_query_installed&lifecycle_get_installed_package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                lifecycle_query_installed will get all chaincode information installed in peer. lifecycle_get_installed_package will get all chaincode files installed in peer,
it's input is packid_id.

Close #issue-320

Signed-off-by: zhaoshihong<523713078@qq.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-04 08:52:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/318" class=".btn">#318</a>
            </td>
            <td>
                <b>
                    [#issue-317] cmdLineLib of chaincode operation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Construct the chaincode class and implement the methods of chaincode package and chaincode install

Close #issue-317

Signed-off-by: zhaoshihong <523713078@qq.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-04 06:58:58 +0000 UTC
    </div>
</div>

