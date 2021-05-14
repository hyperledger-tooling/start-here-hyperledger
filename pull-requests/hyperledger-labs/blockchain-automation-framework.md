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
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1461" class=".btn">#1461</a>
            </td>
            <td>
                <b>
                    adding chaincode static tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Dimbu Afonso <dimbu.k.afonso@accenture.com>

**Changelog**
- Adding chaincode static tests

 

**Reviewed by**
@suvajit-sarkar 

 

**Linked issue**
#739 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-11 17:55:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1460" class=".btn">#1460</a>
            </td>
            <td>
                <b>
                    [shared] Use no_ansible_log as variable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Roy,Sownak <sownak.roy@accenture.com>

**Changelog**
- Add ansible logs option

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-11 16:53:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1459" class=".btn">#1459</a>
            </td>
            <td>
                <b>
                    [fabric] Implemented additional annotations for pods
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**
- Added annotations for ca, ca-tools, peernodes and orderernodes.
- Added annotations section for network fabric templates
- Updated charts, helm files for reading those annotations specified in the network.yaml

 

**Reviewed by**
@sownak 

 

**Linked issue**
#1422 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-11 11:18:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1458" class=".btn">#1458</a>
            </td>
            <td>
                <b>
                    Added corda enterprise 4.7 version support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: suvajit-sarkar <suvajit.sarkar@accenture.com>

**Changelog**
- Add 
  - Node 4.7 docker image 
- Changed
  - Node and notary configuration for 4.7
- Fixed
  - jar paths in node and notary charts


 
**Linked issue**
#1267 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-11 09:49:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1457" class=".btn">#1457</a>
            </td>
            <td>
                <b>
                    Bump lodash from 4.17.19 to 4.17.21 in /platforms/r3-corda/images/networkmap/website
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [lodash](https://github.com/lodash/lodash) from 4.17.19 to 4.17.21.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/lodash/lodash/commit/f299b52f39486275a9e6483b60a410e06520c538"><code>f299b52</code></a> Bump to v4.17.21</li>
<li><a href="https://github.com/lodash/lodash/commit/c4847ebe7d14540bb28a8b932a9ce1b9ecbfee1a"><code>c4847eb</code></a> Improve performance of <code>toNumber</code>, <code>trim</code> and <code>trimEnd</code> on large input strings</li>
<li><a href="https://github.com/lodash/lodash/commit/3469357cff396a26c363f8c1b5a91dde28ba4b1c"><code>3469357</code></a> Prevent command injection through <code>_.template</code>'s <code>variable</code> option</li>
<li><a href="https://github.com/lodash/lodash/commit/ded9bc66583ed0b4e3b7dc906206d40757b4a90a"><code>ded9bc6</code></a> Bump to v4.17.20.</li>
<li><a href="https://github.com/lodash/lodash/commit/63150ef7645ac07961b63a86490f419f356429aa"><code>63150ef</code></a> Documentation fixes.</li>
<li><a href="https://github.com/lodash/lodash/commit/00f0f62a979d2f5fa0287c06eae70cf9a62d8794"><code>00f0f62</code></a> test.js: Remove trailing comma.</li>
<li><a href="https://github.com/lodash/lodash/commit/846e434c7a5b5692c55ebf5715ed677b70a32389"><code>846e434</code></a> Temporarily use a custom fork of <code>lodash-cli</code>.</li>
<li><a href="https://github.com/lodash/lodash/commit/5d046f39cbd27f573914768e3b36eeefcc4f1229"><code>5d046f3</code></a> Re-enable Travis tests on <code>4.17</code> branch.</li>
<li><a href="https://github.com/lodash/lodash/commit/aa816b36d402a1ad9385142ce7188f17dae514fd"><code>aa816b3</code></a> Remove <code>/npm-package</code>.</li>
<li>See full diff in <a href="https://github.com/lodash/lodash/compare/4.17.19...4.17.21">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~bnjmnt4n">bnjmnt4n</a>, a new releaser for lodash since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=lodash&package-manager=npm_and_yarn&previous-version=4.17.19&new-version=4.17.21)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-05-11 08:50:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1456" class=".btn">#1456</a>
            </td>
            <td>
                <b>
                    [shared] latest merge master
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
        Created At 2021-05-10 11:44:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1455" class=".btn">#1455</a>
            </td>
            <td>
                <b>
                    Bump lodash from 4.17.19 to 4.17.21 in /examples/supplychain-app/fabric/chaincode_rest_server/rest-server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [lodash](https://github.com/lodash/lodash) from 4.17.19 to 4.17.21.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/lodash/lodash/commit/f299b52f39486275a9e6483b60a410e06520c538"><code>f299b52</code></a> Bump to v4.17.21</li>
<li><a href="https://github.com/lodash/lodash/commit/c4847ebe7d14540bb28a8b932a9ce1b9ecbfee1a"><code>c4847eb</code></a> Improve performance of <code>toNumber</code>, <code>trim</code> and <code>trimEnd</code> on large input strings</li>
<li><a href="https://github.com/lodash/lodash/commit/3469357cff396a26c363f8c1b5a91dde28ba4b1c"><code>3469357</code></a> Prevent command injection through <code>_.template</code>'s <code>variable</code> option</li>
<li><a href="https://github.com/lodash/lodash/commit/ded9bc66583ed0b4e3b7dc906206d40757b4a90a"><code>ded9bc6</code></a> Bump to v4.17.20.</li>
<li><a href="https://github.com/lodash/lodash/commit/63150ef7645ac07961b63a86490f419f356429aa"><code>63150ef</code></a> Documentation fixes.</li>
<li><a href="https://github.com/lodash/lodash/commit/00f0f62a979d2f5fa0287c06eae70cf9a62d8794"><code>00f0f62</code></a> test.js: Remove trailing comma.</li>
<li><a href="https://github.com/lodash/lodash/commit/846e434c7a5b5692c55ebf5715ed677b70a32389"><code>846e434</code></a> Temporarily use a custom fork of <code>lodash-cli</code>.</li>
<li><a href="https://github.com/lodash/lodash/commit/5d046f39cbd27f573914768e3b36eeefcc4f1229"><code>5d046f3</code></a> Re-enable Travis tests on <code>4.17</code> branch.</li>
<li><a href="https://github.com/lodash/lodash/commit/aa816b36d402a1ad9385142ce7188f17dae514fd"><code>aa816b3</code></a> Remove <code>/npm-package</code>.</li>
<li>See full diff in <a href="https://github.com/lodash/lodash/compare/4.17.19...4.17.21">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~bnjmnt4n">bnjmnt4n</a>, a new releaser for lodash since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=lodash&package-manager=npm_and_yarn&previous-version=4.17.19&new-version=4.17.21)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-05-10 11:37:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1454" class=".btn">#1454</a>
            </td>
            <td>
                <b>
                    Bump lodash from 4.17.19 to 4.17.21 in /platforms/r3-corda/images/doorman/website
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [lodash](https://github.com/lodash/lodash) from 4.17.19 to 4.17.21.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/lodash/lodash/commit/f299b52f39486275a9e6483b60a410e06520c538"><code>f299b52</code></a> Bump to v4.17.21</li>
<li><a href="https://github.com/lodash/lodash/commit/c4847ebe7d14540bb28a8b932a9ce1b9ecbfee1a"><code>c4847eb</code></a> Improve performance of <code>toNumber</code>, <code>trim</code> and <code>trimEnd</code> on large input strings</li>
<li><a href="https://github.com/lodash/lodash/commit/3469357cff396a26c363f8c1b5a91dde28ba4b1c"><code>3469357</code></a> Prevent command injection through <code>_.template</code>'s <code>variable</code> option</li>
<li><a href="https://github.com/lodash/lodash/commit/ded9bc66583ed0b4e3b7dc906206d40757b4a90a"><code>ded9bc6</code></a> Bump to v4.17.20.</li>
<li><a href="https://github.com/lodash/lodash/commit/63150ef7645ac07961b63a86490f419f356429aa"><code>63150ef</code></a> Documentation fixes.</li>
<li><a href="https://github.com/lodash/lodash/commit/00f0f62a979d2f5fa0287c06eae70cf9a62d8794"><code>00f0f62</code></a> test.js: Remove trailing comma.</li>
<li><a href="https://github.com/lodash/lodash/commit/846e434c7a5b5692c55ebf5715ed677b70a32389"><code>846e434</code></a> Temporarily use a custom fork of <code>lodash-cli</code>.</li>
<li><a href="https://github.com/lodash/lodash/commit/5d046f39cbd27f573914768e3b36eeefcc4f1229"><code>5d046f3</code></a> Re-enable Travis tests on <code>4.17</code> branch.</li>
<li><a href="https://github.com/lodash/lodash/commit/aa816b36d402a1ad9385142ce7188f17dae514fd"><code>aa816b3</code></a> Remove <code>/npm-package</code>.</li>
<li>See full diff in <a href="https://github.com/lodash/lodash/compare/4.17.19...4.17.21">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~bnjmnt4n">bnjmnt4n</a>, a new releaser for lodash since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=lodash&package-manager=npm_and_yarn&previous-version=4.17.19&new-version=4.17.21)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-05-10 11:33:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1450" class=".btn">#1450</a>
            </td>
            <td>
                <b>
                    Bump ua-parser-js from 0.7.19 to 0.7.28 in /platforms/r3-corda/images/networkmap/website
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [ua-parser-js](https://github.com/faisalman/ua-parser-js) from 0.7.19 to 0.7.28.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/1d3c98a10c23915046a362c4e3b3b503fb40d611"><code>1d3c98a</code></a> Revert breaking fix <a href="https://github-redirect.dependabot.com/faisalman/ua-parser-js/issues/279">#279</a> and release as 0.7.28</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/535f11bd2403910f29dabe6f90adb014ad016747"><code>535f11b</code></a> Delete redundant code</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/642c0399e831e27c5c86c3b7afee02e876250d01"><code>642c039</code></a> Fix <a href="https://github-redirect.dependabot.com/faisalman/ua-parser-js/issues/492">#492</a> LG TV WebOS detection</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/3edacddb2474429c55fa39d1e6222d50bbf9266f"><code>3edacdd</code></a> Merge branch 'master' into develop</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/acc0b91ff5defa2ca9a722874e27277879292907"><code>acc0b91</code></a> Update contributor list</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/f726dcd1ae4fea51e99b8ca574a1be51fbd70e1a"><code>f726dcd</code></a> Merge branch 'master' into develop</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/383ca587ef9b8daffcf652ac39fc9b8f3708572e"><code>383ca58</code></a> More test for tablet devices</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/7c8aa435b26cb14537423cd5fe4ce077e0661db2"><code>7c8aa43</code></a> Minor rearrangement</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/09aa9105dc370ded9275f70eae1f4eb67394966c"><code>09aa910</code></a> Add new device &amp; browser: Tesla</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/557cc2198d88068892eec6b61f2b2f4fe6e96314"><code>557cc21</code></a> More test for latest phones with unique form factor (fold/flip/qwerty/swivel)</li>
<li>Additional commits viewable in <a href="https://github.com/faisalman/ua-parser-js/compare/0.7.19...0.7.28">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ua-parser-js&package-manager=npm_and_yarn&previous-version=0.7.19&new-version=0.7.28)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-05-07 21:44:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1449" class=".btn">#1449</a>
            </td>
            <td>
                <b>
                    Bump ua-parser-js from 0.7.19 to 0.7.28 in /platforms/r3-corda/images/doorman/website
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [ua-parser-js](https://github.com/faisalman/ua-parser-js) from 0.7.19 to 0.7.28.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/1d3c98a10c23915046a362c4e3b3b503fb40d611"><code>1d3c98a</code></a> Revert breaking fix <a href="https://github-redirect.dependabot.com/faisalman/ua-parser-js/issues/279">#279</a> and release as 0.7.28</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/535f11bd2403910f29dabe6f90adb014ad016747"><code>535f11b</code></a> Delete redundant code</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/642c0399e831e27c5c86c3b7afee02e876250d01"><code>642c039</code></a> Fix <a href="https://github-redirect.dependabot.com/faisalman/ua-parser-js/issues/492">#492</a> LG TV WebOS detection</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/3edacddb2474429c55fa39d1e6222d50bbf9266f"><code>3edacdd</code></a> Merge branch 'master' into develop</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/acc0b91ff5defa2ca9a722874e27277879292907"><code>acc0b91</code></a> Update contributor list</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/f726dcd1ae4fea51e99b8ca574a1be51fbd70e1a"><code>f726dcd</code></a> Merge branch 'master' into develop</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/383ca587ef9b8daffcf652ac39fc9b8f3708572e"><code>383ca58</code></a> More test for tablet devices</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/7c8aa435b26cb14537423cd5fe4ce077e0661db2"><code>7c8aa43</code></a> Minor rearrangement</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/09aa9105dc370ded9275f70eae1f4eb67394966c"><code>09aa910</code></a> Add new device &amp; browser: Tesla</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/557cc2198d88068892eec6b61f2b2f4fe6e96314"><code>557cc21</code></a> More test for latest phones with unique form factor (fold/flip/qwerty/swivel)</li>
<li>Additional commits viewable in <a href="https://github.com/faisalman/ua-parser-js/compare/0.7.19...0.7.28">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ua-parser-js&package-manager=npm_and_yarn&previous-version=0.7.19&new-version=0.7.28)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-05-07 18:01:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1448" class=".btn">#1448</a>
            </td>
            <td>
                <b>
                    [corda] 4.7 upgrade
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Roy,Sownak <sownak.roy@accenture.com>

**Changelog**
- Add Corda OS 4.7 Support
- Update Cordite Networkmap to support HA Notaries
- Update Supplychain APP to use fixed notary service name
 

**Linked issue**
resolves #1440 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-07 16:16:55 +0000 UTC
    </div>
</div>

