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
                PR <a href="https://github.com/hyperledger/iroha/pull/4927" class=".btn">#4927</a>
            </td>
            <td>
                <b>
                    chore(deps): bump faker from 26.0.0 to 26.1.0 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [faker](https://github.com/joke2k/faker) from 26.0.0 to 26.1.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/joke2k/faker/releases">faker's releases</a>.</em></p>
<blockquote>
<h2>Release v26.1.0</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v26.1.0/CHANGELOG.md">CHANGELOG.md</a>.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/joke2k/faker/blob/master/CHANGELOG.md">faker's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/joke2k/faker/compare/v26.0.0...v26.1.0">v26.1.0 - 2024-08-01</a></h3>
<ul>
<li>Add more entries to <code>sk_SK</code> Geo provider. Thanks <a href="https://github.com/george0st"><code>@​george0st</code></a>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/joke2k/faker/commit/754f979dfad93a6270d947a001da2ebed59512c5"><code>754f979</code></a> Bump version: 26.0.0 → 26.1.0</li>
<li><a href="https://github.com/joke2k/faker/commit/c78edc4b570d59977f6e5fe85899be765bf97b41"><code>c78edc4</code></a> :pencil: Update CHANGELOG.md</li>
<li><a href="https://github.com/joke2k/faker/commit/001ac36975808290784416c8a1042444d15f09fb"><code>001ac36</code></a> fix typing</li>
<li><a href="https://github.com/joke2k/faker/commit/f9b4ead111cacf4da386951b71c6da6efdd5337a"><code>f9b4ead</code></a> Add more entries to <code>sk_SK</code> Geo provider (<a href="https://redirect.github.com/joke2k/faker/issues/2060">#2060</a>)</li>
<li>See full diff in <a href="https://github.com/joke2k/faker/compare/v26.0.0...v26.1.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=faker&package-manager=pip&previous-version=26.0.0&new-version=26.1.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-08-01 17:05:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4924" class=".btn">#4924</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump mypy from 1.11.0 to 1.11.1 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [mypy](https://github.com/python/mypy) from 1.11.0 to 1.11.1.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/python/mypy/commit/570b90a7a368f04c64f60af339d0ac1808c49c15"><code>570b90a</code></a> Bump version to 1.11</li>
<li><a href="https://github.com/python/mypy/commit/b3a102ef31f63a8a8ba32c8dbe160ddef3c43054"><code>b3a102e</code></a> Fix <code>RawExpressionType.accept</code> crash with <code>--cache-fine-grained</code> (<a href="https://redirect.github.com/python/mypy/issues/17588">#17588</a>)</li>
<li><a href="https://github.com/python/mypy/commit/aec04c74488d46a81a95ed3553b8e953a6ec59a7"><code>aec04c7</code></a> Fix PEP 604 isinstance caching (<a href="https://redirect.github.com/python/mypy/issues/17563">#17563</a>)</li>
<li><a href="https://github.com/python/mypy/commit/cb44e4d8f18b9bc874f1076b33eec7ad67de165c"><code>cb44e4d</code></a> Fix <code>typing.TypeAliasType</code> being undefined on python &lt; 3.12 (<a href="https://redirect.github.com/python/mypy/issues/17558">#17558</a>)</li>
<li><a href="https://github.com/python/mypy/commit/6cf9180e1411dab2ee91b57374f696d391eb24f4"><code>6cf9180</code></a> Fix types.GenericAlias lookup crash (<a href="https://redirect.github.com/python/mypy/issues/17543">#17543</a>)</li>
<li><a href="https://github.com/python/mypy/commit/64c1ebf7cff51c13b1771174e3bb6bce9fe0d5dc"><code>64c1ebf</code></a> Bump version to 1.11.1+dev</li>
<li>See full diff in <a href="https://github.com/python/mypy/compare/v1.11...v1.11.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=mypy&package-manager=pip&previous-version=1.11.0&new-version=1.11.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-31 16:31:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4923" class=".btn">#4923</a>
            </td>
            <td>
                <b>
                    fix(p2p): prevent deadlock on simultaneous sending large message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span>
            </td>
            <td>
                ## Description

When 2 peers try to send each other huge messages they end up deadlocked.
I suspect that this happen when message is large enough that it's not possible to fully put it in the OS buffer.

Here is minimal [example](https://github.com/Erigara/tcp_deadlock) i was able to came up with which suffers from the same issue.

Solution was to lift sending data up to the `select!` statement so peer can either read or write data simultaneously. 

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

No deadlock.

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
        Created At 2024-07-31 14:49:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4922" class=".btn">#4922</a>
            </td>
            <td>
                <b>
                    fix(sumeragi): remove expired transaction from cache
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span>
            </td>
            <td>
                ## Description

- fix a bug in retain that actually non expired transactions were removed
- qol improvment to print transactions by hash in the logs
    - i find it really hard to debug iroha on TRACE level in presence of heavy transactions because all logs are polluted by tx printing 

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

- fewer bugs
- more clear logs

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
        Created At 2024-07-31 07:18:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4921" class=".btn">#4921</a>
            </td>
            <td>
                <b>
                    fix: prevent redundant blocksync block messages - backport to rc22
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
        Created At 2024-07-31 00:24:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4920" class=".btn">#4920</a>
            </td>
            <td>
                <b>
                    chore: version bump to rc.1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Current version should be whatever we're currently working on. 
In this case it should be `rc.1` and not `rc.22` which we have already released

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
        Created At 2024-07-30 16:50:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4919" class=".btn">#4919</a>
            </td>
            <td>
                <b>
                    ci: Add jq tool to iroha2 profiler image
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
        Created At 2024-07-30 15:15:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4918" class=".btn">#4918</a>
            </td>
            <td>
                <b>
                    ci: Implement Containerized Testing
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

Closes #4925 <!-- Replace with an actual number,  -->

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
        Created At 2024-07-30 14:56:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4917" class=".btn">#4917</a>
            </td>
            <td>
                <b>
                    fix: delete exited colleges
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
        Created At 2024-07-30 14:46:32 +0000 UTC
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

