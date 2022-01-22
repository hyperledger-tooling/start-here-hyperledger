---
layout: default
title: cello
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cello
---

# cello <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cello){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/392" class=".btn">#392</a>
            </td>
            <td>
                <b>
                    Bump log4js from 0.6.38 to 6.4.0 in /build_image/dockerhub/v0.9.0/user-dashboard
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [log4js](https://github.com/log4js-node/log4js-node) from 0.6.38 to 6.4.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/log4js-node/log4js-node/blob/master/CHANGELOG.md">log4js's changelog</a>.</em></p>
<blockquote>
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
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1134">chore(deps): bump date-format from 3.0.0 to 4.0.2</a> - thanks <a href="https://github.com/peteriman"><code>@​peteriman</code></a></li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1130">chore(deps): Updated dependencies</a> - thanks <a href="https://github.com/peteriman"><code>@​peteriman</code></a>
<ul>
<li>eslint-config-prettier from 6.15.0 to 8.3.0</li>
<li>eslint-plugin-prettier from 3.4.1 to 4.0.0</li>
<li>husky from 3.1.0 to 7.0.4</li>
<li>prettier from 1.19.0 to 2.5.1</li>
<li>typescript from 3.9.10 to 4.5.4</li>
</ul>
</li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1129">chore(deps-dev): bump eslint-config-prettier from 6.15.0 to 8.3.0</a> - thanks <a href="https://github.com/peteriman"><code>@​peteriman</code></a></li>
<li><a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/pull/1121">chore(deps): Updated dependencies</a> - thanks <a href="https://github.com/peteriman"><code>@​peteriman</code></a>
<ul>
<li>codecov from 3.6.1 to 3.8.3</li>
<li>eslint-config-prettier from 6.5.0 to 6.15.0</li>
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
<li><a href="https://github.com/log4js-node/log4js-node/commit/9fdbed5ad45d1b09b35c1ef5355ba726b60cb702"><code>9fdbed5</code></a> 6.4.0</li>
<li><a href="https://github.com/log4js-node/log4js-node/commit/788c7a83bbb6f9b20a9f17bd7c3013b78b72f4d3"><code>788c7a8</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/issues/1150">#1150</a> from log4js-node/update-changelog</li>
<li><a href="https://github.com/log4js-node/log4js-node/commit/7fdb141135e930960d44597d969a1aff14627346"><code>7fdb141</code></a> chore: updated changelog for 6.4.0</li>
<li><a href="https://github.com/log4js-node/log4js-node/commit/e6bd888c2d4ee2c0ba257349ce78112fc4a591be"><code>e6bd888</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/issues/1151">#1151</a> from log4js-node/feat-zero-backup</li>
<li><a href="https://github.com/log4js-node/log4js-node/commit/ac599e42c6762cd0cc6ee3a34873c6f839dd196f"><code>ac599e4</code></a> allow for zero backup - in sync with <a href="https://github.com/log4js-node/streamrol">https://github.com/log4js-node/streamrol</a>...</li>
<li><a href="https://github.com/log4js-node/log4js-node/commit/53248cd564f63ee2d5634761ed5078d8882d6df4"><code>53248cd</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/issues/1149">#1149</a> from log4js-node/migrate-daysToKeep-to-numBackups</li>
<li><a href="https://github.com/log4js-node/log4js-node/commit/436d9b49515601640be4866caa26d202684e5f26"><code>436d9b4</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/issues/1148">#1148</a> from log4js-node/update-docs</li>
<li><a href="https://github.com/log4js-node/log4js-node/commit/d6b017e72041913a18fefa0194459cebd63ba440"><code>d6b017e</code></a> chore(docs): updated fileSync.md and misc comments</li>
<li><a href="https://github.com/log4js-node/log4js-node/commit/d4617a730da73136be2e887e6a5ec28aacabd899"><code>d4617a7</code></a> chore(deps): migrated from daysToKeep to numBackups due to streamroller@^3.0.0</li>
<li><a href="https://github.com/log4js-node/log4js-node/commit/0ad013382345029d312d30f4d5783c1dd2c16182"><code>0ad0133</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/log4js-node/log4js-node/issues/1147">#1147</a> from log4js-node/update-deps</li>
<li>Additional commits viewable in <a href="https://github.com/log4js-node/log4js-node/compare/v0.6.38...v6.4.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=log4js&package-manager=npm_and_yarn&previous-version=0.6.38&new-version=6.4.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cello/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-21 21:59:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/391" class=".btn">#391</a>
            </td>
            <td>
                <b>
                    [#issue-389] implement query_installed & get_installed_package function
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                implement query_installed & get_installed_package function.We can query the chaincodes info has installed in peer nodes and can get installed chaincode.

Close #389

Signed-off-by: tianxuanhong1 <523713078@qq.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-21 02:01:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/388" class=".btn">#388</a>
            </td>
            <td>
                <b>
                    [#issue-387] implement chaincode install function
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                implement chaincode install function, url:/api/v1/chaincodes/install, and form-data body of key: chaincode_id. If you want to call this function manually, you need to query the ID of chaincode in the database first

Close #387

Signed-off-by: tianxuanhong1 <523713078@qq.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-20 09:14:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/386" class=".btn">#386</a>
            </td>
            <td>
                <b>
                    [#issue-385]Fix the problem of getting token
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixed the problem that the token could not be obtained after the first login

Close #385 
Signed-off-by: fengyang_sy <fengyang.09186@h3c.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-18 03:26:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/384" class=".btn">#384</a>
            </td>
            <td>
                <b>
                    [#issue-383]make dashboard image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1.add command to build dashboard image
2.bootup dashboard by "make start"
Close #383 
Signed-off-by: fengyang_sy <fengyang.09186@h3c.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-15 08:14:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/382" class=".btn">#382</a>
            </td>
            <td>
                <b>
                    Bump shelljs from 0.7.8 to 0.8.5 in /build_image/dockerhub/v0.9.0/user-dashboard
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [shelljs](https://github.com/shelljs/shelljs) from 0.7.8 to 0.8.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/shelljs/shelljs/releases">shelljs's releases</a>.</em></p>
<blockquote>
<h2>v0.8.5</h2>
<p>This was a small security fix for <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/1058">#1058</a>.</p>
<h2>v0.8.4</h2>
<p>Small patch release to fix a circular dependency warning in node v14. See <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/973">#973</a>.</p>
<h2>v0.8.3</h2>
<p><strong>Closed issues:</strong></p>
<ul>
<li>Shelljs print stderr to console even if exec-only &quot;silent&quot; is true <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/905">#905</a></li>
<li>refactor: remove common.state.tempDir <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/902">#902</a></li>
<li>Can't suppress stdout for echo <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/899">#899</a></li>
<li>exec() doesn't apply the arguments correctly <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/895">#895</a></li>
<li>shell.exec('npm pack') painfully slow <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/885">#885</a></li>
<li>shelljs.exec cannot find app.asar/node_modules/shelljs/src/exec-child.js <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/881">#881</a></li>
<li>test infra: mocks and skipOnWin conflict <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/862">#862</a></li>
<li>Support for shell function completion on IDE <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/859">#859</a></li>
<li>echo command shows options in stdout <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/855">#855</a></li>
<li>silent does not always work <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/851">#851</a></li>
<li>Appveyor installs the latest npm, instead of the latest compatible npm <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/844">#844</a></li>
<li>Force symbolic link (ln -sf) does not overwrite/recreate existing destination <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/830">#830</a></li>
<li>inconsistent result when trying to echo to a file <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/798">#798</a></li>
<li>Prevent require()ing executable-only files <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/789">#789</a></li>
<li>Cannot set property to of [object String] which has only a getter <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/752">#752</a></li>
<li>which() should check executability before returning a value <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/657">#657</a></li>
<li>Bad encoding experience <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/456">#456</a></li>
<li>phpcs very slow <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/440">#440</a></li>
<li>Error shown when triggering a sigint during shelljs.exec if process.on sigint is defined <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/254">#254</a></li>
<li><code>.to\(file\)</code> does not mute STDIO output <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/146">#146</a></li>
<li>Escaping shell arguments to exec() <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/143">#143</a></li>
<li>Allow multiple string arguments for exec() <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/103">#103</a></li>
<li>cp does not recursively copy from readonly location  <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/98">#98</a></li>
<li>Handling permissions errors on file I/O <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/64">#64</a></li>
</ul>
<p><strong>Merged pull requests:</strong></p>
<ul>
<li>Add test case for sed on empty file <a href="https://github-redirect.dependabot.com/shelljs/shelljs/pull/904">#904</a> (<a href="https://github.com/wyardley">wyardley</a>)</li>
<li>refactor: don't expose tempdir in common.state <a href="https://github-redirect.dependabot.com/shelljs/shelljs/pull/903">#903</a> (<a href="https://github.com/nfischer">nfischer</a>)</li>
<li>chore(ci): fix codecov on travis <a href="https://github-redirect.dependabot.com/shelljs/shelljs/pull/897">#897</a> (<a href="https://github.com/nfischer">nfischer</a>)</li>
<li>chore(npm): add ci-or-install script <a href="https://github-redirect.dependabot.com/shelljs/shelljs/pull/896">#896</a> (<a href="https://github.com/nfischer">nfischer</a>)</li>
<li>Fix silent exec <a href="https://github-redirect.dependabot.com/shelljs/shelljs/pull/892">#892</a> (<a href="https://github.com/nfischer">nfischer</a>)</li>
<li>chore(appveyor): run entire test matrix <a href="https://github-redirect.dependabot.com/shelljs/shelljs/pull/886">#886</a> (<a href="https://github.com/nfischer">nfischer</a>)</li>
<li>docs: remove gitter badge <a href="https://github-redirect.dependabot.com/shelljs/shelljs/pull/880">#880</a> (<a href="https://github.com/nfischer">nfischer</a>)</li>
<li>grep includes the i flag <a href="https://github-redirect.dependabot.com/shelljs/shelljs/pull/876">#876</a> (<a href="https://github.com/ppsleep">ppsleep</a>)</li>
<li>Fix(which): match only executable files (<a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/657">#657</a>) <a href="https://github-redirect.dependabot.com/shelljs/shelljs/pull/874">#874</a> (<a href="https://github.com/termosa">termosa</a>)</li>
<li>chore: rename some tests <a href="https://github-redirect.dependabot.com/shelljs/shelljs/pull/871">#871</a> (<a href="https://github.com/nfischer">nfischer</a>)</li>
<li>Fix cp from readonly source <a href="https://github-redirect.dependabot.com/shelljs/shelljs/pull/870">#870</a> (<a href="https://github.com/nfischer">nfischer</a>)</li>
<li>chore: bump dev dependencies and add package-lock <a href="https://github-redirect.dependabot.com/shelljs/shelljs/pull/864">#864</a> (<a href="https://github.com/nfischer">nfischer</a>)</li>
<li>fix(mocks): fix conflict between mocks and skip <a href="https://github-redirect.dependabot.com/shelljs/shelljs/pull/863">#863</a> (<a href="https://github.com/nfischer">nfischer</a>)</li>
<li>chore: output npm version in travis <a href="https://github-redirect.dependabot.com/shelljs/shelljs/pull/850">#850</a> (<a href="https://github.com/nfischer">nfischer</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/shelljs/shelljs/blob/master/CHANGELOG.md">shelljs's changelog</a>.</em></p>
<blockquote>
<h1>Change Log</h1>
<h2><a href="https://github.com/shelljs/shelljs/tree/HEAD">Unreleased</a></h2>
<p><a href="https://github.com/shelljs/shelljs/compare/v0.8.3...HEAD">Full Changelog</a></p>
<p><strong>Closed issues:</strong></p>
<ul>
<li>find returns empty array even though directory has files <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/922">#922</a></li>
<li>exec() should support node v10 (maxbuffer change) <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/915">#915</a></li>
<li>grep exit status and extra newlines <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/900">#900</a></li>
<li>Travis CI currently broken <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/893">#893</a></li>
<li>Drop node v4 support <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/873">#873</a></li>
<li>cp -Ru respects the -R but not the -u <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/808">#808</a></li>
</ul>
<p><strong>Merged pull requests:</strong></p>
<ul>
<li>feat(options): initial support for long options <a href="https://github-redirect.dependabot.com/shelljs/shelljs/pull/926">#926</a> (<a href="https://github.com/nfischer">nfischer</a>)</li>
<li>test(touch): add coverage for -d option <a href="https://github-redirect.dependabot.com/shelljs/shelljs/pull/925">#925</a> (<a href="https://github.com/nfischer">nfischer</a>)</li>
<li>chore(node): add v10 and v11 to CI <a href="https://github-redirect.dependabot.com/shelljs/shelljs/pull/921">#921</a> (<a href="https://github.com/nfischer">nfischer</a>)</li>
<li>chore(test): no coverage by default <a href="https://github-redirect.dependabot.com/shelljs/shelljs/pull/920">#920</a> (<a href="https://github.com/nfischer">nfischer</a>)</li>
<li>fix(exec): consistent error message for maxBuffer <a href="https://github-redirect.dependabot.com/shelljs/shelljs/pull/919">#919</a> (<a href="https://github.com/nfischer">nfischer</a>)</li>
<li>chore(node): drop node v4 and v5 <a href="https://github-redirect.dependabot.com/shelljs/shelljs/pull/917">#917</a> (<a href="https://github.com/nfischer">nfischer</a>)</li>
<li>chore: script to bump supported node versions <a href="https://github-redirect.dependabot.com/shelljs/shelljs/pull/913">#913</a> (<a href="https://github.com/nfischer">nfischer</a>)</li>
<li>chore(npm): remove lockfile <a href="https://github-redirect.dependabot.com/shelljs/shelljs/pull/911">#911</a> (<a href="https://github.com/nfischer">nfischer</a>)</li>
<li>ci: change language to node_js and remove obsolete scripts <a href="https://github-redirect.dependabot.com/shelljs/shelljs/pull/910">#910</a> (<a href="https://github.com/DanielRuf">DanielRuf</a>)</li>
<li>chore: remove gitter integration <a href="https://github-redirect.dependabot.com/shelljs/shelljs/pull/907">#907</a> (<a href="https://github.com/nfischer">nfischer</a>)</li>
<li>fix: Exit 1 with empty string if no match <a href="https://github-redirect.dependabot.com/shelljs/shelljs/pull/901">#901</a> (<a href="https://github.com/wyardley">wyardley</a>)</li>
<li>feat(cp): support update flag when recursing <a href="https://github-redirect.dependabot.com/shelljs/shelljs/pull/889">#889</a> (<a href="https://github.com/joshi-sh">joshi-sh</a>)</li>
</ul>
<h2><a href="https://github.com/shelljs/shelljs/tree/v0.8.3">v0.8.3</a> (2018-11-13)</h2>
<p><a href="https://github.com/shelljs/shelljs/compare/v0.8.2...v0.8.3">Full Changelog</a></p>
<p><strong>Closed issues:</strong></p>
<ul>
<li>Shelljs print stderr to console even if exec-only &quot;silent&quot; is true <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/905">#905</a></li>
<li>refactor: remove common.state.tempDir <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/902">#902</a></li>
<li>Can't suppress stdout for echo <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/899">#899</a></li>
<li>exec() doesn't apply the arguments correctly <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/895">#895</a></li>
<li>shell.exec('npm pack') painfully slow <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/885">#885</a></li>
<li>shelljs.exec cannot find app.asar/node_modules/shelljs/src/exec-child.js <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/881">#881</a></li>
<li>test infra: mocks and skipOnWin conflict <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/862">#862</a></li>
<li>Support for shell function completion on IDE <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/859">#859</a></li>
<li>echo command shows options in stdout <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/855">#855</a></li>
<li>silent does not always work <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/851">#851</a></li>
<li>Appveyor installs the latest npm, instead of the latest compatible npm <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/844">#844</a></li>
<li>Force symbolic link (ln -sf) does not overwrite/recreate existing destination <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/830">#830</a></li>
<li>inconsistent result when trying to echo to a file <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/798">#798</a></li>
<li>Prevent require()ing executable-only files <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/789">#789</a></li>
<li>Cannot set property to of [object String] which has only a getter <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/752">#752</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/shelljs/shelljs/commit/70668a4555c7d49c4f67d53ea063b899be4d6d40"><code>70668a4</code></a> 0.8.5</li>
<li><a href="https://github.com/shelljs/shelljs/commit/d919d22dd6de385edaa9d90313075a77f74b338c"><code>d919d22</code></a> fix(exec): lockdown file permissions (<a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/1060">#1060</a>)</li>
<li><a href="https://github.com/shelljs/shelljs/commit/fcf1651be9a3bb8e20ba1fd24b8a91f369829c53"><code>fcf1651</code></a> 0.8.4</li>
<li><a href="https://github.com/shelljs/shelljs/commit/a1111ee793e0292e4eff27b69214b361bd1eb712"><code>a1111ee</code></a> Silence potentially upcoming circular dependency warning (<a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/973">#973</a>)</li>
<li><a href="https://github.com/shelljs/shelljs/commit/d4d1317ce62531fbd49085852b8492db3dd39312"><code>d4d1317</code></a> 0.8.3</li>
<li><a href="https://github.com/shelljs/shelljs/commit/db317bf09236b8cabfa6a18b232a02035e9e08f1"><code>db317bf</code></a> Add test case for sed on empty file (<a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/904">#904</a>)</li>
<li><a href="https://github.com/shelljs/shelljs/commit/0d5ecb673e65d4041a2ca26956deee7f5b9480f4"><code>0d5ecb6</code></a> docs(changelog): updated by Nate Fischer [ci skip]</li>
<li><a href="https://github.com/shelljs/shelljs/commit/6b3c7b1e44b5cd308aac3a924165658fac3268d8"><code>6b3c7b1</code></a> refactor: don't expose tempdir in common.state (<a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/903">#903</a>)</li>
<li><a href="https://github.com/shelljs/shelljs/commit/4bd22e77423182219cd43f0c8d38621b1c957986"><code>4bd22e7</code></a> chore(ci): fix codecov on travis (<a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/897">#897</a>)</li>
<li><a href="https://github.com/shelljs/shelljs/commit/2b3b781bbc41add8ca17bcd35a6d8f19797285ce"><code>2b3b781</code></a> fix: silent exec (<a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/892">#892</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/shelljs/shelljs/compare/v0.7.8...v0.8.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=shelljs&package-manager=npm_and_yarn&previous-version=0.7.8&new-version=0.8.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cello/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-15 05:55:03 +0000 UTC
    </div>
</div>

