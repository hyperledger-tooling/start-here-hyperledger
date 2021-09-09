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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/314" class=".btn">#314</a>
            </td>
            <td>
                <b>
                    [#issue-313] cmdline lib function list and getinfo has no info return
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added information processing of function list and function getinfo

Close #issue-313

Signed-off-by: zhaoshihong<523713078@qq.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-02 08:06:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/312" class=".btn">#312</a>
            </td>
            <td>
                <b>
                    Bump tar from 4.4.15 to 4.4.19 in /build_image/dockerhub/v0.9.0/user-dashboard
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [tar](https://github.com/npm/node-tar) from 4.4.15 to 4.4.19.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/npm/node-tar/commit/9a6faa017ca90538840f3ae2ccdb4550ac3f4dcf"><code>9a6faa0</code></a> 4.4.19</li>
<li><a href="https://github.com/npm/node-tar/commit/70ef812593184cc54ea1bc74c5dae2d22995002d"><code>70ef812</code></a> drop dirCache for symlink on all platforms</li>
<li><a href="https://github.com/npm/node-tar/commit/3e35515c09da615ac268254bed85fe43ee71e2f0"><code>3e35515</code></a> 4.4.18</li>
<li><a href="https://github.com/npm/node-tar/commit/52b09e309bcae0c741a7eb79a17ef36e7828b946"><code>52b09e3</code></a> fix: prevent path escape using drive-relative paths</li>
<li><a href="https://github.com/npm/node-tar/commit/bb93ba243746f705092905da1955ac3b0509ba1e"><code>bb93ba2</code></a> fix: reserve paths properly for unicode, windows</li>
<li><a href="https://github.com/npm/node-tar/commit/2f1bca027286c23e110b8dfc7efc10756fa3db5a"><code>2f1bca0</code></a> fix: prune dirCache properly for unicode, windows</li>
<li><a href="https://github.com/npm/node-tar/commit/9bf70a8cf725c3af5fe2270f1e5d2e06d1559b93"><code>9bf70a8</code></a> 4.4.17</li>
<li><a href="https://github.com/npm/node-tar/commit/6aafff0a8621ba9509b63654bde28762be373d58"><code>6aafff0</code></a> fix: skip extract if linkpath is stripped entirely</li>
<li><a href="https://github.com/npm/node-tar/commit/5c5059a69c2aaaedfe4e9766e102ae9fb79e8255"><code>5c5059a</code></a> fix: reserve paths case-insensitively</li>
<li><a href="https://github.com/npm/node-tar/commit/fd6accba697070560f301604b8f5f7e2995a2a8b"><code>fd6accb</code></a> 4.4.16</li>
<li>Additional commits viewable in <a href="https://github.com/npm/node-tar/compare/v4.4.15...v4.4.19">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tar&package-manager=npm_and_yarn&previous-version=4.4.15&new-version=4.4.19)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-09-02 05:04:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/311" class=".btn">#311</a>
            </td>
            <td>
                <b>
                    Update Dockerfile.in
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                update python3 in build_image/docker/agent/ansible/Dockerfile.in. Because Ubuntu: latest is version 20.04, there is no Python-pip source, so errors will be executed all the time
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-02 02:21:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/310" class=".btn">#310</a>
            </td>
            <td>
                <b>
                    add fabric tools
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                *add fabric tools

Signed-off-by: XuHugo <xq-310@163.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-02 01:43:05 +0000 UTC
    </div>
</div>

