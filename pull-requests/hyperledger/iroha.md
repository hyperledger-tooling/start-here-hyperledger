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
                PR <a href="https://github.com/hyperledger/iroha/pull/4706" class=".btn">#4706</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump pylint from 3.2.2 to 3.2.3 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pylint](https://github.com/pylint-dev/pylint) from 3.2.2 to 3.2.3.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pylint-dev/pylint/commit/918d2168e15662df90cfb993df100e566f69d418"><code>918d216</code></a> Bump pylint to 3.2.3, update changelog</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/8aba7d1ccca0552f2e47183bd748e4a535926b05"><code>8aba7d1</code></a> Fix false positive in <code>use-yield-from</code> when using <code>yield</code> return (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9700">#9700</a>) (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9701">#9701</a>)</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/192727b7b30c7fb4e261518a55b4fe75a1027b64"><code>192727b</code></a> [multiple-statements] Make pylint compatible with black's 2024 style (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9697">#9697</a>) ...</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/7e5e4f9a4bdca1af4f32f981d11ee42bfc6f5f3d"><code>7e5e4f9</code></a> Fix a false positive for <code>redefined-outer-name</code> (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9678">#9678</a>) (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9695">#9695</a>)</li>
<li>See full diff in <a href="https://github.com/pylint-dev/pylint/compare/v3.2.2...v3.2.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pylint&package-manager=pip&previous-version=3.2.2&new-version=3.2.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-06 16:10:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4705" class=".btn">#4705</a>
            </td>
            <td>
                <b>
                    fix: add missing getters for data model structs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Add missing getters.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4420 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Struct fields could be accessed from wasm or client.

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
        Created At 2024-06-06 13:49:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4701" class=".btn">#4701</a>
            </td>
            <td>
                <b>
                    refactor: remove index Assets in AssetsMap by AssetDefinitionId
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
            </td>
            <td>
                ## Description

AssetsMap stores assets for a particular account, so indexing them via AssetId (which is AccountId + AssetDefinitionId) is redundant

Also remove some unnecessary AccoundId clones

### Linked issue

Closes #4700

### Benefits

A bit more efficient, allows for more efficient implementations testing whether an account has some asset or not.

### Checklist

- [ ] make CI pass

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-06 10:44:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4699" class=".btn">#4699</a>
            </td>
            <td>
                <b>
                    refactor(irohad): always start torii as task
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

Simplify iroha startup + fix in integration test.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4562 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Simpler code.

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
        Created At 2024-06-06 08:56:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4697" class=".btn">#4697</a>
            </td>
            <td>
                <b>
                    refactor: fix application of the core chain-wide parameters; chores
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

While working on #4516, I experimented with extreme reduction of consensus timings, i.e. `block_time` and `commit_time`. Those are configured by `NewParameter` and `SetParameter` ISIs (until #4028). It turned out that there are a few issues in `iroha_core`:

- In some places it relies on hardcoded `DEFAULT_CONSENSUS_ESTIMATION` (4 seconds) for no reason, leading to some bugs, e.g. improper time triggers execution. I made it rely on the values in the actual State config.
- Config in the State was not updated immediately when relevant ISI executed, leading Iroha to ignore updates that actually affect its behaviour, which caused desynchronisation and unexpectedly long block times when the config values are small.

So, this PR "tightens" these gaps and makes parameters application preciser.

This PR doesn't introduce changes to the tests themselves, as I am still experimenting with it.

### Linked issue

None

### Benefits

More expected behaviour of the chain-wide parameters.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-06 02:12:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4695" class=".btn">#4695</a>
            </td>
            <td>
                <b>
                    chore(deps): bump cryptography from 42.0.7 to 42.0.8 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [cryptography](https://github.com/pyca/cryptography) from 42.0.7 to 42.0.8.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pyca/cryptography/blob/main/CHANGELOG.rst">cryptography's changelog</a>.</em></p>
<blockquote>
<p>42.0.8 - 2024-06-04</p>
<pre><code>
* Updated Windows, macOS, and Linux wheels to be compiled with OpenSSL 3.2.2.
<p>.. _v42-0-7:
</code></pre></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pyca/cryptography/commit/761ef4b955697c63e83734096f672224224082e1"><code>761ef4b</code></a> bump for 42.0.8 release (<a href="https://redirect.github.com/pyca/cryptography/issues/11072">#11072</a>)</li>
<li>See full diff in <a href="https://github.com/pyca/cryptography/compare/42.0.7...42.0.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=cryptography&package-manager=pip&previous-version=42.0.7&new-version=42.0.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-05 16:55:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4694" class=".btn">#4694</a>
            </td>
            <td>
                <b>
                    chore(deps): bump faker from 25.4.0 to 25.5.0 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [faker](https://github.com/joke2k/faker) from 25.4.0 to 25.5.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/joke2k/faker/releases">faker's releases</a>.</em></p>
<blockquote>
<h2>Release v25.5.0</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v25.5.0/CHANGELOG.md">CHANGELOG.md</a>.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/joke2k/faker/blob/master/CHANGELOG.md">faker's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/joke2k/faker/compare/v25.4.0...v25.5.0">v25.5.0 - 2024-05-04</a></h3>
<ul>
<li>Fix data in geo for <code>pl_PL</code>. Thanks <a href="https://github.com/george0st"><code>@​george0st</code></a>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/joke2k/faker/commit/cd2c4230cdbff4c19106f42dbd97eb1cb1c80cf7"><code>cd2c423</code></a> Bump version: 25.4.0 → 25.5.0</li>
<li><a href="https://github.com/joke2k/faker/commit/194ae15480814625e1bb4ca04611431426ddce00"><code>194ae15</code></a> :pencil: Update CHANGELOG.md</li>
<li><a href="https://github.com/joke2k/faker/commit/4213d3b949d01015abbb8642fddbbb8d45c6a0e5"><code>4213d3b</code></a> Fix data in geo for <code>pl_PL</code> (<a href="https://redirect.github.com/joke2k/faker/issues/2056">#2056</a>)</li>
<li><a href="https://github.com/joke2k/faker/commit/198df37fc314a67b4a6408fac69044c0d8370cef"><code>198df37</code></a> Update CONTRIBUTING.rst</li>
<li><a href="https://github.com/joke2k/faker/commit/35f87fd1bf9d8e505b979045a769b586a4816af1"><code>35f87fd</code></a> Update CONTRIBUTING.rst</li>
<li>See full diff in <a href="https://github.com/joke2k/faker/compare/v25.4.0...v25.5.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=faker&package-manager=pip&previous-version=25.4.0&new-version=25.5.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-05 16:55:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4693" class=".btn">#4693</a>
            </td>
            <td>
                <b>
                    refactor: Remove `GenesisNetwork`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Continuation of #4673.
`GenesisNetwork` always has exactly one `GenesisTransaction`, so it is worth to use `GenesisTransaction` directly

### Linked issue

### Benefits

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-05 14:32:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4692" class=".btn">#4692</a>
            </td>
            <td>
                <b>
                    fix: Correct default value for `JsonString`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span>
            </td>
            <td>
                ## Description

Set `"null"` as default value for `JsonString` instead of `""` which is not valid json.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4686 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

### How to test

```
cargo test --package iroha_core --lib -- snapshot::tests --show-output 
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-05 11:46:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4691" class=".btn">#4691</a>
            </td>
            <td>
                <b>
                    chore(deps): bump toml from 0.8.13 to 0.8.14
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [toml](https://github.com/toml-rs/toml) from 0.8.13 to 0.8.14.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/toml-rs/toml/commit/c383efa2a3b5ec2761c680773b3056c87f35f353"><code>c383efa</code></a> chore: Release</li>
<li><a href="https://github.com/toml-rs/toml/commit/7bb178167a4bf55be852bcf360bdb9389b9ad982"><code>7bb1781</code></a> docs: Update changelog</li>
<li><a href="https://github.com/toml-rs/toml/commit/0af6deb30b6c808ac589712d869177270ae99e09"><code>0af6deb</code></a> Merge pull request <a href="https://redirect.github.com/toml-rs/toml/issues/740">#740</a> from epage/key-quotes</li>
<li><a href="https://github.com/toml-rs/toml/commit/c9e36e7a0fe7fb3f7c25a6f217eeb0d1182eecc5"><code>c9e36e7</code></a> fix(encode): Prefer literals over escaping double-quotes</li>
<li><a href="https://github.com/toml-rs/toml/commit/42f7a1b3e92baf371c5e46c42fa48203870572d1"><code>42f7a1b</code></a> test(encode): Show existing quote behavior</li>
<li><a href="https://github.com/toml-rs/toml/commit/9e6290fc72a0f9cb983aa611c817ea09a3b711f7"><code>9e6290f</code></a> chore(deps): Update compatible (dev) (<a href="https://redirect.github.com/toml-rs/toml/issues/737">#737</a>)</li>
<li><a href="https://github.com/toml-rs/toml/commit/dbf1cc188082f2e537ffca1a6df7a2bf81444899"><code>dbf1cc1</code></a> Merge pull request <a href="https://redirect.github.com/toml-rs/toml/issues/736">#736</a> from epage/snapbox</li>
<li><a href="https://github.com/toml-rs/toml/commit/ec9bfd71ac4e58b5d7e44f823ce70b257c741b50"><code>ec9bfd7</code></a> chore: Update to snapbox 0.6</li>
<li><a href="https://github.com/toml-rs/toml/commit/881bf672692be0c9427db76e596f55c8d3a3c17f"><code>881bf67</code></a> chore: Remove unused features</li>
<li><a href="https://github.com/toml-rs/toml/commit/b62c76e261b0ffb43ce6dc214070f43fb58b088e"><code>b62c76e</code></a> refactor: Resolve deprecations</li>
<li>Additional commits viewable in <a href="https://github.com/toml-rs/toml/compare/toml-v0.8.13...toml-v0.8.14">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=toml&package-manager=cargo&previous-version=0.8.13&new-version=0.8.14)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-04 16:33:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4690" class=".btn">#4690</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump pytest from 8.2.1 to 8.2.2 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.2.1 to 8.2.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>8.2.2</h2>
<h1>pytest 8.2.2 (2024-06-04)</h1>
<h2>Bug Fixes</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12355">#12355</a>: Fix possible catastrophic performance slowdown on a certain parametrization pattern involving many higher-scoped parameters.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12367">#12367</a>: Fix a regression in pytest 8.2.0 where unittest class instances (a fresh one is created for each test) were not released promptly on test teardown but only on session teardown.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12381">#12381</a>: Fix possible &quot;Directory not empty&quot; crashes arising from concurent cache dir (<code>.pytest_cache</code>) creation. Regressed in pytest 8.2.0.</li>
</ul>
<h2>Improved Documentation</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12290">#12290</a>: Updated Sphinx theme to use Furo instead of Flask, enabling Dark mode theme.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12356">#12356</a>: Added a subsection to the documentation for debugging flaky tests to mention
lack of thread safety in pytest as a possible source of flakyness.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12363">#12363</a>: The documentation webpages now links to a canonical version to reduce outdated documentation in search engine results.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/329d3712146e69c471be3e30883d54bdde2f76cb"><code>329d371</code></a> Prepare release version 8.2.2</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/214d098fcce88940f5ce9353786b3cc8f0bd3938"><code>214d098</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12414">#12414</a> from bluetech/backport-12409</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/153a436bc40c9e89d90d62255ef5a89e9a762dca"><code>153a436</code></a> [8.2.x] fixtures: fix catastrophic performance problem in <code>reorder_items</code></li>
<li><a href="https://github.com/pytest-dev/pytest/commit/b41d5a52bbb808780ab310456d71e5ce509fd402"><code>b41d5a5</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12412">#12412</a> from pytest-dev/backport-12408-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/9bb73d734ff40f52d7bbebd708b5e3ab1ba20798"><code>9bb73d7</code></a> [8.2.x] cacheprovider: fix &quot;Directory not empty&quot; crash from cache directory c...</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/4569a01e3d20d64811d48b0b09539596520ea5a6"><code>4569a01</code></a> [8.2.x] doc: Update trainings/events (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12402">#12402</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/1d103e5cdc1cb08f332e61a5b20fb205fa5228e7"><code>1d103e5</code></a> [8.2.x] Clarify pytest_ignore_collect docs (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12386">#12386</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/240a252d34fff26efad5b3a92e62be4c9af94b70"><code>240a252</code></a> [8.2.x] Add html_baseurl to sphinx conf.py (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12372">#12372</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/a5ee3c41268199c2c0af59c33050326b1c4a342e"><code>a5ee3c4</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12370">#12370</a> from pytest-dev/backport-12368-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/f7358aec2884720b4de4594ffd0811b46316514c"><code>f7358ae</code></a> [8.2.x] unittest: fix class instances no longer released on test teardown sin...</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/8.2.1...8.2.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=8.2.1&new-version=8.2.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-04 16:30:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4688" class=".btn">#4688</a>
            </td>
            <td>
                <b>
                    build(Dockerfile): pin platform to `linux/amd64`, refactor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Since the Dockerfile only supports building for `linux/amd64`, let's pin it for now before we introduce multi-arch builds. Unused (seemingly) dependencies and unnecessary `RUN` layers have been removed/compressed.

### Linked issue

Related to #4687.

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Docker builds should be faster, unneeded stuff doesn't clutter the Dockerfile.

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
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
        Created At 2024-06-04 11:09:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4684" class=".btn">#4684</a>
            </td>
            <td>
                <b>
                    feat(client cli): extend client cli to request json queries
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Extend `json` subcommand to allow pass json queries.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Examples

```bash
echo '{"FindAllParameters": null }' | ./iroha --config client.toml json query
```

### Benefits

Simplify troubleshooting.

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
        Created At 2024-06-04 09:26:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4683" class=".btn">#4683</a>
            </td>
            <td>
                <b>
                    chore(deps): bump faker from 25.3.0 to 25.4.0 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [faker](https://github.com/joke2k/faker) from 25.3.0 to 25.4.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/joke2k/faker/releases">faker's releases</a>.</em></p>
<blockquote>
<h2>Release v25.4.0</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v25.4.0/CHANGELOG.md">CHANGELOG.md</a>.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/joke2k/faker/blob/master/CHANGELOG.md">faker's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/joke2k/faker/compare/v25.3.0...v25.4.0">v25.4.0 - 2024-05-03</a></h3>
<ul>
<li>Add landmarks in <code>geo</code> for <code>pl_PL</code>. Thanks <a href="https://github.com/george0st"><code>@​george0st</code></a>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/joke2k/faker/commit/9c25db8bb15fa4da30cadbbbab52943e749e7b8e"><code>9c25db8</code></a> Bump version: 25.3.0 → 25.4.0</li>
<li><a href="https://github.com/joke2k/faker/commit/605d1ecc1fad2ad328846b7eaa757b6457613b04"><code>605d1ec</code></a> :pencil: Update CHANGELOG.md</li>
<li><a href="https://github.com/joke2k/faker/commit/705b9e85e344b8ab2ba631bedb915ba818b7a000"><code>705b9e8</code></a> Add landmarks in <code>geo</code> for <code>pl_PL</code> (<a href="https://redirect.github.com/joke2k/faker/issues/2048">#2048</a>)</li>
<li><a href="https://github.com/joke2k/faker/commit/6e888548325f6e280aef6ecc5c8001a25a6c9114"><code>6e88854</code></a> lint code</li>
<li><a href="https://github.com/joke2k/faker/commit/5f791e4e9832a52e721c3f076f48baaffb58e2b0"><code>5f791e4</code></a> Filter code over <code>pyupgrade --py38-plus</code> and ruff (<a href="https://redirect.github.com/joke2k/faker/issues/2052">#2052</a>)</li>
<li><a href="https://github.com/joke2k/faker/commit/2ad1315be066e7b35f10e9b93b0b78904f3dd6d2"><code>2ad1315</code></a> Use comprehension in it_IT address provider to populate cities for performanc...</li>
<li>See full diff in <a href="https://github.com/joke2k/faker/compare/v25.3.0...v25.4.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=faker&package-manager=pip&previous-version=25.3.0&new-version=25.4.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-03 16:44:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4682" class=".btn">#4682</a>
            </td>
            <td>
                <b>
                    chore(deps): bump proc-macro2 from 1.0.84 to 1.0.85
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [proc-macro2](https://github.com/dtolnay/proc-macro2) from 1.0.84 to 1.0.85.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/proc-macro2/releases">proc-macro2's releases</a>.</em></p>
<blockquote>
<h2>1.0.85</h2>
<ul>
<li>Mark some tests as only for 64-bit targets (<a href="https://redirect.github.com/dtolnay/proc-macro2/issues/463">#463</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/5ee1cabadb40abe12abe27e3b34de8fc6f60bc0a"><code>5ee1cab</code></a> Release 1.0.85</li>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/aa64c2007390a33d4edbc07aa3e576848ae3d653"><code>aa64c20</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/proc-macro2/issues/464">#464</a> from dtolnay/testsize</li>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/bc9f4d938058be43d38f921f34f48b94a25278b7"><code>bc9f4d9</code></a> Ignore size tests on non-64bit target</li>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/1160ec3c7d723e115c5acf2b4e9f00c2c049e84a"><code>1160ec3</code></a> Make size tests #[ignore] in cfg(randomize_layout)</li>
<li>See full diff in <a href="https://github.com/dtolnay/proc-macro2/compare/1.0.84...1.0.85">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=proc-macro2&package-manager=cargo&previous-version=1.0.84&new-version=1.0.85)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-03 16:20:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4681" class=".btn">#4681</a>
            </td>
            <td>
                <b>
                    chore(deps): bump w3f-bls from 0.1.3 to 0.1.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [w3f-bls](https://github.com/w3f/bls) from 0.1.3 to 0.1.4.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/w3f/bls/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=w3f-bls&package-manager=cargo&previous-version=0.1.3&new-version=0.1.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-03 16:16:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4680" class=".btn">#4680</a>
            </td>
            <td>
                <b>
                    feat: Add detect support for `parity_scale_decoder`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->
- add color detect support in partiy_scale_decoder
- fix typo (colour -> color) in cli

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4487

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits
Users don't have to rebuild `parity_scale_cli` when disabling terminal-colors. 
Which seems not happening right now since no color is used in parity_scale_cli for now.

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
- [x] (optional) I've written unit tests for the code changes
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
        Created At 2024-06-03 15:08:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4679" class=".btn">#4679</a>
            </td>
            <td>
                <b>
                    refactor!: Rename `--outfile` to `--out-file`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Rename parameter `--outfile` to `--out-file` for `iroha_swarm` and `iroha_wasm_builder`

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4675

### Benefits

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-03 14:35:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4676" class=".btn">#4676</a>
            </td>
            <td>
                <b>
                    chore(deps): bump tokio from 1.37.0 to 1.38.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [tokio](https://github.com/tokio-rs/tokio) from 1.37.0 to 1.38.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/tokio-rs/tokio/releases">tokio's releases</a>.</em></p>
<blockquote>
<h2>Tokio v1.38.0</h2>
<p>This release marks the beginning of stabilization for runtime metrics. It
stabilizes <code>RuntimeMetrics::worker_count</code>. Future releases will continue to
stabilize more metrics.</p>
<h3>Added</h3>
<ul>
<li>fs: add <code>File::create_new</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6573">#6573</a>)</li>
<li>io: add <code>copy_bidirectional_with_sizes</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6500">#6500</a>)</li>
<li>io: implement <code>AsyncBufRead</code> for <code>Join</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6449">#6449</a>)</li>
<li>net: add Apple visionOS support (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6465">#6465</a>)</li>
<li>net: implement <code>Clone</code> for <code>NamedPipeInfo</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6586">#6586</a>)</li>
<li>net: support QNX OS (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6421">#6421</a>)</li>
<li>sync: add <code>Notify::notify_last</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6520">#6520</a>)</li>
<li>sync: add <code>mpsc::Receiver::{capacity,max_capacity}</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6511">#6511</a>)</li>
<li>sync: add <code>split</code> method to the semaphore permit (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6472">#6472</a>, <a href="https://redirect.github.com/tokio-rs/tokio/issues/6478">#6478</a>)</li>
<li>task: add <code>tokio::task::join_set::Builder::spawn_blocking</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6578">#6578</a>)</li>
<li>wasm: support rt-multi-thread with wasm32-wasi-preview1-threads (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6510">#6510</a>)</li>
</ul>
<h3>Changed</h3>
<ul>
<li>macros: make <code>#[tokio::test]</code> append <code>#[test]</code> at the end of the attribute list (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6497">#6497</a>)</li>
<li>metrics: fix <code>blocking_threads</code> count (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6551">#6551</a>)</li>
<li>metrics: stabilize <code>RuntimeMetrics::worker_count</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6556">#6556</a>)</li>
<li>runtime: move task out of the <code>lifo_slot</code> in <code>block_in_place</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6596">#6596</a>)</li>
<li>runtime: panic if <code>global_queue_interval</code> is zero (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6445">#6445</a>)</li>
<li>sync: always drop message in destructor for oneshot receiver (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6558">#6558</a>)</li>
<li>sync: instrument <code>Semaphore</code> for task dumps (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6499">#6499</a>)</li>
<li>sync: use FIFO ordering when waking batches of wakers (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6521">#6521</a>)</li>
<li>task: make <code>LocalKey::get</code> work with Clone types (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6433">#6433</a>)</li>
<li>tests: update nix and mio-aio dev-dependencies (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6552">#6552</a>)</li>
<li>time: clean up implementation (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6517">#6517</a>)</li>
<li>time: lazily init timers on first poll (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6512">#6512</a>)</li>
<li>time: remove the <code>true_when</code> field in <code>TimerShared</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6563">#6563</a>)</li>
<li>time: use sharding for timer implementation (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6534">#6534</a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>taskdump: allow building taskdump docs on non-unix machines (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6564">#6564</a>)</li>
<li>time: check for overflow in <code>Interval::poll_tick</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6487">#6487</a>)</li>
<li>sync: fix incorrect <code>is_empty</code> on mpsc block boundaries (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6603">#6603</a>)</li>
</ul>
<h3>Documented</h3>
<ul>
<li>fs: rewrite file system docs (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6467">#6467</a>)</li>
<li>io: fix <code>stdin</code> documentation (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6581">#6581</a>)</li>
<li>io: fix obsolete reference in <code>ReadHalf::unsplit()</code> documentation (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6498">#6498</a>)</li>
<li>macros: render more comprehensible documentation for <code>select!</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6468">#6468</a>)</li>
<li>net: add missing types to module docs (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6482">#6482</a>)</li>
<li>net: fix misleading <code>NamedPipeServer</code> example (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6590">#6590</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tokio-rs/tokio/commit/14c17fc09656a30230177b600bacceb9db33e942"><code>14c17fc</code></a> chore: prepare Tokio v1.38.0 (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6601">#6601</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/65cbf730de48ef9d3c84959d26ab717a85a5de62"><code>65cbf73</code></a> chore: prepare tokio-macros v2.3.0 (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6600">#6600</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/dbf93c71844a01574a10f9dee0d4d9655a569f0a"><code>dbf93c7</code></a> sync: fix incorrect is_empty on mpsc block boundaries (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6603">#6603</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/873cb8ae2fc291eaffbd71e3c83d17b2f0ed7abf"><code>873cb8a</code></a> runtime: move task out of the <code>lifo_slot</code> in <code>block_in_place</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6596">#6596</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/97bb47b480c66083397c21d54e7ae33cab6c1b20"><code>97bb47b</code></a> task: fix a typo in doc of <code>LocalSet::run_until</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6599">#6599</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/86658bd87dc470f8e36eb6b893cc403820cfb7ee"><code>86658bd</code></a> metrics: stabilize <code>RuntimeMetrics::worker_count</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6556">#6556</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/9e00b266e08d263c497dc9de57d9acbc049ae69b"><code>9e00b26</code></a> sync: add <code>Notify::notify_last</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6520">#6520</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/6c42d286b343f498ce29de2aab9358a0aedb081c"><code>6c42d28</code></a> net: fix misleading <code>NamedPipeServer</code> example (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6590">#6590</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/3a6fdc05681841c30fe4e27b63924c7908ea4634"><code>3a6fdc0</code></a> license: fix formatting and remove year in licenses (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6451">#6451</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/2890d0c3db4f595330d8d223bfbfeb81e205b048"><code>2890d0c</code></a> metrics: fix blocking_threads count (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6551">#6551</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/tokio-rs/tokio/compare/tokio-1.37.0...tokio-1.38.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tokio&package-manager=cargo&previous-version=1.37.0&new-version=1.38.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-31 16:44:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4674" class=".btn">#4674</a>
            </td>
            <td>
                <b>
                    chore: use temporary `displaydoc` fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Use the fix from https://github.com/yaahc/displaydoc/pull/47 until it is merged into the upstream.

### Linked issue

Closes #4567

### Benefits

Reduces warnings noise

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-31 04:50:03 +0000 UTC
    </div>
</div>

