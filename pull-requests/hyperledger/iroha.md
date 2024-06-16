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
                PR <a href="https://github.com/hyperledger/iroha/pull/4734" class=".btn">#4734</a>
            </td>
            <td>
                <b>
                    refactor: Make domain structure shallow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
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
        Created At 2024-06-15 22:27:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4732" class=".btn">#4732</a>
            </td>
            <td>
                <b>
                    refactor: Metadata became dynamic and consists of JsonString
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
            </td>
            <td>
                ## Description

* Removed MetadataValueBox
* Added JsonString

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

* Closes #4353  <!-- Replace with an actual number,  -->

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
        Created At 2024-06-14 09:56:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4731" class=".btn">#4731</a>
            </td>
            <td>
                <b>
                    fix!: remove on-chain parameters from config and remove NewParameter ISI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span><span class="chip">config-changes</span>
            </td>
            <td>
                ## Description

* remove `NewParametere` ISI
* remove on-chain parameters from configuration
* strong type on-chain parameters
* removed `MetadataLimits` and `LenghtLimits` as built-in on-chain parameters (they can be defined as custom)

Next PR will introduce Custom parameters

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
        Created At 2024-06-14 09:35:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4730" class=".btn">#4730</a>
            </td>
            <td>
                <b>
                    fix: update schema.json
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Add missing types into the schema.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-14 08:58:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4728" class=".btn">#4728</a>
            </td>
            <td>
                <b>
                    fix: Introduce p2p idle timeout
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Backport of #4398.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4267 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

No problem with connectivity on rc20.

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
        Created At 2024-06-13 14:20:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4725" class=".btn">#4725</a>
            </td>
            <td>
                <b>
                    fix: Make `iroha_smart_contract_utils` `log` and `dbg` functions work outside of wasm
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

This PR adds support for `iroha_smart_contract_utils`'s `log` and `dbg` functions to be used outside of wasm. This allows writing tests to be ran against the host target and to still use those wasm-specific functions.

Both implementations just print the requested object to stderr.

As a drive-by, this also makes sure to run wasm tests from `iroha_smart_contract_utils`, which was omitted in CI for some time.

### Linked issue

Fixes #4721

### Benefits

- [ ] make CI pass

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-13 11:56:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4724" class=".btn">#4724</a>
            </td>
            <td>
                <b>
                    refactor(genesis)!: remove _id and _file suffix from genesis fields
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
        Created At 2024-06-13 11:00:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4723" class=".btn">#4723</a>
            </td>
            <td>
                <b>
                    fix(swarm): remove `_id` suffix from docker-compose files
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
        Created At 2024-06-13 10:57:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4719" class=".btn">#4719</a>
            </td>
            <td>
                <b>
                    feat(swarm): reimplement, optimize compose config and its generation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Reimplement most of Swarm generation logic, optimize the generated Compose config.

### Benefits

- declutters schema code
- removes almost all clones
- optimizes Compose config: builds/pulls image only once instead of per peer (this has caused sigkills during builds)
- allows writing to any `std::io::Write` instead of just files
  - adds an option to print the config to stdout (used in CI to check config updates)

### Checklist

- [x] I've written unit tests for the code changes=
- [x] Update usage of Swarm in CI
- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-11 16:05:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4718" class=".btn">#4718</a>
            </td>
            <td>
                <b>
                    refactor: migrate to axum
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
            </td>
            <td>
                ## Description

Migrate from `warp` to `axum`.

With current implementation i tried to preserve the same behavior as before.

I would suggest further improvements in the separate PRs.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3776  <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Bring more simplicity to torii.

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
        Created At 2024-06-11 14:25:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4716" class=".btn">#4716</a>
            </td>
            <td>
                <b>
                    refactor: supervise spawned tasks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">api-changes</span><span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

This PR introduces a lightweight `Supervisor` for Tokio tasks.

What it does:

- Monitors multiple children
- Provides a single shutdown signal for everything
- Supports graceful shutdown timeout before aborting a child
- If a child panics, initiates shutdown and exits with an error
- If a child exits _before_ shutdown signal, also initiates shutdown and exits with an error. **Note:** this might not be always the desirable behaviour, but _currently_ there are no other cases in Iroha. This behaviour could be easily extended to support refined per-child strategies.
- Logs children's lifecycle and panics

What it doesn't:

- Doesn't support restarting children. To implement that, we need a formal actor system.

### Linked issue

Closes #4698
Related to #4516 (helps to identify failures)

### Benefits

- Clearer shutdown traces
- Clearer Iroha lifecycle
- Less unnoticed panics

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-11 02:55:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4715" class=".btn">#4715</a>
            </td>
            <td>
                <b>
                    chore(deps): bump faker from 25.5.0 to 25.8.0 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [faker](https://github.com/joke2k/faker) from 25.5.0 to 25.8.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/joke2k/faker/releases">faker's releases</a>.</em></p>
<blockquote>
<h2>Release v25.8.0</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v25.8.0/CHANGELOG.md">CHANGELOG.md</a>.</p>
<h2>Release v25.7.0</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v25.7.0/CHANGELOG.md">CHANGELOG.md</a>.</p>
<h2>Release v25.6.0</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v25.6.0/CHANGELOG.md">CHANGELOG.md</a>.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/joke2k/faker/blob/master/CHANGELOG.md">faker's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/joke2k/faker/compare/v25.7.0..v25.8.0">v25.8.0 - 2024-05-07</a></h3>
<ul>
<li>Add handshake emoji with different color variations to emoji provider list. Thanks <a href="https://github.com/tamkc"><code>@​tamkc</code></a>.</li>
</ul>
<h3><a href="https://github.com/joke2k/faker/compare/v25.6.0..v25.7.0">v25.7.0 - 2024-05-07</a></h3>
<ul>
<li>Add missing translation for countries in <code>pt-BR</code>. Thanks <a href="https://github.com/LeonardoFurtado"><code>@​LeonardoFurtado</code></a>.</li>
</ul>
<h3><a href="https://github.com/joke2k/faker/compare/v25.5.0...v25.6.0">v25.6.0 - 2024-05-06</a></h3>
<ul>
<li>Fix data in geo for <code>pl_PL</code>. Thanks <a href="https://github.com/george0st"><code>@​george0st</code></a>, <a href="https://github.com/mgorny"><code>@​mgorny</code></a>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/joke2k/faker/commit/cf60c42dbfbb202e6d55c43057455530bf1edd1e"><code>cf60c42</code></a> Bump version: 25.7.0 → 25.8.0</li>
<li><a href="https://github.com/joke2k/faker/commit/cbdeb1c37c8e9f0d4227301baa0f4466e7c376b9"><code>cbdeb1c</code></a> :pencil: Update CHANGELOG.md</li>
<li><a href="https://github.com/joke2k/faker/commit/e2d94bfbbc321b4dc6367648ed8255dc07bc6795"><code>e2d94bf</code></a> Add handshake emoji with different color variations to emoji provider list (#...</li>
<li><a href="https://github.com/joke2k/faker/commit/aa64332a1dd87adcd439d326197b47898c28caab"><code>aa64332</code></a> Bump version: 25.6.0 → 25.7.0</li>
<li><a href="https://github.com/joke2k/faker/commit/4d63c7d6ec59ac2cdccea6d772323daacc8addf1"><code>4d63c7d</code></a> :pencil: Update CHANGELOG.md</li>
<li><a href="https://github.com/joke2k/faker/commit/ac86040d87c6ffdc5621cdb3f33a068b216f63e6"><code>ac86040</code></a> Add missing translation for countries in <code>pt-BR</code>. (<a href="https://redirect.github.com/joke2k/faker/issues/2049">#2049</a>)</li>
<li><a href="https://github.com/joke2k/faker/commit/9b1c0d271470f1475664d07c70c0bf7712b5c265"><code>9b1c0d2</code></a> Bump version: 25.5.0 → 25.6.0</li>
<li><a href="https://github.com/joke2k/faker/commit/7a523b2e6ccfabbe362aa223b12c74a033969b17"><code>7a523b2</code></a> :pencil: Update CHANGELOG.md</li>
<li><a href="https://github.com/joke2k/faker/commit/3ad60494991c99e6976dcd9a62d0f396a85a25f7"><code>3ad6049</code></a> Update <strong>init</strong>.py</li>
<li><a href="https://github.com/joke2k/faker/commit/1e61099ba19c9af48f8ff74d90f6d36d0439c8f9"><code>1e61099</code></a> More fixes for the <code>geo/pl_PL</code> provider (<a href="https://redirect.github.com/joke2k/faker/issues/2057">#2057</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/joke2k/faker/compare/v25.5.0...v25.8.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=faker&package-manager=pip&previous-version=25.5.0&new-version=25.8.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-10 17:00:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4714" class=".btn">#4714</a>
            </td>
            <td>
                <b>
                    refactor!: remove `_id` suffix for entity ids in public API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span><span class="chip">config-changes</span>
            </td>
            <td>
                ## Description

Remove `_id` suffix from tokens, config files and data model

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
        Created At 2024-06-10 16:37:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4713" class=".btn">#4713</a>
            </td>
            <td>
                <b>
                    chore(deps): bump url from 2.5.0 to 2.5.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [url](https://github.com/servo/rust-url) from 2.5.0 to 2.5.1.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/servo/rust-url/commit/3d6dbbb1dfc64c597745d5d6b97f2a8dd543c42b"><code>3d6dbbb</code></a> Reimplement idna on top of ICU4X (<a href="https://redirect.github.com/servo/rust-url/issues/923">#923</a>)</li>
<li><a href="https://github.com/servo/rust-url/commit/de947abf896f44efc5f0fe382064fd95363dff37"><code>de947ab</code></a> Document possible replacements of the base URL (<a href="https://redirect.github.com/servo/rust-url/issues/926">#926</a>)</li>
<li><a href="https://github.com/servo/rust-url/commit/8b8431bbe10d0f06c53885d5ba2602d69f61888f"><code>8b8431b</code></a> docs: document SyntaxViolation variants, remove bare URLs (<a href="https://redirect.github.com/servo/rust-url/issues/924">#924</a>)</li>
<li><a href="https://github.com/servo/rust-url/commit/fd042e003fe583426454001554542ef95538d794"><code>fd042e0</code></a> Non-special URLs can have their paths erased (<a href="https://redirect.github.com/servo/rust-url/issues/921">#921</a>)</li>
<li><a href="https://github.com/servo/rust-url/commit/49eea1c2eb3bb7259e3f8e15ace5f86990adb0bd"><code>49eea1c</code></a> Fix multiple issues on wasm32: (<a href="https://redirect.github.com/servo/rust-url/issues/886">#886</a>)</li>
<li><a href="https://github.com/servo/rust-url/commit/a4dd58be5989afedddec023174b2cdcd81912239"><code>a4dd58b</code></a> Fix lint (<a href="https://redirect.github.com/servo/rust-url/issues/920">#920</a>)</li>
<li><a href="https://github.com/servo/rust-url/commit/73803fa780c8890e0b40cd01fbbd5362fbe4c9e0"><code>73803fa</code></a> Update URLs (<a href="https://redirect.github.com/servo/rust-url/issues/916">#916</a>)</li>
<li><a href="https://github.com/servo/rust-url/commit/8e4331d26018d3c46a42f81b5613fcc7ab16b850"><code>8e4331d</code></a> Add bench for to_ascii on an already-Punycode name (<a href="https://redirect.github.com/servo/rust-url/issues/915">#915</a>)</li>
<li><a href="https://github.com/servo/rust-url/commit/9c51937adba5f5f54117999a6a7983b00a049995"><code>9c51937</code></a> Rename <code>master</code> branch to <code>main</code> (<a href="https://redirect.github.com/servo/rust-url/issues/914">#914</a>)</li>
<li><a href="https://github.com/servo/rust-url/commit/e654efb9c19732f680f14db43a673a726b834f42"><code>e654efb</code></a> Fix non-base64 data URLs with % character not followed by hex digits (<a href="https://redirect.github.com/servo/rust-url/issues/797">#797</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/servo/rust-url/compare/v2.5.0...v2.5.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=url&package-manager=cargo&previous-version=2.5.0&new-version=2.5.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-10 16:29:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4712" class=".btn">#4712</a>
            </td>
            <td>
                <b>
                    chore(deps): bump console-subscriber from 0.2.0 to 0.3.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [console-subscriber](https://github.com/tokio-rs/console) from 0.2.0 to 0.3.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/tokio-rs/console/releases">console-subscriber's releases</a>.</em></p>
<blockquote>
<h2>console-subscriber-v0.3.0 - (2024-06-10)</h2>
<h3><!-- raw HTML omitted --><!-- raw HTML omitted -->Breaking Changes</h3>
<ul>
<li><strong>Bump tonic to 0.11 (<a href="https://redirect.github.com/tokio-rs/console/pull/547">#547</a>)</strong> (<a href="https://github.com/tokio-rs/console/commit/ef6816caa0fe84171105b513425506f25d3082af">ef6816c</a>)<!-- raw HTML omitted -->This is a breaking change for users of <code>console-api</code> and
<code>console-subscriber</code>, as it changes the public <code>tonic</code> dependency to a
semver-incompatible version. This breaks compatibility with <code>tonic</code>
0.10.x.</li>
</ul>
<h3>Added</h3>
<ul>
<li>Replace target column with kind column in tasks view (<a href="https://redirect.github.com/tokio-rs/console/pull/478">#478</a>) (<a href="https://github.com/tokio-rs/console/commit/903d9fa9f9d2dddec2235206b792c264ed9892fb">903d9fa</a>)</li>
<li>Reduce retention period to fit in max message size (<a href="https://redirect.github.com/tokio-rs/console/pull/503">#503</a>) (<a href="https://github.com/tokio-rs/console/commit/bd3dd71eb0645c028858967ed5b3f14ed34d0605">bd3dd71</a>)</li>
<li>Support grpc-web and add <code>grpc-web</code> feature (<a href="https://redirect.github.com/tokio-rs/console/pull/498">#498</a>) (<a href="https://github.com/tokio-rs/console/commit/41502531396106b551a9dde2d3a83ddb0beac774">4150253</a>)</li>
</ul>
<h3>Documented</h3>
<ul>
<li>Add a grpc-web app example (<a href="https://redirect.github.com/tokio-rs/console/pull/526">#526</a>) (<a href="https://github.com/tokio-rs/console/commit/4af30f2c1df919a1e0d4f448534d15b4a1bb836b">4af30f2</a>)</li>
<li>Fix typo in doc comment (<a href="https://redirect.github.com/tokio-rs/console/pull/543">#543</a>) (<a href="https://github.com/tokio-rs/console/commit/ff2267880ba96f4fdf32090e05b66cf80189d7f8">ff22678</a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Don't save poll_ops if no-one is receiving them (<a href="https://redirect.github.com/tokio-rs/console/pull/501">#501</a>) (<a href="https://github.com/tokio-rs/console/commit/1656c791af35bb0500bb6dd3c60344a0ceb12520">1656c79</a>)</li>
<li>Ignore metadata that is not a span or event (<a href="https://redirect.github.com/tokio-rs/console/pull/554">#554</a>) (<a href="https://github.com/tokio-rs/console/commit/852a977bab71d0f6ae47c6c5c1c20b8679c9e576">852a977</a>)</li>
</ul>
<h3>Updated</h3>
<ul>
<li><a href="%5B#0%5D(https://redirect.github.com/tokio-rs/console/issues/0).3.0-breaking"><strong>breaking</strong></a> Bump tonic to 0.11 (<a href="https://redirect.github.com/tokio-rs/console/pull/547">#547</a>) (<a href="https://github.com/tokio-rs/console/commit/ef6816caa0fe84171105b513425506f25d3082af">ef6816c</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tokio-rs/console/commit/b802bf147bc0e54e01c7946e6ca67ff428eb4f86"><code>b802bf1</code></a> chore: release tokio-console-v0.1.11, console-api-v0.7.0, console-subscriber-...</li>
<li><a href="https://github.com/tokio-rs/console/commit/87ba91c9a5cd88037072f9758d9b94309c619164"><code>87ba91c</code></a> chore(console): update cargo dist (<a href="https://redirect.github.com/tokio-rs/console/issues/556">#556</a>)</li>
<li><a href="https://github.com/tokio-rs/console/commit/dcf8c2c73794cc92c78061316875f36ae2b7653b"><code>dcf8c2c</code></a> chore: include tonic updates in release notes (<a href="https://redirect.github.com/tokio-rs/console/issues/559">#559</a>)</li>
<li><a href="https://github.com/tokio-rs/console/commit/99437b012ac419150a96fe33ca66d2d481f6c51e"><code>99437b0</code></a> chore: automate releases with Release-plz (<a href="https://redirect.github.com/tokio-rs/console/issues/545">#545</a>)</li>
<li><a href="https://github.com/tokio-rs/console/commit/852a977bab71d0f6ae47c6c5c1c20b8679c9e576"><code>852a977</code></a> fix(subscriber): ignore metadata that is not a span or event (<a href="https://redirect.github.com/tokio-rs/console/issues/554">#554</a>)</li>
<li><a href="https://github.com/tokio-rs/console/commit/a0d20fd62df07470b6033524afc00a96d156aaa5"><code>a0d20fd</code></a> docs(console): add note about running on Windows (<a href="https://redirect.github.com/tokio-rs/console/issues/510">#510</a>)</li>
<li><a href="https://github.com/tokio-rs/console/commit/60bcf87537d414b21efbd84159207f9ecda5e914"><code>60bcf87</code></a> chore: get rid of remove_dir_all (<a href="https://redirect.github.com/tokio-rs/console/issues/542">#542</a>)</li>
<li><a href="https://github.com/tokio-rs/console/commit/1c1d599d5b741af89aef14889762ee3bf9c4e688"><code>1c1d599</code></a> chore: bump clap and clap_complete to the latest version (<a href="https://redirect.github.com/tokio-rs/console/issues/552">#552</a>)</li>
<li><a href="https://github.com/tokio-rs/console/commit/ef6816caa0fe84171105b513425506f25d3082af"><code>ef6816c</code></a> chore: bump tonic to 0.11 (<a href="https://redirect.github.com/tokio-rs/console/issues/547">#547</a>)</li>
<li><a href="https://github.com/tokio-rs/console/commit/6cbd6db7b50893c4d4f6b9f090be309fc0e34d8c"><code>6cbd6db</code></a> chore(console): bump ratatui to 0.26.2 and crossterm to 0.27.0 (<a href="https://redirect.github.com/tokio-rs/console/issues/515">#515</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/tokio-rs/console/compare/console-subscriber-v0.2.0...console-subscriber-v0.3.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=console-subscriber&package-manager=cargo&previous-version=0.2.0&new-version=0.3.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-10 16:28:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4711" class=".btn">#4711</a>
            </td>
            <td>
                <b>
                    chore(deps): bump clap from 4.5.4 to 4.5.7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [clap](https://github.com/clap-rs/clap) from 4.5.4 to 4.5.7.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/clap-rs/clap/releases">clap's releases</a>.</em></p>
<blockquote>
<h2>v4.5.7</h2>
<h2>[4.5.7] - 2024-06-10</h2>
<h3>Fixes</h3>
<ul>
<li>Clean up error message when too few arguments for <code>num_args</code></li>
</ul>
<h2>v4.5.6</h2>
<h2>[4.5.6] - 2024-06-06</h2>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/clap-rs/clap/blob/master/CHANGELOG.md">clap's changelog</a>.</em></p>
<blockquote>
<h2>[4.5.7] - 2024-06-10</h2>
<h3>Fixes</h3>
<ul>
<li>Clean up error message when too few arguments for <code>num_args</code></li>
</ul>
<h2>[4.5.6] - 2024-06-06</h2>
<h2>[4.5.5] - 2024-06-06</h2>
<h3>Fixes</h3>
<ul>
<li>Allow <code>exclusive</code> to override <code>required_unless_present</code>, <code>required_unless_present_any</code>, <code>required_unless_present_all</code></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/clap-rs/clap/commit/6c6839a454c2cbfc3007e6a2b2a55dd64685771e"><code>6c6839a</code></a> chore: Release</li>
<li><a href="https://github.com/clap-rs/clap/commit/e79ff0d42be524502cc9a59b6e1d4c669cb4c760"><code>e79ff0d</code></a> docs: Update changelog</li>
<li><a href="https://github.com/clap-rs/clap/commit/be2e5ca91e34c60333cc7c7e7daeaf457972c815"><code>be2e5ca</code></a> Merge pull request <a href="https://redirect.github.com/clap-rs/clap/issues/5527">#5527</a> from epage/min</li>
<li><a href="https://github.com/clap-rs/clap/commit/cf5c95862ecea004df7a8f44b234a959ea8ea36f"><code>cf5c958</code></a> fix(parser): Report correct num_args on too-few</li>
<li><a href="https://github.com/clap-rs/clap/commit/e0c9619c2796c9b7d784d4b8465b51c60756e05c"><code>e0c9619</code></a> test(parser): Snapshot num_args errors</li>
<li><a href="https://github.com/clap-rs/clap/commit/2f645d3e81c783a4e76ad17f1ccf283a58b75660"><code>2f645d3</code></a> chore: Release</li>
<li><a href="https://github.com/clap-rs/clap/commit/6e1e0368f9456eb85f232b4c72ccdf18b039947a"><code>6e1e036</code></a> docs: Update changelog</li>
<li><a href="https://github.com/clap-rs/clap/commit/7e1bbf82afd8dfd56926cbcdc687348086f9ade6"><code>7e1bbf8</code></a> Merge pull request <a href="https://redirect.github.com/clap-rs/clap/issues/5523">#5523</a> from ben--/zsh-colon</li>
<li><a href="https://github.com/clap-rs/clap/commit/8e3c273b611b5579699d4ddd0eada278f490798b"><code>8e3c273</code></a> fix(zsh): Separate options from _arguments options</li>
<li>See full diff in <a href="https://github.com/clap-rs/clap/compare/clap_complete-v4.5.4...v4.5.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=clap&package-manager=cargo&previous-version=4.5.4&new-version=4.5.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-10 16:27:42 +0000 UTC
    </div>
</div>

