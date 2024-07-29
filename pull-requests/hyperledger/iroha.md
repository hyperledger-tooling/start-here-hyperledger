---
layout: default
title: iroha
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha
---

# iroha <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4913" class=".btn">#4913</a>
            </td>
            <td>
                <b>
                    chore(deps): bump trybuild from 1.0.97 to 1.0.98
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [trybuild](https://github.com/dtolnay/trybuild) from 1.0.97 to 1.0.98.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/trybuild/releases">trybuild's releases</a>.</em></p>
<blockquote>
<h2>1.0.98</h2>
<ul>
<li>Fix enabling of default features for workspace dependencies (<a href="https://redirect.github.com/dtolnay/trybuild/issues/282">#282</a>, thanks <a href="https://github.com/gui1117"><code>@​gui1117</code></a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/trybuild/commit/a4f4171e5595d2537d273e72394230adcb97c54b"><code>a4f4171</code></a> Release 1.0.98</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/aa567ec5426d6bf91225784fd399e11518995d88"><code>aa567ec</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/trybuild/issues/282">#282</a> from gui1117/gui-fix-default-features</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/c08e3f76e6a26fce9f9f01f7ca94c70a91a1f345"><code>c08e3f7</code></a> remove unused</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/cd88ca2bb4c27baf2d578014c42f8e62f0cf0cd9"><code>cd88ca2</code></a> Fix default features</li>
<li>See full diff in <a href="https://github.com/dtolnay/trybuild/compare/1.0.97...1.0.98">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=trybuild&package-manager=cargo&previous-version=1.0.97&new-version=1.0.98)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-29 16:50:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4912" class=".btn">#4912</a>
            </td>
            <td>
                <b>
                    chore(deps): bump serde_json from 1.0.120 to 1.0.121
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [serde_json](https://github.com/serde-rs/json) from 1.0.120 to 1.0.121.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/serde-rs/json/releases">serde_json's releases</a>.</em></p>
<blockquote>
<h2>v1.0.121</h2>
<ul>
<li>Optimize position search in error path (<a href="https://redirect.github.com/serde-rs/json/issues/1160">#1160</a>, thanks <a href="https://github.com/purplesyringa"><code>@​purplesyringa</code></a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/serde-rs/json/commit/eca2658a22cb39952783cb6914eb18242659f66a"><code>eca2658</code></a> Release 1.0.121</li>
<li><a href="https://github.com/serde-rs/json/commit/b0d678cfb473386830d559b6ab255d9e21ba39c5"><code>b0d678c</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/json/issues/1160">#1160</a> from iex-rs/efficient-position</li>
<li><a href="https://github.com/serde-rs/json/commit/b1edc7d13f72880fd0ac569403a409e5f7961d5f"><code>b1edc7d</code></a> Optimize position search in error path</li>
<li><a href="https://github.com/serde-rs/json/commit/40dd7f5e862436f02471fe076f3486c55e472bc2"><code>40dd7f5</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/json/issues/1159">#1159</a> from iex-rs/fix-recursion</li>
<li><a href="https://github.com/serde-rs/json/commit/6a306e6ee9f47f3b37088217ffe3ebe9bbb54e5a"><code>6a306e6</code></a> Move call to tri! out of check_recursion!</li>
<li><a href="https://github.com/serde-rs/json/commit/3f1c6de4af28b1f6c5100da323f2bffaf7c2083f"><code>3f1c6de</code></a> Ignore byte_char_slices clippy lint in test</li>
<li><a href="https://github.com/serde-rs/json/commit/3fd6f5f49dc1c732d9b1d7dfece4f02c0d440d39"><code>3fd6f5f</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/json/issues/1153">#1153</a> from dpathakj/master</li>
<li><a href="https://github.com/serde-rs/json/commit/fcb5e83e44abe0f9c27c755a240a6ad56312c090"><code>fcb5e83</code></a> Correct documentation URL for Value's Index impl.</li>
<li>See full diff in <a href="https://github.com/serde-rs/json/compare/v1.0.120...v1.0.121">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=serde_json&package-manager=cargo&previous-version=1.0.120&new-version=1.0.121)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-29 16:48:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4911" class=".btn">#4911</a>
            </td>
            <td>
                <b>
                    chore(deps): bump tokio from 1.39.1 to 1.39.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [tokio](https://github.com/tokio-rs/tokio) from 1.39.1 to 1.39.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/tokio-rs/tokio/releases">tokio's releases</a>.</em></p>
<blockquote>
<h2>Tokio v1.39.2</h2>
<h1>1.39.2 (July 27th, 2024)</h1>
<p>This release fixes a regression where the <code>select!</code> macro stopped accepting expressions that make use of temporary lifetime extension. (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6722">#6722</a>)</p>
<p><a href="https://redirect.github.com/tokio-rs/tokio/issues/6722">#6722</a>: <a href="https://redirect.github.com/tokio-rs/tokio/pull/6722">tokio-rs/tokio#6722</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tokio-rs/tokio/commit/f602eae49988dbad2a11fd83e6b3fbd4f094713c"><code>f602eae</code></a> chore: prepare Tokio v1.39.2 (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6730">#6730</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/438def79579a7e285beb5f0d93b1eb6a9f8062b3"><code>438def7</code></a> macros: allow temporary lifetime extension in select (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6722">#6722</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/ee8d4d1b0546c67198af3cd053d6b7b8b4fd26c3"><code>ee8d4d1</code></a> chore: fix ci failures (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6725">#6725</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/32970527633bb72fc4f01d02523484a9376ac26a"><code>3297052</code></a> ci: test Quinn in CI (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6719">#6719</a>)</li>
<li>See full diff in <a href="https://github.com/tokio-rs/tokio/compare/tokio-1.39.1...tokio-1.39.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tokio&package-manager=cargo&previous-version=1.39.1&new-version=1.39.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-29 16:46:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4909" class=".btn">#4909</a>
            </td>
            <td>
                <b>
                    fix: prevent redundant blocksync block messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

There was a problem during TPS testing where block sync could not occur quickly because it would re-request the
same blocks from each peer. Here is a solution that should be robust against that scenario but doesn't introduce
any new issues.

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-27 14:18:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4904" class=".btn">#4904</a>
            </td>
            <td>
                <b>
                    chore(deps): bump iroha_schema_gen from 2.0.0-pre-rc.21 to 2.0.0-pre-rc.22.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps iroha_schema_gen from 2.0.0-pre-rc.21 to 2.0.0-pre-rc.22.0.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=iroha_schema_gen&package-manager=cargo&previous-version=2.0.0-pre-rc.21&new-version=2.0.0-pre-rc.22.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-26 16:20:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4903" class=".btn">#4903</a>
            </td>
            <td>
                <b>
                    fix(client): Fix torii url with path
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">config-changes</span>
            </td>
            <td>
                ## Description

Consider `client.toml`:
```toml
torii_url = "http://iroha-test.com/peer-1/"
```
Currently `/peer-1/` part will be ignored and queries will be send to `http://iroha-test.com/query`. This PR fixes it

### Benefits

Fix using `torii_url` with path in `client.toml`

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-26 14:20:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4899" class=".btn">#4899</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump pytest from 8.3.1 to 8.3.2 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.3.1 to 8.3.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>8.3.2</h2>
<h1>pytest 8.3.2 (2024-07-24)</h1>
<h2>Bug fixes</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12652">#12652</a>: Resolve regression [conda]{.title-ref} environments where no longer being automatically detected.</p>
<p>-- by <code>RonnyPfannschmidt</code>{.interpreted-text role=&quot;user&quot;}</p>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/bbcec9c46509c417ef58e4849847b4aa43f4591e"><code>bbcec9c</code></a> Prepare release version 8.3.2</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/78fe8b61fa716cd9775f1e37b395bab7679734a6"><code>78fe8b6</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12657">#12657</a> from pytest-dev/patchback/backports/8.3.x/6c806b499...</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/238bad2d2a1f1dbb47d740c84b5b4f5224f8a965"><code>238bad2</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12656">#12656</a> from RonnyPfannschmidt/fix-12652-detect-conda-env</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/ae6034a781a50b572fa700911e5d8e0eb074ca17"><code>ae6034a</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12641">#12641</a> from pytest-dev/patchback/backports/8.3.x/c03989cee...</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/31337aba02a7698a87a6792eacf887fceff08af2"><code>31337ab</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12640">#12640</a> from pytest-dev/update-user</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/ca3070b1356e5edf43f085d8c4ec1b34627061dd"><code>ca3070b</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12637">#12637</a> from pytest-dev/release-8.3.1</li>
<li>See full diff in <a href="https://github.com/pytest-dev/pytest/compare/8.3.1...8.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=8.3.1&new-version=8.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-25 17:06:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4897" class=".btn">#4897</a>
            </td>
            <td>
                <b>
                    chore(deps): bump clap from 4.5.10 to 4.5.11
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [clap](https://github.com/clap-rs/clap) from 4.5.10 to 4.5.11.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/clap-rs/clap/blob/master/CHANGELOG.md">clap's changelog</a>.</em></p>
<blockquote>
<h2>[4.5.11] - 2024-07-25</h2>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/clap-rs/clap/compare/clap_complete-v4.5.10...v4.5.11">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=clap&package-manager=cargo&previous-version=4.5.10&new-version=4.5.11)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-25 16:09:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4896" class=".btn">#4896</a>
            </td>
            <td>
                <b>
                    chore(deps): bump toml from 0.8.15 to 0.8.16
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [toml](https://github.com/toml-rs/toml) from 0.8.15 to 0.8.16.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/toml-rs/toml/commit/4ac61f76176cb028207096cbc6dd7263e6f120b1"><code>4ac61f7</code></a> chore: Release</li>
<li><a href="https://github.com/toml-rs/toml/commit/a5eb1ac08508b7a0b771b01231356b1591a27c1b"><code>a5eb1ac</code></a> chore: Disable serde_toml releasing for now</li>
<li>See full diff in <a href="https://github.com/toml-rs/toml/compare/toml-v0.8.15...toml-v0.8.16">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=toml&package-manager=cargo&previous-version=0.8.15&new-version=0.8.16)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-25 16:07:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4894" class=".btn">#4894</a>
            </td>
            <td>
                <b>
                    refactor: remove dependency on iroha_wasm_builder from iroha cli and client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                

## Description

We had some unnecessary dependencies on `iroha_wasm_builder`, blocking the build of iroha cli and client. This PR removes those and makes it so only the `iroha_wasm_builder` cli and integration tests actually depend on the crate.

As a part of this change, `construct_executor` utility function is moved from `iroha_cli` to `test_network`, as it only gets used in tests. Not _entirely_ happy with its new location, but `iroha_cli` is definitely a worse place for this.

### Linked issue

Closes #4882

### Benefits

Hopefully, faster incremental builds in cases when integration tests are not being built.

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-25 15:59:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4893" class=".btn">#4893</a>
            </td>
            <td>
                <b>
                    fix: Add limits to LiveQueryStore to prevent high memory usage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span><span class="chip">config-changes</span>
            </td>
            <td>
                ## Description

Added two new config parameters which limits number of live queries (global and per-user). Default value for both is 128. This is needed to prevent high memory usage in cases when client sends a lot of queries with large output, but do not fully consume those queries (that is obtain only first batch and doesn't send requests for the next batches). Normally clients should not do this, but malicious third-party can send such requests to DDOS iroha peer. In case limits are exceeded, iroha peer will return error "429 too many requests" for the query request.

* Names of parameters:
```toml
[torii]
query_store_capacity = 128
query_store_capacity_per_user = 128
```

Also:
* Changed default value of query idle time from 30s to 10s (for the same reason to decrease potential peak memory usage)
* Changed default value of fetch size from 10 to 100 (I think it is strange that when query output has e.g. 1000 items, client currently has to send 100 requests to get full query result)

Some notes about implementation:
* Currently when adding new query, the message is send to `mpsc::channel`, and `LiveQueryStore` thread does the addition. I changed it to perform addition directly without `mpsc::channel` since we now need to check capacity and return error to client if it exceeds.

### Linked issue

Closes #4830

### Benefits

Add limit to number of live queries to prevent high memory usage in cases when client don't fully consume query output.

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-25 15:43:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4891" class=".btn">#4891</a>
            </td>
            <td>
                <b>
                    chore: version bump to RC22
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-25 07:56:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4890" class=".btn">#4890</a>
            </td>
            <td>
                <b>
                    refactor: derive block hash from header
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

Derive block hash from the header only.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4641 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

- block hash is the same for the whole lifetime of the block
- block hash is less expensive as only header is used
- light client is able to verify block chain by only headers and corresponding signatures (without obligation to load the whole block)

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-24 13:10:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4889" class=".btn">#4889</a>
            </td>
            <td>
                <b>
                    refactor(p2p): remove `garbage`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

Remove adding garbage to p2p handshake.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4888 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

No redundant code.

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-24 10:18:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4886" class=".btn">#4886</a>
            </td>
            <td>
                <b>
                    fix(schema): make `Role` transparent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
            </td>
            <td>
                ## Description

* make `Role` transparent in schema
* rename `NewXXX` to `XXX` when serializing as json

This is how schema looked like:
```json
"NewRole": {
  "Struct": [
    {
      "name": "inner",
      "type": "Role"
    }
  ]
},
```

but in genesis it was:
```json
{
  "Register": {
    "Role": {
      "id": "ALICE_METADATA_ACCESS",
      "permissions": [
        {
          "name": "CanRemoveKeyValueInAccount",
          "payload": {
            "account": "ed0120CE7FA46C9DCE7EA4B125E2E36BDB63EA33073E7590AC92816AE1E861B7048B03@wonderland"
          }
        },
        {
          "name": "CanSetKeyValueInAccount",
          "payload": {
            "account": "ed0120CE7FA46C9DCE7EA4B125E2E36BDB63EA33073E7590AC92816AE1E861B7048B03@wonderland"
          }
        }
      ]
    }
  }
},
```

which is the consequence of the fact that we have no way of representing transparency in schema

### Linked issue

Related to #1660 

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-23 17:41:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4885" class=".btn">#4885</a>
            </td>
            <td>
                <b>
                    chore(deps): bump tokio from 1.38.1 to 1.39.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [tokio](https://github.com/tokio-rs/tokio) from 1.38.1 to 1.39.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/tokio-rs/tokio/releases">tokio's releases</a>.</em></p>
<blockquote>
<h2>Tokio v1.39.1</h2>
<h1>1.39.1 (July 23rd, 2024)</h1>
<p>This release reverts &quot;time: avoid traversing entries in the time wheel twice&quot; because it contains a bug. (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6715">#6715</a>)</p>
<p><a href="https://redirect.github.com/tokio-rs/tokio/issues/6715">#6715</a>: <a href="https://redirect.github.com/tokio-rs/tokio/pull/6715">tokio-rs/tokio#6715</a></p>
<h2>Tokio v1.39.0</h2>
<h1>1.39.0 (July 23rd, 2024)</h1>
<ul>
<li>This release bumps the MSRV to 1.70. (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6645">#6645</a>)</li>
<li>This release upgrades to mio v1. (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6635">#6635</a>)</li>
<li>This release upgrades to windows-sys v0.52 (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6154">#6154</a>)</li>
</ul>
<h3>Added</h3>
<ul>
<li>io: implement <code>AsyncSeek</code> for <code>Empty</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6663">#6663</a>)</li>
<li>metrics: stabilize <code>num_alive_tasks</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6619">#6619</a>, <a href="https://redirect.github.com/tokio-rs/tokio/issues/6667">#6667</a>)</li>
<li>process: add <code>Command::as_std_mut</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6608">#6608</a>)</li>
<li>sync: add <code>watch::Sender::same_channel</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6637">#6637</a>)</li>
<li>sync: add <code>{Receiver,UnboundedReceiver}::{sender_strong_count,sender_weak_count}</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6661">#6661</a>)</li>
<li>sync: implement <code>Default</code> for <code>watch::Sender</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6626">#6626</a>)</li>
<li>task: implement <code>Clone</code> for <code>AbortHandle</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6621">#6621</a>)</li>
<li>task: stabilize <code>consume_budget</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6622">#6622</a>)</li>
</ul>
<h3>Changed</h3>
<ul>
<li>io: improve panic message of <code>ReadBuf::put_slice()</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6629">#6629</a>)</li>
<li>io: read during write in <code>copy_bidirectional</code> and <code>copy</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6532">#6532</a>)</li>
<li>runtime: replace <code>num_cpus</code> with <code>available_parallelism</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6709">#6709</a>)</li>
<li>task: avoid stack overflow when passing large future to <code>block_on</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6692">#6692</a>)</li>
<li>time: avoid traversing entries in the time wheel twice (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6584">#6584</a>)</li>
<li>time: support <code>IntoFuture</code> with <code>timeout</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6666">#6666</a>)</li>
<li>macros: support <code>IntoFuture</code> with <code>join!</code> and <code>select!</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6710">#6710</a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>docs: fix docsrs builds with the fs feature enabled (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6585">#6585</a>)</li>
<li>io: only use short-read optimization on known-to-be-compatible platforms (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6668">#6668</a>)</li>
<li>time: fix overflow panic when using large durations with <code>Interval</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6612">#6612</a>)</li>
</ul>
<h3>Added (unstable)</h3>
<ul>
<li>macros: allow <code>unhandled_panic</code> behavior for <code>#[tokio::main]</code> and <code>#[tokio::test]</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6593">#6593</a>)</li>
<li>metrics: add <code>spawned_tasks_count</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6114">#6114</a>)</li>
<li>metrics: add <code>worker_park_unpark_count</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6696">#6696</a>)</li>
<li>metrics: add worker thread id (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6695">#6695</a>)</li>
</ul>
<h3>Documented</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tokio-rs/tokio/commit/f8fe0ffb23c2279708cb5dada7c88defdae60845"><code>f8fe0ff</code></a> chore: prepare Tokio v1.39.1 (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6716">#6716</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/47210a8e6eeb82b51aa778074fdc4d757b953b8c"><code>47210a8</code></a> time: revert &quot;avoid traversing entries in the time wheel twice&quot; (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6715">#6715</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/29545d90370d925a7264ff8636013ee6bf1760e6"><code>29545d9</code></a> runtime: ignore many_oneshot_futures test for alt scheduler (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6712">#6712</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/48e35c11d924ffa3a009b89fbb6d36e57b835da4"><code>48e35c1</code></a> chore: release Tokio v1.39.0 (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6711">#6711</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/dd1d37167d1f4008ca5d3df500e86826112a8cad"><code>dd1d371</code></a> macros: accept <code>IntoFuture</code> args for macros (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6710">#6710</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/6a1a7b15912d1a86ab4c0d09e1a8f0a221dbfeee"><code>6a1a7b1</code></a> chore: prepare tokio-macros v2.4.0 (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6707">#6707</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/51b03f0334a79298c942c123eb99ebf8daac0352"><code>51b03f0</code></a> deps: update to windows-sys v0.52 (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6154">#6154</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/754a1fb03c7456682a652f66eba6d76cfa1c6ad8"><code>754a1fb</code></a> deps: update to Mio v1 (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6635">#6635</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/90b23a9584db99ae81fffee38a89a09d2eca1834"><code>90b23a9</code></a> metrics: add worker thread id (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6695">#6695</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/b69f16aa219818bc75e7ae6a22631d4e574efd39"><code>b69f16a</code></a> metrics: add <code>worker_park_unpark_count</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6696">#6696</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/tokio-rs/tokio/compare/tokio-1.38.1...tokio-1.39.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tokio&package-manager=cargo&previous-version=1.38.1&new-version=1.39.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-23 16:31:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4884" class=".btn">#4884</a>
            </td>
            <td>
                <b>
                    chore(deps): bump clap from 4.5.9 to 4.5.10
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [clap](https://github.com/clap-rs/clap) from 4.5.9 to 4.5.10.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/clap-rs/clap/releases">clap's releases</a>.</em></p>
<blockquote>
<h2>v4.5.10</h2>
<h2>[4.5.10] - 2024-07-23</h2>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/clap-rs/clap/blob/master/CHANGELOG.md">clap's changelog</a>.</em></p>
<blockquote>
<h2>[4.5.10] - 2024-07-23</h2>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/clap-rs/clap/commit/6243d6546301855c6fc71680e2bf6976f064aee1"><code>6243d65</code></a> fix: Only generate stubs if has subcommands</li>
<li><a href="https://github.com/clap-rs/clap/commit/f5965e586292d31b2a2cbd83f19d145180471012"><code>f5965e5</code></a> chore: Update dependencies</li>
<li>See full diff in <a href="https://github.com/clap-rs/clap/compare/clap_complete-v4.5.9...v4.5.10">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=clap&package-manager=cargo&previous-version=4.5.9&new-version=4.5.10)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-23 16:29:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4881" class=".btn">#4881</a>
            </td>
            <td>
                <b>
                    ci: containerised testing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-23 11:50:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4880" class=".btn">#4880</a>
            </td>
            <td>
                <b>
                    refactor: remove committed_topology from block
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span><span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

- committed topology is removed from block
- committed topology for latest and previous blocks are stored in the state
    - it's required for blocks sync
    - and for initializing state from the snapshot + block store
- initial topology in the genesis block is passed as transaction with `Register<Peer>` instructions
- trusted peers are removed from `World` constructor

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4879 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Less space used in the block store, easier to derive block hash.

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### How to test

Run, try to submit new blocks, try restart peers check that iroha operates as usual.

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-23 11:23:38 +0000 UTC
    </div>
</div>

