---
layout: default
title: fabric-chaincode-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-chaincode-go
---

# fabric-chaincode-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-chaincode-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/53" class=".btn">#53</a>
            </td>
            <td>
                <b>
                    Add GHA support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-05 10:42:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/52" class=".btn">#52</a>
            </td>
            <td>
                <b>
                    Bump github.com/stretchr/testify from 1.7.0 to 1.8.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/stretchr/testify](https://github.com/stretchr/testify) from 1.7.0 to 1.8.0.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/stretchr/testify/commit/181cea6eab8b2de7071383eca4be32a424db38dd"><code>181cea6</code></a> impr: <code>CallerInfo</code> should print full paths to the terminal (<a href="https://github-redirect.dependabot.com/stretchr/testify/issues/1201">#1201</a>)</li>
<li><a href="https://github.com/stretchr/testify/commit/cf1284f8dd6f0bf34eed4ab8808ef88f40f7d00f"><code>cf1284f</code></a> Allow mock expectations to be ordered (<a href="https://github-redirect.dependabot.com/stretchr/testify/issues/1106">#1106</a>)</li>
<li><a href="https://github.com/stretchr/testify/commit/66eef0ef3adb4691cdc275620c9a129f2f98935a"><code>66eef0e</code></a> fix: assert.MapSubset (or just support maps in assert.Subset) (<a href="https://github-redirect.dependabot.com/stretchr/testify/issues/1178">#1178</a>)</li>
<li><a href="https://github.com/stretchr/testify/commit/2fab6dffcf101c5a79fc8f3cd67a3541432db5fd"><code>2fab6df</code></a> Add WithinTimeRange method (<a href="https://github-redirect.dependabot.com/stretchr/testify/issues/1188">#1188</a>)</li>
<li><a href="https://github.com/stretchr/testify/commit/b5ce16571001d6e96e1693ac891fed5c2510c651"><code>b5ce165</code></a> fixing panic in calls to assertion with nil m.mutex (<a href="https://github-redirect.dependabot.com/stretchr/testify/issues/1212">#1212</a>)</li>
<li><a href="https://github.com/stretchr/testify/commit/c206b2e823e70c1e4e7ca8eded9e410acc8f71be"><code>c206b2e</code></a> Mock can be deadlocked by a panic (<a href="https://github-redirect.dependabot.com/stretchr/testify/issues/1157">#1157</a>)</li>
<li><a href="https://github.com/stretchr/testify/commit/1b73601ae8d1c3e389e93092f595b1f6e3d68251"><code>1b73601</code></a> suite: correctly set stats on test panic (<a href="https://github-redirect.dependabot.com/stretchr/testify/issues/1195">#1195</a>)</li>
<li><a href="https://github.com/stretchr/testify/commit/ba1076d8b3b67cdaf7bf92c95b3641636a039be2"><code>ba1076d</code></a> Add .Unset method to mock (<a href="https://github-redirect.dependabot.com/stretchr/testify/issues/982">#982</a>)</li>
<li><a href="https://github.com/stretchr/testify/commit/c31ea0312f8a96ca55801db5ebdf62119800fb70"><code>c31ea03</code></a> Support comparing byte slice (<a href="https://github-redirect.dependabot.com/stretchr/testify/issues/1202">#1202</a>)</li>
<li><a href="https://github.com/stretchr/testify/commit/48391ba5eb8c5f49132138e67ec112d180b88f63"><code>48391ba</code></a> Fix panic in AssertExpectations for mocks without expectations (<a href="https://github-redirect.dependabot.com/stretchr/testify/issues/1207">#1207</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/stretchr/testify/compare/v1.7.0...v1.8.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/stretchr/testify&package-manager=go_modules&previous-version=1.7.0&new-version=1.8.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-30 04:40:07 +0000 UTC
    </div>
</div>

