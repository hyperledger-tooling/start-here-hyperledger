---
layout: default
title: blockchain-carbon-accounting
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-carbon-accounting
---

# blockchain-carbon-accounting <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-carbon-accounting){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/216" class=".btn">#216</a>
            </td>
            <td>
                <b>
                    fix(utilityAPI): ./start.sh on local machine
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Pritam Singh <pkspritam16@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-29 19:46:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/215" class=".btn">#215</a>
            </td>
            <td>
                <b>
                    fix(utility_app): start api with docker, fixed swagger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - start utility api using `./start.sh`
- made swagger work

Signed-off-by: Pritam Singh <pkspritam16@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-29 19:10:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/211" class=".btn">#211</a>
            </td>
            <td>
                <b>
                    Integrating automated-test to Github pipeline
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Pihu1998 pranamika.pihu1998@gmail.com

Created .YAML file in /.github/workflows/ directory.

Please suggest changes. Thanks!
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-28 07:57:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/208" class=".btn">#208</a>
            </td>
            <td>
                <b>
                    Adding test for correct year records
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Pihu1998 <pranamika.pihu1998@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-27 16:14:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/207" class=".btn">#207</a>
            </td>
            <td>
                <b>
                    feat(utilityCC): update tokenId of audited Emission tokens in batch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #199 

Signed-off-by: Pritam Singh <pkspritam16@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-25 20:31:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/206" class=".btn">#206</a>
            </td>
            <td>
                <b>
                    bringing mentorship-cactus-integration branch up to date with main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-25 20:13:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/203" class=".btn">#203</a>
            </td>
            <td>
                <b>
                    fix(typescript_app): fixed web3 version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Pritam Singh <pkspritam16@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-25 14:05:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/202" class=".btn">#202</a>
            </td>
            <td>
                <b>
                    Bump color-string from 1.5.4 to 1.5.5 in /utility-emissions-channel/typescript_app
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [color-string](https://github.com/Qix-/color-string) from 1.5.4 to 1.5.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/Qix-/color-string/releases">color-string's releases</a>.</em></p>
<blockquote>
<h2>1.5.5 (Patch/Security Release) - hwb() ReDos patch (low-severity)</h2>
<blockquote>
<p>Release notes copied verbatim from the commit message, which can be found here: 0789e21284c33d89ebc4ab4ca6f759b9375ac9d3</p>
</blockquote>
<pre><code>Discovered by Yeting Li, c/o Colin Ife via Snyk.io.
<p>A ReDos (Regular Expression Denial of Service) vulnerability
was responsibly disclosed to me via email by Colin on
Mar 5 2021 regarding an exponential time complexity for
linearly increasing input lengths for <code>hwb()</code> color strings.</p>
<p>Strings reaching more than 5000 characters would see several
milliseconds of processing time; strings reaching more than
50,000 characters began seeing 1500ms (1.5s) of processing time.</p>
<p>The cause was due to a the regular expression that parses
hwb() strings - specifically, the hue value - where
the integer portion of the hue value used a 0-or-more quantifier
shortly thereafter followed by a 1-or-more quantifier.</p>
<p>This caused excessive backtracking and a cartesian scan,
resulting in exponential time complexity given a linear
increase in input length.</p>
<p>Thank you Yeting Li and Colin Ife for bringing this to my
attention in a secure, responsible and professional manner.</p>
<p>A CVE will not be assigned for this vulnerability.
</code></pre></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/Qix-/color-string/commit/966ae4d80fc8f237674d099ce6214a9fb6a816bb"><code>966ae4d</code></a> 1.5.5</li>
<li><a href="https://github.com/Qix-/color-string/commit/0789e21284c33d89ebc4ab4ca6f759b9375ac9d3"><code>0789e21</code></a> fix ReDos in hwb() parser (low-severity)</li>
<li>See full diff in <a href="https://github.com/Qix-/color-string/compare/1.5.4...1.5.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=color-string&package-manager=npm_and_yarn&previous-version=1.5.4&new-version=1.5.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-23 18:11:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/201" class=".btn">#201</a>
            </td>
            <td>
                <b>
                    Bump color-string from 1.5.4 to 1.5.5 in /utility-emissions-channel/docker-compose-setup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [color-string](https://github.com/Qix-/color-string) from 1.5.4 to 1.5.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/Qix-/color-string/releases">color-string's releases</a>.</em></p>
<blockquote>
<h2>1.5.5 (Patch/Security Release) - hwb() ReDos patch (low-severity)</h2>
<blockquote>
<p>Release notes copied verbatim from the commit message, which can be found here: 0789e21284c33d89ebc4ab4ca6f759b9375ac9d3</p>
</blockquote>
<pre><code>Discovered by Yeting Li, c/o Colin Ife via Snyk.io.
<p>A ReDos (Regular Expression Denial of Service) vulnerability
was responsibly disclosed to me via email by Colin on
Mar 5 2021 regarding an exponential time complexity for
linearly increasing input lengths for <code>hwb()</code> color strings.</p>
<p>Strings reaching more than 5000 characters would see several
milliseconds of processing time; strings reaching more than
50,000 characters began seeing 1500ms (1.5s) of processing time.</p>
<p>The cause was due to a the regular expression that parses
hwb() strings - specifically, the hue value - where
the integer portion of the hue value used a 0-or-more quantifier
shortly thereafter followed by a 1-or-more quantifier.</p>
<p>This caused excessive backtracking and a cartesian scan,
resulting in exponential time complexity given a linear
increase in input length.</p>
<p>Thank you Yeting Li and Colin Ife for bringing this to my
attention in a secure, responsible and professional manner.</p>
<p>A CVE will not be assigned for this vulnerability.
</code></pre></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/Qix-/color-string/commit/966ae4d80fc8f237674d099ce6214a9fb6a816bb"><code>966ae4d</code></a> 1.5.5</li>
<li><a href="https://github.com/Qix-/color-string/commit/0789e21284c33d89ebc4ab4ca6f759b9375ac9d3"><code>0789e21</code></a> fix ReDos in hwb() parser (low-severity)</li>
<li>See full diff in <a href="https://github.com/Qix-/color-string/compare/1.5.4...1.5.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=color-string&package-manager=npm_and_yarn&previous-version=1.5.4&new-version=1.5.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-23 18:11:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/200" class=".btn">#200</a>
            </td>
            <td>
                <b>
                    Fixing NERC 2019 Data Loader 'undefined' bug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Pihu1998 <pranamika.pihu1998@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-23 17:51:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/198" class=".btn">#198</a>
            </td>
            <td>
                <b>
                    puting mentorship-cactus-integration branch up to date with main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-23 15:01:17 +0000 UTC
    </div>
</div>

