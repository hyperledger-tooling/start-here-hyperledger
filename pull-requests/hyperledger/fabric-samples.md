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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/722" class=".btn">#722</a>
            </td>
            <td>
                <b>
                    Bump nconf from 0.11.3 to 0.11.4 in /asset-transfer-basic/rest-api-typescript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [nconf](https://github.com/flatiron/nconf) from 0.11.3 to 0.11.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/flatiron/nconf/releases">nconf's releases</a>.</em></p>
<blockquote>
<h2>v0.11.4</h2>
<p>Fixes:</p>
<ul>
<li>Prevent improper usage of the memory store from polluting the object prototype (<a href="https://github-redirect.dependabot.com/flatiron/nconf/issues/397">#397</a>) (<a href="https://github.com/mhamann"><code>@​mhamann</code></a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/indexzero/nconf/commit/f25feb2913fc21a5d80039f6213c2d9ae906ec29"><code>f25feb2</code></a> 0.11.4</li>
<li><a href="https://github.com/indexzero/nconf/commit/2e9e4538a8b9c33dabdafd8ec1dc6064fac9d070"><code>2e9e453</code></a> chore: disable package-lock, since this is a lib</li>
<li><a href="https://github.com/indexzero/nconf/commit/7aa94020e493eca482239492d0126d63b1ce2630"><code>7aa9402</code></a> chore: update node version test matrix</li>
<li><a href="https://github.com/indexzero/nconf/commit/feaba562b812b21215897f71b0c8b3bf39cf8d7d"><code>feaba56</code></a> fix(security): prevent prototype pollution in memory store (<a href="https://github-redirect.dependabot.com/flatiron/nconf/issues/397">#397</a>)</li>
<li>See full diff in <a href="https://github.com/flatiron/nconf/compare/v0.11.3...v0.11.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=nconf&package-manager=npm_and_yarn&previous-version=0.11.3&new-version=0.11.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-04-22 23:09:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/721" class=".btn">#721</a>
            </td>
            <td>
                <b>
                    Use maven central for gateway client dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates the release-1.4 commercial paper client applications to pull the gateway jars from Maven central.

This PR supersedes PR #585 (abandoned / closed) 
    
Signed-off-by: lyd <luoyaodong98@gmail.com>

Co-authored-by: Josh Kneubuhl <jkneubuh@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 14:57:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/720" class=".btn">#720</a>
            </td>
            <td>
                <b>
                    test-network-k8s: Remove kubectl binary (again)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Since kubectl binary is mistakenly added again in PR #714, this patch removes it.

It seems that the following commit was mixed up with another PR commits, including PR #713.
https://github.com/hyperledger/fabric-samples/pull/714/commits/24c296c8a8e6966595c6395bcc4ba9948217176a
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 02:15:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/719" class=".btn">#719</a>
            </td>
            <td>
                <b>
                    test-network-k8s: Remove kubectl binary
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In PR#713, I mistakenly added kubectl binary, so this patch removes it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-19 08:35:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/718" class=".btn">#718</a>
            </td>
            <td>
                <b>
                    test-network-k8s: Some minor improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This patch includes some minor improvements, such as:
- Fix typos and broken links
- Correct chaincode type of asset-transfer-basic-debug
  (seems it should be ccaas)

Signed-off-by: Tatsuya Sato <tatsuya.sato.so@hitachi.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-19 07:38:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/717" class=".btn">#717</a>
            </td>
            <td>
                <b>
                    Can implement a simple CURD
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Leave the serialization of parameters to the upper level

Signed-off-by: D <gvssimux@qq.com>

Co-authored-by: D <gvssimux@qq.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-19 02:43:35 +0000 UTC
    </div>
</div>

