---
layout: default
title: blockchain-explorer
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/blockchain-explorer
---

# blockchain-explorer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/blockchain-explorer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/blockchain-explorer/pull/273" class=".btn">#273</a>
            </td>
            <td>
                <b>
                    Bump nanoid from 3.1.30 to 3.2.0 in /client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [nanoid](https://github.com/ai/nanoid) from 3.1.30 to 3.2.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ai/nanoid/blob/main/CHANGELOG.md">nanoid's changelog</a>.</em></p>
<blockquote>
<h1>Change Log</h1>
<p>This project adheres to <a href="http://semver.org/">Semantic Versioning</a>.</p>
<h2>3.2</h2>
<ul>
<li>Added <code>--size</code> and <code>--alphabet</code> arguments to binary (by Vitaly Baev).</li>
</ul>
<h2>3.1.32</h2>
<ul>
<li>Reduced <code>async</code> exports size (by Artyom Arutyunyan).</li>
<li>Moved from Jest to uvu (by Vitaly Baev).</li>
</ul>
<h2>3.1.31</h2>
<ul>
<li>Fixed collision vulnerability on object in <code>size</code> (by Artyom Arutyunyan).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ai/nanoid/commit/23b136929a6d58f32e31b269534a3ce3f680a086"><code>23b1369</code></a> Release 3.2 version</li>
<li><a href="https://github.com/ai/nanoid/commit/967788efce880960512f969a56f8f22f3fc20bae"><code>967788e</code></a> Remove TS test tools</li>
<li><a href="https://github.com/ai/nanoid/commit/27eaa90cd207a7782bbcf17343092ae87dd62164"><code>27eaa90</code></a> Simplify new binary tool</li>
<li><a href="https://github.com/ai/nanoid/commit/a9d91239931dc77506381874826d297aee71d6ef"><code>a9d9123</code></a> Update dependencies</li>
<li><a href="https://github.com/ai/nanoid/commit/32b9bdaab1fbc28576b17de8516164ce0360f292"><code>32b9bda</code></a> Allows passing size or custom alphabet via cli as args (<a href="https://github-redirect.dependabot.com/ai/nanoid/issues/334">#334</a>)</li>
<li><a href="https://github.com/ai/nanoid/commit/246d5f87b6b34e23b5e401bdf3da1f80c810ac4c"><code>246d5f8</code></a> Update vite</li>
<li><a href="https://github.com/ai/nanoid/commit/afdf9c92b41427f35476fbe14b5af5d73dd7fbdb"><code>afdf9c9</code></a> doc: Fixed Typo (<a href="https://github-redirect.dependabot.com/ai/nanoid/issues/335">#335</a>)</li>
<li><a href="https://github.com/ai/nanoid/commit/90a446fef3ecaac78e5af2ea01025c4f40182e2b"><code>90a446f</code></a> Update benchmark results</li>
<li><a href="https://github.com/ai/nanoid/commit/8ba2319b579895cc1f9060b9946a44852f97c509"><code>8ba2319</code></a> bench: add <code>@​napi-rs/uuid</code> v4 (<a href="https://github-redirect.dependabot.com/ai/nanoid/issues/333">#333</a>)</li>
<li><a href="https://github.com/ai/nanoid/commit/f4257780ece488734a65c176e80c2fd8ab6aab8e"><code>f425778</code></a> Release 3.1.32 version</li>
<li>Additional commits viewable in <a href="https://github.com/ai/nanoid/compare/3.1.30...3.2.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=nanoid&package-manager=npm_and_yarn&previous-version=3.1.30&new-version=3.2.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/blockchain-explorer/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-22 11:04:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/blockchain-explorer/pull/272" class=".btn">#272</a>
            </td>
            <td>
                <b>
                    Bump log4js from 6.3.0 to 6.4.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [log4js](https://github.com/log4js-node/log4js-node) from 6.3.0 to 6.4.0.
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
<li>Additional commits viewable in <a href="https://github.com/log4js-node/log4js-node/compare/v6.3.0...v6.4.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=log4js&package-manager=npm_and_yarn&previous-version=6.3.0&new-version=6.4.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/blockchain-explorer/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-21 20:34:13 +0000 UTC
    </div>
</div>

