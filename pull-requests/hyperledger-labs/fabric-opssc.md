---
layout: default
title: fabric-opssc
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-opssc
---

# fabric-opssc <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-opssc){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-opssc/pull/32" class=".btn">#32</a>
            </td>
            <td>
                <b>
                    feat(*): Improve Web Socket notifications and some log formats
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This patch includes:
- feat(api-server): Add config options whether to enable WebSocket server
- feat(agent): Improve console log and WebSocket message format
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-18 11:32:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-opssc/pull/31" class=".btn">#31</a>
            </td>
            <td>
                <b>
                    chore(*): Bump fabric versions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This patch updates the fabric versions for build and testing:
- Update Fabric from 2.4.1 to 2.4.2
- Update Fabric from 2.2.4 to 2.2.5

Also, this patch removes the v2.3 series from build and testing
because they haven't been an update since the release of the 2.4 series.

This includes updating the OpsSC related material information in README.

Signed-off-by: Tatsuya Sato <tatsuya.sato.so@hitachi.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-17 01:13:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-opssc/pull/30" class=".btn">#30</a>
            </td>
            <td>
                <b>
                    Some bug fixes and adding a minor API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR includes the following updates.

- Bug fixes
  - Bug fix on the conditions for a vote to be considered `Rejected`
  - Bug fix in the case of reusing chaincode definitions without proposals
-  API updates
   - Add API to get organization information
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-16 04:02:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-opssc/pull/29" class=".btn">#29</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump lodash from 4.17.20 to 4.17.21 in /integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [lodash](https://github.com/lodash/lodash) from 4.17.20 to 4.17.21.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/lodash/lodash/commit/f299b52f39486275a9e6483b60a410e06520c538"><code>f299b52</code></a> Bump to v4.17.21</li>
<li><a href="https://github.com/lodash/lodash/commit/c4847ebe7d14540bb28a8b932a9ce1b9ecbfee1a"><code>c4847eb</code></a> Improve performance of <code>toNumber</code>, <code>trim</code> and <code>trimEnd</code> on large input strings</li>
<li><a href="https://github.com/lodash/lodash/commit/3469357cff396a26c363f8c1b5a91dde28ba4b1c"><code>3469357</code></a> Prevent command injection through <code>_.template</code>'s <code>variable</code> option</li>
<li>See full diff in <a href="https://github.com/lodash/lodash/compare/4.17.20...4.17.21">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=lodash&package-manager=npm_and_yarn&previous-version=4.17.20&new-version=4.17.21)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-opssc/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-15 03:13:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-opssc/pull/28" class=".btn">#28</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump log4js from 6.3.0 to 6.4.1 in /integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [log4js](https://github.com/log4js-node/log4js-node) from 6.3.0 to 6.4.1.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/log4js-node/log4js-node/blob/master/CHANGELOG.md">log4js's changelog</a>.</em></p>
<blockquote>
<h2>6.4.1</h2>
<ul>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1162">bug: Fixed to startup multiprocess even when no direct appenders</a> - thanks <a href="https://github.com/nicojs"><code>@​nicojs</code></a>
<ul>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1165">refactor: fixed eslint warnings</a> - thanks <a href="https://github.com/peteriman"><code>@​peteriman</code></a></li>
</ul>
</li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1163">improvement: additional alias for date patterns</a> - thanks <a href="https://github.com/peteriman"><code>@​peteriman</code></a></li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1164">improvement: added emitWarning for deprecation</a> - thanks <a href="https://github.com/peteriman"><code>@​peteriman</code></a></li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1158">type: Fixed wrong types from 6.4.0 regression</a> - thanks <a href="https://github.com/glasser"><code>@​glasser</code></a></li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1153">chore(docs): changed author to contributors in package.json</a> - thanks <a href="https://github.com/peteriman"><code>@​peteriman</code></a></li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1167">chore(deps): bump node-fetch from 2.6.6 to 2.6.7</a> - thanks <a href="https://github.com/dependabot"><code>@​Dependabot</code></a></li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1166">chore(deps-dev): bump typescript from 4.5.4 to 4.5.5</a> - thanks <a href="https://github.com/peteriman"><code>@​peteriman</code></a></li>
</ul>
<h2>6.4.0</h2>
<ul>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1141">security: default file permission to be 0o600 instead of 0o644</a> - thanks <a href="https://www.huntr.dev/users/ranjit-git">ranjit-git</a> and <a href="https://github.com/peteriman"><code>@​peteriman</code></a>
<ul>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1148">chore(docs): updated fileSync.md and misc comments</a> - thanks <a href="https://github.com/peteriman"><code>@​peteriman</code></a></li>
</ul>
</li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1062">feat: Added warnings when log() is used with invalid levels before fallbacking to INFO</a> - thanks <a href="https://github.com/abernh"><code>@​abernh</code></a></li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1103">feat: exposed Recording</a> - thanks <a href="https://github.com/polo-language"><code>@​polo-language</code></a></li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1113">bug: Fixed file descriptor leak if repeated configure()</a> - thanks <a href="https://github.com/peteriman"><code>@​peteriman</code></a></li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1110">bug: Fixed MaxListenersExceededWarning from NodeJS</a> - thanks <a href="https://github.com/peteriman"><code>@​peteriman</code></a>
<ul>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1142">test: added assertion for increase of SIGHUP listeners on log4js.configure()</a> - thanks <a href="https://github.com/peteriman"><code>@​peteriman</code></a></li>
</ul>
</li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1028">bug: Fixed missing TCP appender with Webpack and Typescript</a> - thanks <a href="https://github.com/techmunk"><code>@​techmunk</code></a></li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1097">bug: Fixed dateFile appender exiting NodeJS on error</a> - thanks <a href="https://github.com/4eb0da"><code>@​4eb0da</code></a>
<ul>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1144">refactor: using writer.writable instead of alive for checking</a> - thanks <a href="https://github.com/peteriman"><code>@​peteriman</code></a></li>
</ul>
</li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1089">bug: Fixed TCP appender exiting NodeJS on error</a> - thanks <a href="https://github.com/jhonatanTeixeira"><code>@​jhonatanTeixeira</code></a></li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/529">bug: Fixed Multiprocess appender exiting NodeJS on error</a> - thanks <a href="https://github.com/harlentan"><code>@​harlentan</code></a></li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1127">test: update fakeFS.read as graceful-fs uses it</a> - thanks <a href="https://github.com/peteriman"><code>@​peteriman</code></a></li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1128">test: update fakeFS.realpath as fs-extra uses it</a> - thanks <a href="https://github.com/peteriman"><code>@​peteriman</code></a></li>
<li>test: added tap.tearDown() to clean up test files
<ul>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1143">#1143</a> - thanks <a href="https://github.com/peteriman"><code>@​peteriman</code></a></li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1022">#1022</a> - thanks <a href="https://github.com/abetomo"><code>@​abetomo</code></a></li>
</ul>
</li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1079"><code>type: improved @​types for AppenderModule</code></a> - thanks <a href="https://github.com/nicobao"><code>@​nicobao</code></a></li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1116">type: Updated fileSync appender types</a> - thanks <a href="https://github.com/peteriman"><code>@​peteriman</code></a></li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1031">type: Removed erroneous type in file appender</a> - thanks <a href="https://github.com/vdmtrv"><code>@​vdmtrv</code></a></li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1115">type: Updated Logger.log type</a> - thanks <a href="https://github.com/ZLundqvist"><code>@​ZLundqvist</code></a></li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1117">type: Updated Logger._log type</a> - thanks <a href="https://github.com/peteriman"><code>@​peteriman</code></a></li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1118">type: Updated Logger.level type</a> - thanks <a href="https://github.com/peteriman"><code>@​peteriman</code></a></li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1072">type: Updated Levels.getLevel type</a> - thanks <a href="https://github.com/saulzhong"><code>@​saulzhong</code></a></li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1147">chore(deps): bump streamroller from 3.0.1 to 3.0.2</a> - thanks <a href="https://github.com/peteriman"><code>@​peteriman</code></a></li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1146">chore(deps): bump date-format from 4.0.2 to 4.0.3</a> - thanks <a href="https://github.com/peteriman"><code>@​peteriman</code></a></li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1145">chore(deps-dev): bump eslint from from 8.6.0 to 8.7.0</a> - thanks <a href="https://github.com/peteriman"><code>@​peteriman</code></a></li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1140">chore(deps-dev): bump nyc from 14.1.1 to 15.1.0</a> - thanks <a href="https://github.com/peteriman"><code>@​peteriman</code></a></li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1138">chore(deps-dev): bump eslint from 5.16.0 to 8.6.0</a> - thanks <a href="https://github.com/peteriman"><code>@​peteriman</code></a></li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1137">chore(deps): bump flatted from 2.0.2 to 3.2.4</a> - thanks <a href="https://github.com/peteriman"><code>@​peteriman</code></a></li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1136">chore(deps-dev): bump fs-extra from 8.1.0 to 10.0.0</a> - thanks <a href="https://github.com/peteriman"><code>@​peteriman</code></a></li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1135">chore(deps): bump streamroller from 2.2.4 to 3.0.1</a> - thanks <a href="https://github.com/peteriman"><code>@​peteriman</code></a>
<ul>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1151">feat: allows for zero backups</a> - thanks <a href="https://github.com/peteriman"><code>@​peteriman</code></a></li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1149">api: migrated from daysToKeep to numBackups due to streamroller@^3.0.0</a> - thanks <a href="https://github.com/peteriman"><code>@​peteriman</code></a></li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/streamroller/pull/65">bug: compressed file ignores dateFile appender &quot;mode&quot;</a> - thanks <a href="https://github.com/rnd-debug"><code>@​rnd-debug</code></a></li>
<li>issue: addresses additional separator in filename (<a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/issues/1039">#1039</a>) - details: <a href="https://github.com/log4js-node/streamroller/blob/master/CHANGELOG.md">streamroller@3.0.0 changelog</a></li>
<li>issue: addresses daysToKeep naming confusion (<a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/issues/1035">#1035</a>, <a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/issues/1080">#1080</a>)  - details: <a href="https://github.com/log4js-node/streamroller/blob/master/CHANGELOG.md">streamroller@3.0.0 changelog</a></li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/log4js-node/log4js-node/commit/909a522c2789a5c404ae0720e581837ec4476753"><code>909a522</code></a> 6.4.1</li>
<li><a href="https://github.com/log4js-node/log4js-node/commit/461f2fbe8c2e20e8716c7d11ef22a17e6c24a6da"><code>461f2fb</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/issues/1168">#1168</a> from log4js-node/update-changelog</li>
<li><a href="https://github.com/log4js-node/log4js-node/commit/060da55fe84b617a510e3766674ebac1cdb50174"><code>060da55</code></a> Updated package.json to npm publish CHANGELOG.md and SECURITY.md</li>
<li><a href="https://github.com/log4js-node/log4js-node/commit/1fdc562430e54cd81d6948404398b7fc37370f62"><code>1fdc562</code></a> chore: updated changelog for 6.4.1</li>
<li><a href="https://github.com/log4js-node/log4js-node/commit/aed96d1e6532c25f205fcd254b21960fc833a3a6"><code>aed96d1</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/issues/1167">#1167</a> from log4js-node/dependabot/npm_and_yarn/node-fetch-...</li>
<li><a href="https://github.com/log4js-node/log4js-node/commit/1dd2f173acf168eeabef91fda58bad7765d7caf0"><code>1dd2f17</code></a> chore(deps): bump node-fetch from 2.6.6 to 2.6.7</li>
<li><a href="https://github.com/log4js-node/log4js-node/commit/2a959156319dccf87ffb7ea6c460b92d1aaa6086"><code>2a95915</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/issues/1166">#1166</a> from log4js-node/update-deps</li>
<li><a href="https://github.com/log4js-node/log4js-node/commit/a7ec9bad90c890043d18abf1cdd1560340d73f3d"><code>a7ec9ba</code></a> chore(deps-dev): bump typescript from 4.5.4 to 4.5.5</li>
<li><a href="https://github.com/log4js-node/log4js-node/commit/adcd0ffeaf37425da6bf11890eca0bc73966f4c5"><code>adcd0ff</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/issues/1165">#1165</a> from log4js-node/fixed-eslint</li>
<li><a href="https://github.com/log4js-node/log4js-node/commit/bf2b326e518b423a89a20076af78e5154d7c525c"><code>bf2b326</code></a> fixed eslint</li>
<li>Additional commits viewable in <a href="https://github.com/log4js-node/log4js-node/compare/v6.3.0...v6.4.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=log4js&package-manager=npm_and_yarn&previous-version=6.3.0&new-version=6.4.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-opssc/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-15 03:13:10 +0000 UTC
    </div>
</div>

