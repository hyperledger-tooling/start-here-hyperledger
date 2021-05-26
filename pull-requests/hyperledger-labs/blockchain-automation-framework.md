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
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1497" class=".btn">#1497</a>
            </td>
            <td>
                <b>
                    [shared] removing repetition in github actions molecule tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**
- Updated molecule github actions by removing repetition

 

**Reviewed by**
@suvajit-sarkar 

 

**Linked issue**
#issue_number

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-26 08:46:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1496" class=".btn">#1496</a>
            </td>
            <td>
                <b>
                    [corda] implemented new test for reset-network roles
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: mgCepeda <marina.gomez.cepeda@accenture.com>

**Changelog**
- Add new test for reset-network roles
- Fixed task using molecule-idempotence-notest tag to be able to run the implemented test




 

**Reviewed by**
@suvajit-sarkar
@alvaropicazo 

 

**Linked issue**
#628 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-25 15:42:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1493" class=".btn">#1493</a>
            </td>
            <td>
                <b>
                    [besu] Updated besu and orion version in samples and docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: alvaropicazo <alvaro.picazo.haase@accenture.com>

Deployed 21.1.1 Besu version using latest Orion version (21.1.0) and also 1.6.0.

**Changelog**
- Updated orion and besu versions in samples and docs

 

**Reviewed by**
@suvajit-sarkar 

 

**Linked issue**
#1452 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-24 11:17:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1492" class=".btn">#1492</a>
            </td>
            <td>
                <b>
                    [corda-ent] Upgrade CENM version to 1.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: suvajit-sarkar <suvajit.sarkar@accenture.com>

**Changelog**
- Add 1.5 CENM images
- Fix base directory hard coding in charts
- Update code to support CENM upgrade

 

**Reviewed by**
@pppazos 

 

**Linked issue**
#1289 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-24 10:49:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1490" class=".btn">#1490</a>
            </td>
            <td>
                <b>
                    [docs] latest master changes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**
- Add
- Fix
- Update

 

**Reviewed by**
@developer_github_id

 

**Linked issue**
#issue_number

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-21 16:39:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1489" class=".btn">#1489</a>
            </td>
            <td>
                <b>
                    Develop to master
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**
- Add
- Fix
- Update

 

**Reviewed by**
@developer_github_id

 

**Linked issue**
#issue_number

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-21 16:30:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1488" class=".btn">#1488</a>
            </td>
            <td>
                <b>
                    Bump react-dom from 16.4.1 to 16.4.2 in /platforms/r3-corda/images/networkmap/website
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [react-dom](https://github.com/facebook/react/tree/HEAD/packages/react-dom) from 16.4.1 to 16.4.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/facebook/react/releases">react-dom's releases</a>.</em></p>
<blockquote>
<h2>v16.4.2</h2>
<h2>16.4.2 (August 1, 2018)</h2>
<h3>React DOM Server</h3>
<ul>
<li>
<p>Fix a <a href="https://reactjs.org/blog/2018/08/01/react-v-16-4-2.html">potential XSS vulnerability when the attacker controls an attribute name</a> (<code>CVE-2018-6341</code>). This fix is available in the latest <code>react-dom@16.4.2</code>, as well as in previous affected minor versions: <code>react-dom@16.0.1</code>, <code>react-dom@16.1.2</code>, <code>react-dom@16.2.1</code>, and <code>react-dom@16.3.3</code>. (<a href="https://github.com/gaearon"><code>@​gaearon</code></a> in <a href="https://github-redirect.dependabot.com/facebook/react/pull/13302">#13302</a>)</p>
</li>
<li>
<p>Fix a crash in the server renderer when an attribute is called <code>hasOwnProperty</code>. This fix is only available in <code>react-dom@16.4.2</code>. (<a href="https://github.com/gaearon"><code>@​gaearon</code></a> in <a href="https://github-redirect.dependabot.com/facebook/react/pull/13303">#13303</a>)</p>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/facebook/react/blob/master/CHANGELOG.md">react-dom's changelog</a>.</em></p>
<blockquote>
<h2>16.4.2 (August 1, 2018)</h2>
<h3>React DOM Server</h3>
<ul>
<li>
<p>Fix a <a href="https://reactjs.org/blog/2018/08/01/react-v-16-4-2.html">potential XSS vulnerability when the attacker controls an attribute name</a> (<code>CVE-2018-6341</code>). This fix is available in the latest <code>react-dom@16.4.2</code>, as well as in previous affected minor versions: <code>react-dom@16.0.1</code>, <code>react-dom@16.1.2</code>, <code>react-dom@16.2.1</code>, and <code>react-dom@16.3.3</code>. (<a href="https://github.com/gaearon"><code>@​gaearon</code></a> in <a href="https://github-redirect.dependabot.com/facebook/react/pull/13302">#13302</a>)</p>
</li>
<li>
<p>Fix a crash in the server renderer when an attribute is called <code>hasOwnProperty</code>. This fix is only available in <code>react-dom@16.4.2</code>. (<a href="https://github.com/gaearon"><code>@​gaearon</code></a> in <a href="https://github-redirect.dependabot.com/facebook/react/pull/13303">#13303</a>)</p>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/facebook/react/commit/54adb2674afe16ec603e0c54bf46ccf1afa42308"><code>54adb26</code></a> 16.4.2</li>
<li><a href="https://github.com/facebook/react/commit/d922ed2cf2fadf2578a1379be3bb89430e7ceb0c"><code>d922ed2</code></a> Fix SSR crash on a hasOwnProperty attribute</li>
<li><a href="https://github.com/facebook/react/commit/5b19684fc3eddb44a790f31804707de9234147c7"><code>5b19684</code></a> Sanitize unknown attribute names for SSR</li>
<li>See full diff in <a href="https://github.com/facebook/react/commits/v16.4.2/packages/react-dom">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=react-dom&package-manager=npm_and_yarn&previous-version=16.4.1&new-version=16.4.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-05-21 16:13:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1487" class=".btn">#1487</a>
            </td>
            <td>
                <b>
                    Bump junit from 4.12 to 4.13.1 in /platforms/r3-corda/images/networkmap
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">java</span>
            </td>
            <td>
                Bumps [junit](https://github.com/junit-team/junit4) from 4.12 to 4.13.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/junit-team/junit4/releases">junit's releases</a>.</em></p>
<blockquote>
<h2>JUnit 4.13.1</h2>
<p>Please refer to the <a href="https://github.com/junit-team/junit/blob/HEAD/doc/ReleaseNotes4.13.1.md">release notes</a> for details.</p>
<h2>JUnit 4.13</h2>
<p>Please refer to the <a href="https://github.com/junit-team/junit/blob/HEAD/doc/ReleaseNotes4.13.md">release notes</a> for details.</p>
<h2>JUnit 4.13 RC 2</h2>
<p>Please refer to the <a href="https://github.com/junit-team/junit4/wiki/4.13-Release-Notes">release notes</a> for details.</p>
<h2>JUnit 4.13 RC 1</h2>
<p>Please refer to the <a href="https://github.com/junit-team/junit4/wiki/4.13-Release-Notes">release notes</a> for details.</p>
<h2>JUnit 4.13 Beta 3</h2>
<p>Please refer to the <a href="https://github.com/junit-team/junit4/wiki/4.13-Release-Notes">release notes</a> for details.</p>
<h2>JUnit 4.13 Beta 2</h2>
<p>Please refer to the <a href="https://github.com/junit-team/junit4/wiki/4.13-Release-Notes">release notes</a> for details.</p>
<h2>JUnit 4.13 Beta 1</h2>
<p>Please refer to the <a href="https://github.com/junit-team/junit4/wiki/4.13-Release-Notes">release notes</a> for details.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/junit-team/junit4/commit/1b683f4ec07bcfa40149f086d32240f805487e66"><code>1b683f4</code></a> [maven-release-plugin] prepare release r4.13.1</li>
<li><a href="https://github.com/junit-team/junit4/commit/ce6ce3aadc070db2902698fe0d3dc6729cd631f2"><code>ce6ce3a</code></a> Draft 4.13.1 release notes</li>
<li><a href="https://github.com/junit-team/junit4/commit/c29dd8239d6b353e699397eb090a1fd27411fa24"><code>c29dd82</code></a> Change version to 4.13.1-SNAPSHOT</li>
<li><a href="https://github.com/junit-team/junit4/commit/1d174861f0b64f97ab0722bb324a760bfb02f567"><code>1d17486</code></a> Add a link to assertThrows in exception testing</li>
<li><a href="https://github.com/junit-team/junit4/commit/543905df72ff10364b94dda27552efebf3dd04e9"><code>543905d</code></a> Use separate line for annotation in Javadoc</li>
<li><a href="https://github.com/junit-team/junit4/commit/510e906b391e7e46a346e1c852416dc7be934944"><code>510e906</code></a> Add sub headlines to class Javadoc</li>
<li><a href="https://github.com/junit-team/junit4/commit/610155b8c22138329f0723eec22521627dbc52ae"><code>610155b</code></a> Merge pull request from GHSA-269g-pwp5-87pp</li>
<li><a href="https://github.com/junit-team/junit4/commit/b6cfd1e3d736cc2106242a8be799615b472c7fec"><code>b6cfd1e</code></a> Explicitly wrap float parameter for consistency (<a href="https://github-redirect.dependabot.com/junit-team/junit4/issues/1671">#1671</a>)</li>
<li><a href="https://github.com/junit-team/junit4/commit/a5d205c7956dbed302b3bb5ecde5ba4299f0b646"><code>a5d205c</code></a> Fix GitHub link in FAQ (<a href="https://github-redirect.dependabot.com/junit-team/junit4/issues/1672">#1672</a>)</li>
<li><a href="https://github.com/junit-team/junit4/commit/3a5c6b4d08f408c8ca6a8e0bae71a9bc5a8f97e8"><code>3a5c6b4</code></a> Deprecated since jdk9 replacing constructor instance of Double and Float (<a href="https://github-redirect.dependabot.com/junit-team/junit4/issues/1660">#1660</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/junit-team/junit4/compare/r4.12...r4.13.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=junit:junit&package-manager=maven&previous-version=4.12&new-version=4.13.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-05-21 16:11:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1486" class=".btn">#1486</a>
            </td>
            <td>
                <b>
                    [shared] update PR workflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Roy,Sownak <sownak.roy@accenture.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-21 15:55:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1485" class=".btn">#1485</a>
            </td>
            <td>
                <b>
                    [shared] updated gitactions flow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**
- Add
- Fix
- Update

 

**Reviewed by**
@developer_github_id

 

**Linked issue**
#issue_number

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-21 15:33:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1484" class=".btn">#1484</a>
            </td>
            <td>
                <b>
                    Bump ini from 1.3.5 to 1.3.8 in /platforms/r3-corda/images/networkmap/website
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [ini](https://github.com/isaacs/ini) from 1.3.5 to 1.3.8.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/npm/ini/commit/a2c5da86604bc2238fe393c5ff083bf23a9910eb"><code>a2c5da8</code></a> 1.3.8</li>
<li><a href="https://github.com/npm/ini/commit/af5c6bb5dca6f0248c153aa87e25bddfc515ff6e"><code>af5c6bb</code></a> Do not use Object.create(null)</li>
<li><a href="https://github.com/npm/ini/commit/8b648a1ac49e1b3b7686ea957e0b95e544bc6ec1"><code>8b648a1</code></a> don't test where our devdeps don't even work</li>
<li><a href="https://github.com/npm/ini/commit/c74c8af35f32b801a7e82a8309eab792a95932f6"><code>c74c8af</code></a> 1.3.7</li>
<li><a href="https://github.com/npm/ini/commit/024b8b55ac1c980c6225607b007714c54eb501ba"><code>024b8b5</code></a> update deps, add linting</li>
<li><a href="https://github.com/npm/ini/commit/032fbaf5f0b98fce70c8cc380e0d05177a9c9073"><code>032fbaf</code></a> Use Object.create(null) to avoid default object property hazards</li>
<li><a href="https://github.com/npm/ini/commit/2da90391ef70db41d10f013e3a87f9a8c5d01a72"><code>2da9039</code></a> 1.3.6</li>
<li><a href="https://github.com/npm/ini/commit/cfea636f534b5ca7550d2c28b7d1a95d936d56c6"><code>cfea636</code></a> better git push script, before publish instead of after</li>
<li><a href="https://github.com/npm/ini/commit/56d2805e07ccd94e2ba0984ac9240ff02d44b6f1"><code>56d2805</code></a> do not allow invalid hazardous string as section name</li>
<li>See full diff in <a href="https://github.com/isaacs/ini/compare/v1.3.5...v1.3.8">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~isaacs">isaacs</a>, a new releaser for ini since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ini&package-manager=npm_and_yarn&previous-version=1.3.5&new-version=1.3.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-05-21 15:28:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1482" class=".btn">#1482</a>
            </td>
            <td>
                <b>
                    Bump elliptic from 6.5.1 to 6.5.4 in /platforms/r3-corda/images/networkmap/website
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [elliptic](https://github.com/indutny/elliptic) from 6.5.1 to 6.5.4.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/indutny/elliptic/commit/43ac7f230069bd1575e1e4a58394a512303ba803"><code>43ac7f2</code></a> 6.5.4</li>
<li><a href="https://github.com/indutny/elliptic/commit/f4bc72be11b0a508fb790f445c43534307c9255b"><code>f4bc72b</code></a> package: bump deps</li>
<li><a href="https://github.com/indutny/elliptic/commit/441b7428b0e8f6636c42118ad2aaa186d3c34c3f"><code>441b742</code></a> ec: validate that a point before deriving keys</li>
<li><a href="https://github.com/indutny/elliptic/commit/e71b2d9359c5fe9437fbf46f1f05096de447de57"><code>e71b2d9</code></a> lib: relint using eslint</li>
<li><a href="https://github.com/indutny/elliptic/commit/8421a01aa3ff789c79f91eaf8845558a7be2b9fa"><code>8421a01</code></a> build(deps): bump elliptic from 6.4.1 to 6.5.3 (<a href="https://github-redirect.dependabot.com/indutny/elliptic/issues/231">#231</a>)</li>
<li><a href="https://github.com/indutny/elliptic/commit/8647803dc3d90506aa03021737f7b061ba959ae1"><code>8647803</code></a> 6.5.3</li>
<li><a href="https://github.com/indutny/elliptic/commit/856fe4d99fe7b6200556e6400b3bf585b1721bec"><code>856fe4d</code></a> signature: prevent malleability and overflows</li>
<li><a href="https://github.com/indutny/elliptic/commit/60489415e545efdfd3010ae74b9726facbf08ca8"><code>6048941</code></a> 6.5.2</li>
<li><a href="https://github.com/indutny/elliptic/commit/9984964457c9f8a63b91b01ea103260417eca237"><code>9984964</code></a> package: bump dependencies</li>
<li><a href="https://github.com/indutny/elliptic/commit/ec735edde187a43693197f6fa3667ceade751a3a"><code>ec735ed</code></a> utils: leak less information in <code>getNAF()</code></li>
<li>See full diff in <a href="https://github.com/indutny/elliptic/compare/v6.5.1...v6.5.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=elliptic&package-manager=npm_and_yarn&previous-version=6.5.1&new-version=6.5.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-05-21 15:28:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1481" class=".btn">#1481</a>
            </td>
            <td>
                <b>
                    Bump pug from 2.0.3 to 3.0.1 in /platforms/r3-corda/images/networkmap/website
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [pug](https://github.com/pugjs/pug) from 2.0.3 to 3.0.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pugjs/pug/releases">pug's releases</a>.</em></p>
<blockquote>
<h2>pug-code-gen@3.0.1</h2>
<h2>Bug Fixes</h2>
<ul>
<li>Update <code>with</code> to resolve core-js deprecation notice (<a href="https://github-redirect.dependabot.com/pugjs/pug/issues/3259">#3259</a>)</li>
</ul>
<h2>pug@3.0.1</h2>
<h2>Bug Fixes</h2>
<ul>
<li>
<p>Sanitise the <code>pretty</code> option (<a href="https://github-redirect.dependabot.com/pugjs/pug/issues/3314">#3314</a>)</p>
<p>If a malicious attacker could control the <code>pretty</code> option, it was possible for them to achieve remote code execution on the server rendering the template. All pug users should upgrade as soon as possible, see <a href="https://github-redirect.dependabot.com/pugjs/pug/issues/3312">#3312</a> for more details.</p>
</li>
</ul>
<h2>pug-runtime@3.0.1</h2>
<h2>Bug Fixes</h2>
<ul>
<li>Properly handle non-string values when rethrowing errors (<a href="https://github-redirect.dependabot.com/pugjs/pug/issues/3269">#3269</a>)</li>
</ul>
<h2>pug-runtime@3.0.0</h2>
<h2>Breaking Changes</h2>
<ul>
<li>Drop support for node 6 and 8 (<a href="https://github-redirect.dependabot.com/pugjs/pug/issues/3243">#3243</a>)</li>
</ul>
<h2>Bug Fixes</h2>
<ul>
<li>wrap setting err.message with a try/catch (<a href="https://github-redirect.dependabot.com/pugjs/pug/issues/2996">#2996</a>)</li>
</ul>
<h2>pug-attrs@3.0.0</h2>
<h2>Breaking Changes</h2>
<ul>
<li>Drop support for node 6 and 8 (<a href="https://github-redirect.dependabot.com/pugjs/pug/issues/3243">#3243</a>)</li>
</ul>
<h2>pug-code-gen@3.0.0</h2>
<h2>Breaking Changes</h2>
<ul>
<li>Drop support for node 6 and 8 (<a href="https://github-redirect.dependabot.com/pugjs/pug/issues/3243">#3243</a>)</li>
</ul>
<h2>New Features</h2>
<ul>
<li>Support <code>EachOf</code> nodes (<a href="https://github-redirect.dependabot.com/pugjs/pug/issues/3179">#3179</a>)</li>
</ul>
<h2>pug-load@3.0.0</h2>
<h2>Breaking Changes</h2>
<ul>
<li>
<p><code>read</code> plugins must now return <code>Buffer</code> if you want to support filters that use <code>renderBuffer</code> (<a href="https://github-redirect.dependabot.com/pugjs/pug/issues/3213">#3213</a>)</p>
</li>
<li>
<p>Drop support for node 6 and 8 (<a href="https://github-redirect.dependabot.com/pugjs/pug/issues/3243">#3243</a>)</p>
</li>
</ul>
<h2>New Features</h2>
<ul>
<li>File nodes now get a <code>raw</code> property that is a <code>Buffer</code>, in addition to the <code>str</code> (<a href="https://github-redirect.dependabot.com/pugjs/pug/issues/3213">#3213</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pugjs/pug/commit/991e78f7c4220b2f8da042877c6f0ef5a4683be0"><code>991e78f</code></a> fix: sanitise and escape the <code>pretty</code> option (<a href="https://github-redirect.dependabot.com/pugjs/pug/issues/3314">#3314</a>)</li>
<li><a href="https://github.com/pugjs/pug/commit/06baa525a23049756de9587461d389a12bc12537"><code>06baa52</code></a> Fix TypeScript and add eachOf token definition (<a href="https://github-redirect.dependabot.com/pugjs/pug/issues/3262">#3262</a>)</li>
<li><a href="https://github.com/pugjs/pug/commit/13e46e9fe87220530a066d3aae49131969920275"><code>13e46e9</code></a> chore: update with (<a href="https://github-redirect.dependabot.com/pugjs/pug/issues/3259">#3259</a>)</li>
<li><a href="https://github.com/pugjs/pug/commit/c077df4a8d523fe42e52f83b62d3c8ba3822d3b3"><code>c077df4</code></a> docs: fix rolling versions link</li>
<li><a href="https://github.com/pugjs/pug/commit/ccba7dae678b1fceaa9b46d9d15a78ee0a2569d4"><code>ccba7da</code></a> ci: publish canary release (<a href="https://github-redirect.dependabot.com/pugjs/pug/issues/3257">#3257</a>)</li>
<li><a href="https://github.com/pugjs/pug/commit/24a7b8eaaf86e53d0581c9e7900fb8fa906c5b2a"><code>24a7b8e</code></a> chore: remove get-repo dependency (<a href="https://github-redirect.dependabot.com/pugjs/pug/issues/3256">#3256</a>)</li>
<li><a href="https://github.com/pugjs/pug/commit/8288ec5fa9b28781be78ea4508b3f8c9ca7f9ba1"><code>8288ec5</code></a> ci: fix some problems with the workflows and add dry-run (<a href="https://github-redirect.dependabot.com/pugjs/pug/issues/3254">#3254</a>)</li>
<li><a href="https://github.com/pugjs/pug/commit/eca9342bf3046e5170301d8839df551c1fe35d99"><code>eca9342</code></a> chore: update is-expression and jest (<a href="https://github-redirect.dependabot.com/pugjs/pug/issues/3253">#3253</a>)</li>
<li><a href="https://github.com/pugjs/pug/commit/9e96bb722c706a2fc89bce401e4ba215205bd9b1"><code>9e96bb7</code></a> feat: allow filters to read non-text include files (<a href="https://github-redirect.dependabot.com/pugjs/pug/issues/3213">#3213</a>)</li>
<li><a href="https://github.com/pugjs/pug/commit/bb0731f75813aa30d8e077808b5465a67ef284ef"><code>bb0731f</code></a> chore: use minimal settings to format test files (<a href="https://github-redirect.dependabot.com/pugjs/pug/issues/3245">#3245</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/pugjs/pug/compare/pug@2.0.3...pug@3.0.1">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~pug-bot">pug-bot</a>, a new releaser for pug since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pug&package-manager=npm_and_yarn&previous-version=2.0.3&new-version=3.0.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-05-21 15:28:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1480" class=".btn">#1480</a>
            </td>
            <td>
                <b>
                    Bump highlight.js from 9.12.0 to 10.4.1 in /platforms/r3-corda/images/networkmap/website
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [highlight.js](https://github.com/highlightjs/highlight.js) from 9.12.0 to 10.4.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/highlightjs/highlight.js/releases">highlight.js's releases</a>.</em></p>
<blockquote>
<h2>10.4.1</h2>
<p>Security fixes:</p>
<ul>
<li>(fix) Exponential backtracking fixes for: <a href="https://github.com/joshgoebel">Josh Goebel</a>
<ul>
<li>cpp</li>
<li>handlebars</li>
<li>gams</li>
<li>perl</li>
<li>jboss-cli</li>
<li>r</li>
<li>erlang-repl</li>
<li>powershell</li>
<li>routeros</li>
</ul>
</li>
<li>(fix) Polynomial backtracking fixes for: <a href="https://github.com/joshgoebel">Josh Goebel</a>
<ul>
<li>asciidoc</li>
<li>reasonml</li>
<li>latex</li>
<li>kotlin</li>
<li>gcode</li>
<li>d</li>
<li>aspectj</li>
<li>moonscript</li>
<li>coffeescript/livescript</li>
<li>csharp</li>
<li>scilab</li>
<li>crystal</li>
<li>elixir</li>
<li>basic</li>
<li>ebnf</li>
<li>ruby</li>
<li>fortran/irpf90</li>
<li>livecodeserver</li>
<li>yaml</li>
<li>x86asm</li>
<li>dsconfig</li>
<li>markdown</li>
<li>ruleslanguage</li>
<li>xquery</li>
<li>sqf</li>
</ul>
</li>
</ul>
<p>Very grateful to <a href="https://github.com/RunDevelopment">Michael Schmidt</a> for all the help.</p>
<h2>10.4.0 - November 2020</h2>
<p>A largish release with many improvements and fixes from quite a few different contributors.  Enjoy!</p>
<p>Deprecations:</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/highlightjs/highlight.js/blob/main/CHANGES.md">highlight.js's changelog</a>.</em></p>
<blockquote>
<h2>Version 10.4.1 (tentative)</h2>
<p>Security</p>
<ul>
<li>(fix) Exponential backtracking fixes for: <a href="https://github.com/joshgoebel">Josh Goebel</a>
<ul>
<li>cpp</li>
<li>handlebars</li>
<li>gams</li>
<li>perl</li>
<li>jboss-cli</li>
<li>r</li>
<li>erlang-repl</li>
<li>powershell</li>
<li>routeros</li>
</ul>
</li>
<li>(fix) Polynomial backtracking fixes for: <a href="https://github.com/joshgoebel">Josh Goebel</a>
<ul>
<li>asciidoc</li>
<li>reasonml</li>
<li>latex</li>
<li>kotlin</li>
<li>gcode</li>
<li>d</li>
<li>aspectj</li>
<li>moonscript</li>
<li>coffeescript/livescript</li>
<li>csharp</li>
<li>scilab</li>
<li>crystal</li>
<li>elixir</li>
<li>basic</li>
<li>ebnf</li>
<li>ruby</li>
<li>fortran/irpf90</li>
<li>livecodeserver</li>
<li>yaml</li>
<li>x86asm</li>
<li>dsconfig</li>
<li>markdown</li>
<li>ruleslanguage</li>
<li>xquery</li>
<li>sqf</li>
</ul>
</li>
</ul>
<p>Very grateful to <a href="https://github.com/RunDevelopment">Michael Schmidt</a> for all the help.</p>
<h2>Version 10.4.0</h2>
<p>A largish release with many improvements and fixes from quite a few different contributors.  Enjoy!</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/highlightjs/highlight.js/commit/e96b915af70d1c3f014b732c10e7cd077f22b9c3"><code>e96b915</code></a> bump 10.4.1</li>
<li><a href="https://github.com/highlightjs/highlight.js/commit/065f65f41e803ef80a334f7d30da30e7bc653801"><code>065f65f</code></a> chore(release) allow release script to handle production releases</li>
<li><a href="https://github.com/highlightjs/highlight.js/commit/68509fc6301f5bb504d33766c45dd64253512e4b"><code>68509fc</code></a> chore(docs) bump SECURITY mention to 9.18.5</li>
<li><a href="https://github.com/highlightjs/highlight.js/commit/aa0fb850c24e94081bc65687010d41e1b7dda28a"><code>aa0fb85</code></a> chore(docs) Version 9 has reached EOL.</li>
<li><a href="https://github.com/highlightjs/highlight.js/commit/fb0a62650c39bc6b9c9365657ce4f912d50523fc"><code>fb0a626</code></a> enh(ci): Add tests for polynomial regex issues</li>
<li><a href="https://github.com/highlightjs/highlight.js/commit/fa46dd181d3fc37d43847aa253176c88d3d1e640"><code>fa46dd1</code></a> fix(reasonml) fix poly backtracking issue</li>
<li><a href="https://github.com/highlightjs/highlight.js/commit/d496052534bb4317373991098d15ddd5ccb8f566"><code>d496052</code></a> fix(latex) fix poly backtracking issue</li>
<li><a href="https://github.com/highlightjs/highlight.js/commit/d9f1cdb9924a1f22fc145711a499962a76477ac7"><code>d9f1cdb</code></a> fix(javascript/typescript) fix poly backtracking issue</li>
<li><a href="https://github.com/highlightjs/highlight.js/commit/fdec037a569c9f06592dd17304b07640365573b7"><code>fdec037</code></a> fix(asciidoc) fix poly backtracking issue</li>
<li><a href="https://github.com/highlightjs/highlight.js/commit/02ca487e8ca4d56f2cbd1b738eae8f814688b5eb"><code>02ca487</code></a> fix(kotlin) fix poly backtracking issue</li>
<li>Additional commits viewable in <a href="https://github.com/highlightjs/highlight.js/compare/9.12.0...10.4.1">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~joshgoebel">joshgoebel</a>, a new releaser for highlight.js since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=highlight.js&package-manager=npm_and_yarn&previous-version=9.12.0&new-version=10.4.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-05-21 15:28:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1479" class=".btn">#1479</a>
            </td>
            <td>
                <b>
                    end of sprint merge
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Roy,Sownak <sownak.roy@accenture.com>

**Changelog**
- Add
- Fix
- Update

 

**Reviewed by**
@developer_github_id

 

**Linked issue**
#issue_number

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-21 15:21:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1478" class=".btn">#1478</a>
            </td>
            <td>
                <b>
                    develop to master merge
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                End of sprint merge

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-21 15:11:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1477" class=".btn">#1477</a>
            </td>
            <td>
                <b>
                    Develop
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**
- Add
- Fix
- Update

 

**Reviewed by**
@developer_github_id

 

**Linked issue**
#issue_number

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-21 14:37:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1474" class=".btn">#1474</a>
            </td>
            <td>
                <b>
                    [indy] Add Org refactor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Roy,Sownak <sownak.roy@accenture.com>

**Changelog**
- Fix existing Add Org for Indy
- Update Vault default version to 1.7.0
 

**Linked issue**
Resolves #1291 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 16:12:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1473" class=".btn">#1473</a>
            </td>
            <td>
                <b>
                    added all changes made to changes to github workflows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Angela Alagbe <angela.alagbe@accenture.com>

**Changelog**
- Added changes to github workflows

 

**Reviewed by**
@suvajit-sarkar @sownak 

 

**Linked issue**
#722 (and all prev issues I've worked on)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 16:08:27 +0000 UTC
    </div>
</div>

