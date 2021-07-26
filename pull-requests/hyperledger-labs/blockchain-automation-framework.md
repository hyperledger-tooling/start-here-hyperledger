---
layout: default
title: blockchain-automation-framework
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-automation-framework
---

# blockchain-automation-framework <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-automation-framework){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1583" class=".btn">#1583</a>
            </td>
            <td>
                <b>
                    [shared] removed need to have network.yaml in build folder for validation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: suvajit-sarkar <suvajit.sarkar@accenture.com>

**Changelog**
- Add quorum and besu in the validation network.type enum
- Fix need to have network.yaml in build folder for validation 

 

**Reviewed by**
@jagpreetsinghsasan 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-26 06:33:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1582" class=".btn">#1582</a>
            </td>
            <td>
                <b>
                    Create settings.yml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This will set the default branch to main.

Signed-off-by: Ry Jones <ry@linux.com>

**Changelog**
- Update
This will change the default branch to main.
 

**Reviewed by**
@developer_github_id


**Linked issue**
#issue_number

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-23 18:02:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1580" class=".btn">#1580</a>
            </td>
            <td>
                <b>
                    [quorum] Separete quorum node and tessera deployment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: mgCepeda <marina.gomez.cepeda@accenture.com>

**Changelog**
- Add quorum node
- Update tessera node

 

**Reviewed by**
@suvajit-sarkar
@alvaropicazo

 

**Linked issue**
#1556 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-20 13:35:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1579" class=".btn">#1579</a>
            </td>
            <td>
                <b>
                    [quorum] moved tessera crypto creation to k8s job
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: suvajit-sarkar <suvajit.sarkar@accenture.com>

**Changelog**
- Fix molecule test
- Moved crypto creation to k8s job

 

**Reviewed by**
@jagpreetsinghsasan  @mgCepeda 

 

**Linked issue**
#1557 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-20 07:58:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1578" class=".btn">#1578</a>
            </td>
            <td>
                <b>
                    Bump urijs from 1.19.6 to 1.19.7 in /examples/supplychain-app/fabric/chaincode_rest_server/rest-server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [urijs](https://github.com/medialize/URI.js) from 1.19.6 to 1.19.7.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/medialize/URI.js/releases">urijs's releases</a>.</em></p>
<blockquote>
<h2>1.19.7 (July 14th 2021)</h2>
<ul>
<li><strong>SECURITY</strong> fixing <a href="http://medialize.github.io/URI.js/docs.html#static-parseQuery"><code>URI.parseQuery()</code></a> to prevent overwriting <code>__proto__</code> in parseQuery() - disclosed privately by <a href="https://github.com/NewEraCracker"><code>@​NewEraCracker</code></a></li>
<li><strong>SECURITY</strong> fixing <a href="http://medialize.github.io/URI.js/docs.html#static-parse"><code>URI.parse()</code></a> to handle variable amounts of <code>\</code> and <code>/</code> in scheme delimiter as Node and Browsers do - disclosed privately by <a href="https://github.com/ready-research">ready-research</a> via <a href="https://huntr.dev/">https://huntr.dev/</a></li>
<li>removed obsolete build tools</li>
<li>updated jQuery versions (verifying compatibility with 1.12.4, 2.2.4, 3.6.0)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/medialize/URI.js/blob/gh-pages/CHANGELOG.md">urijs's changelog</a>.</em></p>
<blockquote>
<h3>1.19.7 (July 14th 2021)</h3>
<ul>
<li><strong>SECURITY</strong> fixing <a href="http://medialize.github.io/URI.js/docs.html#static-parseQuery"><code>URI.parseQuery()</code></a> to prevent overwriting <code>__proto__</code> in parseQuery() - disclosed privately by <a href="https://github.com/NewEraCracker"><code>@​NewEraCracker</code></a></li>
<li><strong>SECURITY</strong> fixing <a href="http://medialize.github.io/URI.js/docs.html#static-parse"><code>URI.parse()</code></a> to handle variable amounts of <code>\</code> and <code>/</code> in scheme delimiter as Node and Browsers do - disclosed privately by <a href="https://github.com/ready-research">ready-research</a> via <a href="https://huntr.dev/">https://huntr.dev/</a></li>
<li>removed obsolete build tools</li>
<li>updated jQuery versions (verifying compatibility with 1.12.4, 2.2.4, 3.6.0)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/medialize/URI.js/commit/19e54c78d5864aec43986e8f96be8d15998daa80"><code>19e54c7</code></a> chore(build): bumping to version 1.19.7</li>
<li><a href="https://github.com/medialize/URI.js/commit/547d4b69d45d435eed88b04ec0a74cc8080c8694"><code>547d4b6</code></a> build: update jquery</li>
<li><a href="https://github.com/medialize/URI.js/commit/aab4a43e0c0cab5bde140edcb73d29f77365ad02"><code>aab4a43</code></a> build: remove obsolete build tools</li>
<li><a href="https://github.com/medialize/URI.js/commit/ac43ca8f80c042f0256fb551ea5203863dec4481"><code>ac43ca8</code></a> fix(parse): more backslash galore <a href="https://github-redirect.dependabot.com/medialize/URI.js/issues/410">#410</a></li>
<li><a href="https://github.com/medialize/URI.js/commit/622db6d8d6e650d6de4300c97779de50e3331095"><code>622db6d</code></a> docs: add security policy</li>
<li><a href="https://github.com/medialize/URI.js/commit/8e51b00911ba0f6e90949e2c4516b945c35021f7"><code>8e51b00</code></a> fix(parse): prevent overwriting <strong>proto</strong> in parseQuery()</li>
<li>See full diff in <a href="https://github.com/medialize/URI.js/compare/v1.19.6...v1.19.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=urijs&package-manager=npm_and_yarn&previous-version=1.19.6&new-version=1.19.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-automation-framework/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-20 05:49:30 +0000 UTC
    </div>
</div>

