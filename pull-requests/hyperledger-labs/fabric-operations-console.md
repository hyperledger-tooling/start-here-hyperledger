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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/159" class=".btn">#159</a>
            </td>
            <td>
                <b>
                    fix bulk import
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Varad Ramamoorthy <varad@us.ibm.com>


- Bug fix

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-04 17:56:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/158" class=".btn">#158</a>
            </td>
            <td>
                <b>
                    Maintenance mode for system channel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- New feature

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-04 17:19:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/157" class=".btn">#157</a>
            </td>
            <td>
                <b>
                    Stitch policy fixes
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
- fix MSP Role formatting in a chaincode definition, was always being set to `MEMBER`
- remove an empty `endorsementPolicy` if a endorsment policy was not set in a Static Collection Config


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-04 14:48:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/156" class=".btn">#156</a>
            </td>
            <td>
                <b>
                    apply multipart bodyParser to the proxy route only
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
<!--- Describe your changes in detail, including motivation. -->

The added body parser is breaking the configtxlator proxy route. This moves that parser from the global scope to just the generic proxy route.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-04 01:53:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/155" class=".btn">#155</a>
            </td>
            <td>
                <b>
                    allow export import admin endpoint from UI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Varad Ramamoorthy <varad@us.ibm.com>

#### Type of change
- New feature

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-02 19:28:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/154" class=".btn">#154</a>
            </td>
            <td>
                <b>
                    add osnadmin_url in validator
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
allow setting and editing of `osnadmin_url`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-02 19:21:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/153" class=".btn">#153</a>
            </td>
            <td>
                <b>
                    Unjoin from orderer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- New feature
Unjoin a channel from orderer
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-02 15:03:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/152" class=".btn">#152</a>
            </td>
            <td>
                <b>
                    Bump karma from 6.3.14 to 6.3.16 in /packages/stitch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [karma](https://github.com/karma-runner/karma) from 6.3.14 to 6.3.16.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/karma-runner/karma/releases">karma's releases</a>.</em></p>
<blockquote>
<h2>v6.3.16</h2>
<h2><a href="https://github.com/karma-runner/karma/compare/v6.3.15...v6.3.16">6.3.16</a> (2022-02-10)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>security:</strong> mitigate the &quot;Open Redirect Vulnerability&quot; (<a href="https://github.com/karma-runner/karma/commit/ff7edbb2ffbcdd69761bece86b7dc1ef0740508d">ff7edbb</a>)</li>
</ul>
<h2>v6.3.15</h2>
<h2><a href="https://github.com/karma-runner/karma/compare/v6.3.14...v6.3.15">6.3.15</a> (2022-02-05)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>helper:</strong> make mkdirIfNotExists helper resilient to concurrent calls (<a href="https://github.com/karma-runner/karma/commit/d9dade2f004a340e49c9a633177576200c286404">d9dade2</a>), closes <a href="https://github-redirect.dependabot.com//github-redirect.dependabot.com/karma-runner/karma-coverage/issues/434/issues/issuecomment-1017939333">karma-runner/karma-coverage#434</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/karma-runner/karma/blob/master/CHANGELOG.md">karma's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/karma-runner/karma/compare/v6.3.15...v6.3.16">6.3.16</a> (2022-02-10)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>security:</strong> mitigate the &quot;Open Redirect Vulnerability&quot; (<a href="https://github.com/karma-runner/karma/commit/ff7edbb2ffbcdd69761bece86b7dc1ef0740508d">ff7edbb</a>)</li>
</ul>
<h2><a href="https://github.com/karma-runner/karma/compare/v6.3.14...v6.3.15">6.3.15</a> (2022-02-05)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>helper:</strong> make mkdirIfNotExists helper resilient to concurrent calls (<a href="https://github.com/karma-runner/karma/commit/d9dade2f004a340e49c9a633177576200c286404">d9dade2</a>), closes <a href="https://github-redirect.dependabot.com//github-redirect.dependabot.com/karma-runner/karma-coverage/issues/434/issues/issuecomment-1017939333">karma-runner/karma-coverage#434</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/karma-runner/karma/commit/ab4b32898bcb4e0ba3a1e99835d30c113db3eeeb"><code>ab4b328</code></a> chore(release): 6.3.16 [skip ci]</li>
<li><a href="https://github.com/karma-runner/karma/commit/ff7edbb2ffbcdd69761bece86b7dc1ef0740508d"><code>ff7edbb</code></a> fix(security): mitigate the &quot;Open Redirect Vulnerability&quot;</li>
<li><a href="https://github.com/karma-runner/karma/commit/c1befa04b32b90f088fefdc0521c6f48cbc510a9"><code>c1befa0</code></a> chore(release): 6.3.15 [skip ci]</li>
<li><a href="https://github.com/karma-runner/karma/commit/d9dade2f004a340e49c9a633177576200c286404"><code>d9dade2</code></a> fix(helper): make mkdirIfNotExists helper resilient to concurrent calls</li>
<li><a href="https://github.com/karma-runner/karma/commit/653c762be4fa464fed5bfa306317b84cc5c28a17"><code>653c762</code></a> ci: prevent duplicate CI tasks on creating a PR</li>
<li>See full diff in <a href="https://github.com/karma-runner/karma/compare/v6.3.14...v6.3.16">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=karma&package-manager=npm_and_yarn&previous-version=6.3.14&new-version=6.3.16)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-03-02 13:31:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/151" class=".btn">#151</a>
            </td>
            <td>
                <b>
                    store the osnadmin url
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

- New feature

#### Description
stores the osnadmin url in console's component doc


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-01 02:29:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/150" class=".btn">#150</a>
            </td>
            <td>
                <b>
                    Create channel via osnadmin part
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- New feature

#### Description
First part of create channel via osnadmin.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-01 02:09:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/149" class=".btn">#149</a>
            </td>
            <td>
                <b>
                    update release note
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

- release note fix

#### Description
change version of release


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-28 18:05:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/148" class=".btn">#148</a>
            </td>
            <td>
                <b>
                    make license field compliant
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
- Release Notes

#### Description
The `license` field wasn't an acceptable value, technically. 
Also updated release notes...


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-28 17:48:25 +0000 UTC
    </div>
</div>

