---
layout: default
title: solang
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1608" class=".btn">#1608</a>
            </td>
            <td>
                <b>
                    Move to llvm16
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-08 09:41:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1607" class=".btn">#1607</a>
            </td>
            <td>
                <b>
                    [Snyk] Upgrade @solana/spl-token from 0.3.8 to 0.3.9
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <p>This PR was automatically created by Snyk using the credentials of a real user.</p><br /><h3>Snyk has created this PR to upgrade @solana/spl-token from 0.3.8 to 0.3.9.</h3>

:information_source: Keep your dependencies up-to-date. This makes it easier to fix existing vulnerabilities and to more quickly identify and fix newly disclosed vulnerabilities when they affect your project.
<hr/>

- The recommended version is **1 version** ahead of your current version.
- The recommended version was released **21 days ago**, on 2023-11-14.


<details>
<summary><b>Release notes</b></summary>
<br/>
  <details>
    <summary>Package name: <b>@solana/spl-token</b></summary>
    <ul>
      <li>
        <b>0.3.9</b> - <a href="https://snyk.io/redirect/github/solana-labs/solana-program-library/releases/tag/token-js-v0.3.9">2023-11-14</a></br><p>Introduces support for new Token2022 extension functionality:</p>
<ul>
<li><code>TransferHook</code> extension:
<ul>
<li>Account data seed configurations for account resolution (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1990587155" data-permission-text="Title is private" data-url="https://github.com/solana-labs/solana-program-library/issues/5815" data-hovercard-type="pull_request" data-hovercard-url="/solana-labs/solana-program-library/pull/5815/hovercard" href="https://snyk.io/redirect/github/solana-labs/solana-program-library/pull/5815">#5815</a>)</li>
<li>Account meta de-escalation checks when adding extra metas to instructions (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1990587339" data-permission-text="Title is private" data-url="https://github.com/solana-labs/solana-program-library/issues/5816" data-hovercard-type="pull_request" data-hovercard-url="/solana-labs/solana-program-library/pull/5816/hovercard" href="https://snyk.io/redirect/github/solana-labs/solana-program-library/pull/5816">#5816</a>)</li>
<li>Accounts list ordering ensured to match Rust offchain implementation (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1990587490" data-permission-text="Title is private" data-url="https://github.com/solana-labs/solana-program-library/issues/5817" data-hovercard-type="pull_request" data-hovercard-url="/solana-labs/solana-program-library/pull/5817/hovercard" href="https://snyk.io/redirect/github/solana-labs/solana-program-library/pull/5817">#5817</a>)</li>
</ul>
</li>
<li><code>MetadataPointer</code> extension:
<ul>
<li>Adds the <code>MetadataPointer</code> extension to the library's extension support (<a class="issue-link js-issue-link" data-error-text="Failed to load title" data-id="1988811179" data-permission-text="Title is private" data-url="https://github.com/solana-labs/solana-program-library/issues/5805" data-hovercard-type="pull_request" data-hovercard-url="/solana-labs/solana-program-library/pull/5805/hovercard" href="https://snyk.io/redirect/github/solana-labs/solana-program-library/pull/5805">#5805</a>)</li>
</ul>
</li>
</ul>
<p>Thanks for the contributions, <a class="user-mention notranslate" data-hovercard-type="user" data-hovercard-url="/users/mistersimon/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="https://snyk.io/redirect/github/mistersimon">@ mistersimon</a> !</p>
      </li>
      <li>
        <b>0.3.8</b> - 2023-06-01
      </li>
    </ul>
    from <a href="https://snyk.io/redirect/github/solana-labs/solana-program-library/releases">@solana/spl-token GitHub release notes</a>
  </details>
</details>


<details>
  <summary><b>Commit messages</b></summary>
  </br>
  <details>
    <summary>Package name: <b>@solana/spl-token</b></summary>
    <ul>
      <li><a href="https://snyk.io/redirect/github/solana-labs/solana-program-library/commit/a1404b34675945b34873b190d52963f105581d9d">a1404b3</a> [token js]: bump version (#5813)</li>
      <li><a href="https://snyk.io/redirect/github/solana-labs/solana-program-library/commit/ce3e4fc9a0d0f27cd3874038aa560c63594813b7">ce3e4fc</a> build(deps): bump @ solana/codecs-numbers from 2.0.0-experimental.398c396 to 2.0.0-experimental.7123512 (#5831)</li>
      <li><a href="https://snyk.io/redirect/github/solana-labs/solana-program-library/commit/a862ec1b40ce865b5514da9f5e4c81724bda25da">a862ec1</a> build(deps): bump @ solana/options from 2.0.0-experimental.398c396 to 2.0.0-experimental.7123512 (#5826)</li>
      <li><a href="https://snyk.io/redirect/github/solana-labs/solana-program-library/commit/906d4964f42ef5d1754416a1415b218b9bce3ca9">906d496</a> build(deps): bump @ solana/codecs-core from 2.0.0-experimental.398c396 to 2.0.0-experimental.7123512 (#5823)</li>
      <li><a href="https://snyk.io/redirect/github/solana-labs/solana-program-library/commit/26fded0ef3184d80ee34959f445f017f755f74ad">26fded0</a> build(deps-dev): bump @ typescript-eslint/eslint-plugin from 6.10.0 to 6.11.0 (#5828)</li>
      <li><a href="https://snyk.io/redirect/github/solana-labs/solana-program-library/commit/0047bd2fadf7ba71ee6f2a7b932f94d9fce1717b">0047bd2</a> build(deps-dev): bump prettier from 3.0.3 to 3.1.0 (#5827)</li>
      <li><a href="https://snyk.io/redirect/github/solana-labs/solana-program-library/commit/69de0acecdb0f54bffdd70fe344f8eca2c2f0f7f">69de0ac</a> build(deps-dev): bump tsx from 3.14.0 to 4.1.2 (#5825)</li>
      <li><a href="https://snyk.io/redirect/github/solana-labs/solana-program-library/commit/6a27f96aaece3a87f66b885e56f8b266ccb77f99">6a27f96</a> dependabot: Fix time format to add leading 0 (#5822)</li>
      <li><a href="https://snyk.io/redirect/github/solana-labs/solana-program-library/commit/2b30a1b250b89fcb21bf1323e002bc32c590ddd8">2b30a1b</a> [token js]: transfer-hook: align key pushing flow with Rust helpers</li>
      <li><a href="https://snyk.io/redirect/github/solana-labs/solana-program-library/commit/1b89c06f57fd3ae43ae9259c4a2a805aca4703f5">1b89c06</a> [token js]: transfer-hook: add account meta de-escalation</li>
      <li><a href="https://snyk.io/redirect/github/solana-labs/solana-program-library/commit/7b3fef16a4e6ee95fd01b26bc19747f76b19ec7d">7b3fef1</a> [token js]: transfer-hook: add support for account data seeds</li>
      <li><a href="https://snyk.io/redirect/github/solana-labs/solana-program-library/commit/7a4af0a9e67e605bfadffd351cb0a489dae87e9b">7a4af0a</a> js: Add top-level package.json and turbo build (#5819)</li>
      <li><a href="https://snyk.io/redirect/github/solana-labs/solana-program-library/commit/2c1480c52933a22a5c6ed80c781b4067efe51486">2c1480c</a> build(deps): bump proptest from 1.3.1 to 1.4.0 (#5812)</li>
      <li><a href="https://snyk.io/redirect/github/solana-labs/solana-program-library/commit/c94eeec63bdada46453eb46d0e7add4c504b1799">c94eeec</a> token-cli: Refactor tests out of &#x60;main.rs&#x60; (#5804)</li>
      <li><a href="https://snyk.io/redirect/github/solana-labs/solana-program-library/commit/6ac9c28e3a77c9ec5cbcf56cca2226d140822ae8">6ac9c28</a> token-cli: Make update confidential accept multiple args (#5814)</li>
      <li><a href="https://snyk.io/redirect/github/solana-labs/solana-program-library/commit/20f27e2fb68aff98040d3a13e0fa559c7177b0a3">20f27e2</a> token 2022: add metadata pointer extension to js @ solana/spl-token client (#5805)</li>
      <li><a href="https://snyk.io/redirect/github/solana-labs/solana-program-library/commit/6fe3c15a63c0503991514baec90bf30923a30ed6">6fe3c15</a> docs: Fix typos (#5808)</li>
      <li><a href="https://snyk.io/redirect/github/solana-labs/solana-program-library/commit/b1ba6493fb49a89fcbb0abcf0b5f05694a8bf7d1">b1ba649</a> single-pool-js: remove unnecessary deps (#5801)</li>
      <li><a href="https://snyk.io/redirect/github/solana-labs/solana-program-library/commit/f542e00a8905eaf3f55dea1c08ca4787138e1788">f542e00</a> README: Use commit hashes for audits (#5799)</li>
      <li><a href="https://snyk.io/redirect/github/solana-labs/solana-program-library/commit/e6af88751ce3cae4014a311c1ae327b843af10de">e6af887</a> build(deps): bump tokio from 1.33.0 to 1.34.0 (#5800)</li>
      <li><a href="https://snyk.io/redirect/github/solana-labs/solana-program-library/commit/6ed7254d1a578ffbc2b091d28cb92b25e7cc511d">6ed7254</a> stake-pool: Allow mints with confidential transfer fee (#5610)</li>
      <li><a href="https://snyk.io/redirect/github/solana-labs/solana-program-library/commit/1194694fcb312963ca48b81e530a138200caefa5">1194694</a> single-pool-js: bump version</li>
      <li><a href="https://snyk.io/redirect/github/solana-labs/solana-program-library/commit/80adefd344a9082bd75a5f60e7de45f8a451ad6c">80adefd</a> single-pool: update docs with examples (#5414)</li>
      <li><a href="https://snyk.io/redirect/github/solana-labs/solana-program-library/commit/fddc4f43622a10ab7caec1a2b9b14f7572cb7697">fddc4f4</a> build(deps): bump superstruct from 0.14.2 to 1.0.3 in /stake-pool/js (#5793)</li>
    </ul>

   <a href="https://snyk.io/redirect/github/solana-labs/solana-program-library/compare/8f9c33b3a04250938a573809cd9dfdb698025972...a1404b34675945b34873b190d52963f105581d9d">Compare</a>
  </details>
</details>
<hr/>

**Note:** *You are seeing this because you or someone else with access to this repository has authorized Snyk to open upgrade PRs.*

For more information:  <img src="https://api.segment.io/v1/pixel/track?data=eyJ3cml0ZUtleSI6InJyWmxZcEdHY2RyTHZsb0lYd0dUcVg4WkFRTnNCOUEwIiwiYW5vbnltb3VzSWQiOiIyMzZlZDFjMi1mNmRlLTQ2MDktYjhkOS0xNjFiMDYwNDVkYWUiLCJldmVudCI6IlBSIHZpZXdlZCIsInByb3BlcnRpZXMiOnsicHJJZCI6IjIzNmVkMWMyLWY2ZGUtNDYwOS1iOGQ5LTE2MWIwNjA0NWRhZSJ9fQ==" width="0" height="0"/>

🧐 [View latest project report](https://app.snyk.io/org/hyperledger-bot/project/ccb2ab6a-ba20-4d58-979d-b59e66a8e113?utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr)

🛠 [Adjust upgrade PR settings](https://app.snyk.io/org/hyperledger-bot/project/ccb2ab6a-ba20-4d58-979d-b59e66a8e113/settings/integration?utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr)

🔕 [Ignore this dependency or unsubscribe from future upgrade PRs](https://app.snyk.io/org/hyperledger-bot/project/ccb2ab6a-ba20-4d58-979d-b59e66a8e113/settings/integration?pkg&#x3D;@solana/spl-token&amp;utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr#auto-dep-upgrades)

<!--- (snyk:metadata:{"prId":"236ed1c2-f6de-4609-b8d9-161b06045dae","prPublicId":"236ed1c2-f6de-4609-b8d9-161b06045dae","dependencies":[{"name":"@solana/spl-token","from":"0.3.8","to":"0.3.9"}],"packageManager":"npm","type":"auto","projectUrl":"https://app.snyk.io/org/hyperledger-bot/project/ccb2ab6a-ba20-4d58-979d-b59e66a8e113?utm_source=github&utm_medium=referral&page=upgrade-pr","projectPublicId":"ccb2ab6a-ba20-4d58-979d-b59e66a8e113","env":"prod","prType":"upgrade","vulns":[],"issuesToFix":[],"upgrade":[],"upgradeInfo":{"versionsDiff":1,"publishedDate":"2023-11-14T14:21:09.007Z"},"templateVariants":[],"hasFixes":false,"isMajorUpgrade":false,"isBreakingChange":false,"priorityScoreList":[]}) --->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-05 22:56:18 +0000 UTC
    </div>
</div>

