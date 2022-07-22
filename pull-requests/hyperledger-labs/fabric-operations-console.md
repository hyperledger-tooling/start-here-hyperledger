---
layout: default
title: fabric-operations-console
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-operations-console
---

# fabric-operations-console <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-operations-console){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/270" class=".btn">#270</a>
            </td>
            <td>
                <b>
                    remove console component auto restarts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
if the `node_ou` field of a component is edited, the console should not send a restart since the operator will already do that


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-21 19:17:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/269" class=".btn">#269</a>
            </td>
            <td>
                <b>
                    prevent blank pending channel tile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
It's possible to create a blank pending channel tile by creating a real tile, and then canceling the create channel wizard right after starting it. This PR prevents any blank pending channel tiles.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-20 21:05:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/268" class=".btn">#268</a>
            </td>
            <td>
                <b>
                    create channel - show error if 0 orderers are in selected msps
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
Filtering out msps in https://github.com/hyperledger-labs/fabric-operations-console/pull/264  (for the create channel wizard) was the wrong approach.

What we really needed was a warning/error if the user had not selected any MSPs with a known orderer. So with this PR you can select any MSP you want, as long as 1 or more of them have orderers.

This prevents the error we are trying to stop where a user selects MSPs with 0 orderers && leaves the consenter step as `default` and we create a problematic genesis block since it has 0 consenters.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-20 20:41:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/267" class=".btn">#267</a>
            </td>
            <td>
                <b>
                    Bump terser from 4.8.0 to 4.8.1 in /packages/apollo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [terser](https://github.com/terser/terser) from 4.8.0 to 4.8.1.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/terser/terser/blob/master/CHANGELOG.md">terser's changelog</a>.</em></p>
<blockquote>
<h2>v4.8.1 (backport)</h2>
<ul>
<li>Security fix for RegExps that should not be evaluated (regexp DDOS)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/terser/terser/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=terser&package-manager=npm_and_yarn&previous-version=4.8.0&new-version=4.8.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-operations-console/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-20 18:32:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/265" class=".btn">#265</a>
            </td>
            <td>
                <b>
                    Bump terser from 5.10.0 to 5.14.2 in /packages/stitch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [terser](https://github.com/terser/terser) from 5.10.0 to 5.14.2.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/terser/terser/blob/master/CHANGELOG.md">terser's changelog</a>.</em></p>
<blockquote>
<h2>v5.14.2</h2>
<ul>
<li>Security fix for RegExps that should not be evaluated (regexp DDOS)</li>
<li>Source maps improvements (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1211">#1211</a>)</li>
<li>Performance improvements in long property access evaluation (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1213">#1213</a>)</li>
</ul>
<h2>v5.14.1</h2>
<ul>
<li>keep_numbers option added to TypeScript defs (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1208">#1208</a>)</li>
<li>Fixed parsing of nested template strings (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1204">#1204</a>)</li>
</ul>
<h2>v5.14.0</h2>
<ul>
<li>Switched to <code>@​jridgewell/source-map</code> for sourcemap generation (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1190">#1190</a>, <a href="https://github-redirect.dependabot.com/terser/terser/issues/1181">#1181</a>)</li>
<li>Fixed source maps with non-terminated segments (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1106">#1106</a>)</li>
<li>Enabled typescript types to be imported from the package (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1194">#1194</a>)</li>
<li>Extra DOM props have been added (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1191">#1191</a>)</li>
<li>Delete the AST while generating code, as a means to save RAM</li>
</ul>
<h2>v5.13.1</h2>
<ul>
<li>Removed self-assignments (<code>varname=varname</code>) (closes <a href="https://github-redirect.dependabot.com/terser/terser/issues/1081">#1081</a>)</li>
<li>Separated inlining code (for inlining things into references, or removing IIFEs)</li>
<li>Allow multiple identifiers with the same name in <code>var</code> destructuring (eg <code>var { a, a } = x</code>) (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1176">#1176</a>)</li>
</ul>
<h2>v5.13.0</h2>
<ul>
<li>All calls to eval() were removed (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1171">#1171</a>, <a href="https://github-redirect.dependabot.com/terser/terser/issues/1184">#1184</a>)</li>
<li><code>source-map</code> was updated to 0.8.0-beta.0 (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1164">#1164</a>)</li>
<li>NavigatorUAData was added to domprops to avoid property mangling (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1166">#1166</a>)</li>
</ul>
<h2>v5.12.1</h2>
<ul>
<li>Fixed an issue with function definitions inside blocks (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1155">#1155</a>)</li>
<li>Fixed parens of <code>new</code> in some situations (closes <a href="https://github-redirect.dependabot.com/terser/terser/issues/1159">#1159</a>)</li>
</ul>
<h2>v5.12.0</h2>
<ul>
<li><code>TERSER_DEBUG_DIR</code> environment variable</li>
<li><a href="https://github.com/copyright"><code>@​copyright</code></a> comments are now preserved with the comments=&quot;some&quot; option (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1153">#1153</a>)</li>
</ul>
<h2>v5.11.0</h2>
<ul>
<li>Unicode code point escapes (<code>\u{abcde}</code>) are not emitted inside RegExp literals anymore (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1147">#1147</a>)</li>
<li>acorn is now a regular dependency</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/terser/terser/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=terser&package-manager=npm_and_yarn&previous-version=5.10.0&new-version=5.14.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-operations-console/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-20 07:55:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/264" class=".btn">#264</a>
            </td>
            <td>
                <b>
                    Filter orderer msps
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
- fix orderer msp drop down options, removes msps that do not have a known orderer
- fixes update channel flow when system channel less orderer is used, prevents genesis block creation step from appearing


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-19 21:04:09 +0000 UTC
    </div>
</div>

