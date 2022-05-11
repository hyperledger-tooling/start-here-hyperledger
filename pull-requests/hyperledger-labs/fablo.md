---
layout: default
title: fablo
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fablo
---

# fablo <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fablo){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/312" class=".btn">#312</a>
            </td>
            <td>
                <b>
                    Attach fabric-ca-server-config.yaml as a volume
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ❗ ❗  Should be merge after https://github.com/hyperledger-labs/fablo/pull/308

Signed-off-by: Grzegorz Hejduk <grzegorz.hejduk@softwaremill.com>

#168
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-11 05:53:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/311" class=".btn">#311</a>
            </td>
            <td>
                <b>
                    Add version config for fabric-nodeenv, update Node version warnings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Note- replaces previous pull request #309. I used git rebase to add DCO statements and amend multiple commits, so pushed a new branch rather than rewriting history on an already-published branch. 

https://github.com/hyperledger-labs/fablo/issues/274 Update Node.js runtime compatibility

The compatibility information in fabric-chaincode-node
(https://github.com/hyperledger/fabric-chaincode-node/blob/main/COMPATIBILITY.md)
lists an environment variable that can be used on a peer that
hosts chaincode to alter the Node.js runtime used.

This commit adds support for setting that environment variable
to the fablo global config. It also updates fablo to support fabric version 2.4.2.

Based on some recent patches to fabric-chaincode-node:

https://github.com/hyperledger/fabric-chaincode-node/commit/d9cfc3d0b35fad4ed7e72b8ced370bef32f1d0b9
https://github.com/hyperledger/fabric-chaincode-node/blob/main/release_notes/v2.4.2.txt
"This release corrects the 2.4 nodeenv docker image to be Node 16, and ..."

A node version mapping was added similar to the existing javaenv
mapping to used the fixed fabric-nodeenv docker image if
2.4 or 2.4.1 are supplied.
(src/extend-config/extendGlobal.ts)
Probabably "2.4" should be removed from this mapping at such
time that that image incorporates the fix released in 2.4.2,
but for now it was added to potentially avoid cases
where Node v12 is still being unexpected used on the peers.

The Node.js warning message is also updated to recommend 16
if the fabric version is 2.4 or higher, and 12 otherwise.
Referenced existing github issue 274 for this fix. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-10 21:37:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/310" class=".btn">#310</a>
            </td>
            <td>
                <b>
                    Bump color-string from 1.5.3 to 1.9.1 in /samples/chaincodes/chaincode-kv-node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [color-string](https://github.com/Qix-/color-string) from 1.5.3 to 1.9.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/Qix-/color-string/releases">color-string's releases</a>.</em></p>
<blockquote>
<h2>1.9.0</h2>
<h1>Minor Release 1.9.0</h1>
<ul>
<li>Add parsing of exponential alpha values for HWB and HSL (<a href="https://github.com/Qix-/color-string/issues/66">#66</a>)</li>
</ul>
<p>Thanks to <a href="https://github.com/babycannotsay"><code>@​babycannotsay</code></a> for their contribution!</p>
<h2>1.8.2</h2>
<h1>Patch release 1.8.2</h1>
<ul>
<li>Fix incorrect handling of optional comma in rgb() regex (<a href="https://github.com/Qix-/color-string/issues/65">#65</a>)</li>
</ul>
<p>Thanks to <a href="https://github.com/gerdasi"><code>@​gerdasi</code></a> and <a href="https://github.com/mastertheblaster"><code>@​mastertheblaster</code></a> for reporting and confirming the bug!</p>
<h2>1.8.1</h2>
<h1>Patch release 1.8.1</h1>
<ul>
<li>Fix rgb alpha percentage parsing from int to float (<a href="https://github.com/Qix-/color-string/issues/61">#61</a>)</li>
</ul>
<p>Thanks to <a href="https://github.com/clytras"><code>@​clytras</code></a> for their contribution!</p>
<h2>1.8.0</h2>
<h1>Minor release 1.8.0</h1>
<ul>
<li>Add anchors to keyword regex (<a href="https://github.com/Qix-/color-string/issues/64">#64</a>)</li>
</ul>
<p>Thanks to <a href="https://github.com/cq360767996"><code>@​cq360767996</code></a> for their contribution!</p>
<h2>1.7.4</h2>
<h1>Patch Release 1.7.4</h1>
<ul>
<li>Fix bug in <code>.to.hex()</code> output if the inputs aren't rounded numbers (<a href="https://github.com/Qix-/color-string/issues/25">#25</a>)</li>
</ul>
<h2>1.7.3</h2>
<h1>Patch Release 1.7.3</h1>
<ul>
<li>Fix hue modulo operation (<a href="https://github.com/Qix-/color-string/issues/50">#50</a>)</li>
</ul>
<p>Thanks to <a href="https://github.com/adroitwhiz"><code>@​adroitwhiz</code></a> for their contributions.</p>
<h2>1.7.2</h2>
<h1>Patch Release 1.7.2</h1>
<ul>
<li>Fix issue where color-string with incorrectly return a color for properties on Object's prototype like &quot;constructor&quot;. (<a href="https://github.com/Qix-/color-string/issues/45">#45</a>)</li>
</ul>
<p>Thanks to <a href="https://github.com/tolmasky"><code>@​tolmasky</code></a> for their contributions.</p>
<h2>1.7.1</h2>
<h1>Patch release 1.7.1</h1>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/Qix-/color-string/commits/1.9.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=color-string&package-manager=npm_and_yarn&previous-version=1.5.3&new-version=1.9.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fablo/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-10 08:49:19 +0000 UTC
    </div>
</div>

