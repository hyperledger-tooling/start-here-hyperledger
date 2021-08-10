---
layout: default
title: aries-agent-test-harness
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-agent-test-harness
---

# aries-agent-test-harness <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-agent-test-harness){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/318" class=".btn">#318</a>
            </td>
            <td>
                <b>
                    fix: afgo renamed jsonld endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-10 14:51:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/317" class=".btn">#317</a>
            </td>
            <td>
                <b>
                    Changes by create-pull-request action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Automated changes by [create-pull-request](https://github.com/peter-evans/create-pull-request) GitHub action
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-10 03:52:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/316" class=".btn">#316</a>
            </td>
            <td>
                <b>
                    fix for failing mobile tests with new connection reuse PR
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR will fix the failing Mobile Tests because of the interjection of getting a public did on the `And "Faber" and "Bob" have an existing connection` step. The handler now just accepts the 500 not found from the mobile backchannel and continues to create the connection without reporting the 500. 

Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-09 23:03:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/315" class=".btn">#315</a>
            </td>
            <td>
                <b>
                    chore: update to work with latest afgo (removes a bug workaround)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-05 04:58:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/314" class=".btn">#314</a>
            </td>
            <td>
                <b>
                    build(deps): Bump tar from 6.1.0 to 6.1.4 in /aries-backchannels/javascript/server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [tar](https://github.com/npm/node-tar) from 6.1.0 to 6.1.4.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/npm/node-tar/commit/bf693837b3dcfeb76878b212310302dc5dc3d3dc"><code>bf69383</code></a> 6.1.4</li>
<li><a href="https://github.com/npm/node-tar/commit/06cbde5935aa7643f578f874de84a7da2a74fe3a"><code>06cbde5</code></a> Avoid an unlikely but theoretically possible redos</li>
<li><a href="https://github.com/npm/node-tar/commit/0b78386c53b00dce422742e19de94f2a4d9389f3"><code>0b78386</code></a> 6.1.3</li>
<li><a href="https://github.com/npm/node-tar/commit/56c24b0da75c59a7c77b7551ceb887af76dc6fa2"><code>56c24b0</code></a> fix: properly handle top-level files when using strip</li>
<li><a href="https://github.com/npm/node-tar/commit/8d7522968b5185fc666e299711a74033c17fca45"><code>8d75229</code></a> ci: Create codeql workflow</li>
<li><a href="https://github.com/npm/node-tar/commit/3f7b20097e0daba10441507becbf5b87c6b83b8b"><code>3f7b200</code></a> 6.1.2</li>
<li><a href="https://github.com/npm/node-tar/commit/9dbdeb6df8e9dbd96fa9e84341b9d74734be6c20"><code>9dbdeb6</code></a> Remove paths from dirCache when no longer dirs</li>
<li><a href="https://github.com/npm/node-tar/commit/1e33534e1e96ca6385b3a4749876aea2cda61cea"><code>1e33534</code></a> 6.1.1</li>
<li><a href="https://github.com/npm/node-tar/commit/1f036ca23f64a547bdd6c79c1a44bc62e8115da4"><code>1f036ca</code></a> fix: strip absolute paths more comprehensively</li>
<li><a href="https://github.com/npm/node-tar/commit/1b94260e87b3eacad801314ce4d5759716c46058"><code>1b94260</code></a> tap@15</li>
<li>See full diff in <a href="https://github.com/npm/node-tar/compare/v6.1.0...v6.1.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tar&package-manager=npm_and_yarn&previous-version=6.1.0&new-version=6.1.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-agent-test-harness/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-04 00:25:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/313" class=".btn">#313</a>
            </td>
            <td>
                <b>
                    Added Verity Backchannel, only connection protocol for now
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is the initial work for a backchannel for the Verity Agent Service. The purpose of this is just to get the plumbing in place, more protocols will be added over time
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-03 21:34:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/312" class=".btn">#312</a>
            </td>
            <td>
                <b>
                    Connection reuse support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Details on how to use connection reuse in AATH is located in CONNECTION-REUSE.md.

Closes #265 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-03 20:47:58 +0000 UTC
    </div>
</div>

