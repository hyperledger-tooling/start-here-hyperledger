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
                PR <a href="https://github.com/hyperledger/iroha/pull/4548" class=".btn">#4548</a>
            </td>
            <td>
                <b>
                    IGNORE: Merge to main
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
        Created At 2024-05-03 12:40:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4547" class=".btn">#4547</a>
            </td>
            <td>
                <b>
                    fix: remove serde(flatten) from SetKeyValue/RemoveKeyValue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

serde cannot flatten Strings and O::Id is always serialized as string. As a consequence it's impossible to serialize/deserialize SetKeyValue/RemoveKeyValue in genesis

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
        Created At 2024-05-03 11:25:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4546" class=".btn">#4546</a>
            </td>
            <td>
                <b>
                    fix: remove serde(flatten) from SetKeyValue/RemoveKeyValue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

serde cannot flatten `String`s and `O::Id` is always serialized as string. As a consequence it's impossible to serialize/deserialize `SetKeyValue`/`RemoveKeyValue` in genesis

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
        Created At 2024-05-03 11:15:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4545" class=".btn">#4545</a>
            </td>
            <td>
                <b>
                    chore(deps): bump faker from 25.0.0 to 25.0.1 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [faker](https://github.com/joke2k/faker) from 25.0.0 to 25.0.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/joke2k/faker/releases">faker's releases</a>.</em></p>
<blockquote>
<h2>Release v25.0.1</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v25.0.1/CHANGELOG.md">CHANGELOG.md</a>.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/joke2k/faker/blob/master/CHANGELOG.md">faker's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/joke2k/faker/compare/v25.0.0...v25.0.1">v25.0.1 - 2024-05-02</a></h3>
<ul>
<li>Add type stub file to <code>setup.py</code>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/joke2k/faker/commit/2069bd3f57caff88fd0b7cbcd51f970890be43bd"><code>2069bd3</code></a> Bump version: 25.0.0 → 25.0.1</li>
<li><a href="https://github.com/joke2k/faker/commit/681922c11de9abfae3fd72e92becb54dc3c3c733"><code>681922c</code></a> :pencil: Update CHANGELOG.md</li>
<li><a href="https://github.com/joke2k/faker/commit/106d8ba3981445bad6915a0567931416539149f7"><code>106d8ba</code></a> add stub to setup.py</li>
<li>See full diff in <a href="https://github.com/joke2k/faker/compare/v25.0.0...v25.0.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=faker&package-manager=pip&previous-version=25.0.0&new-version=25.0.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-02 16:49:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4544" class=".btn">#4544</a>
            </td>
            <td>
                <b>
                    feat: filtered queries in contracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
            </td>
            <td>
                ## Description

- remove `QueryWithParameters`
- move all parameters to `ClientQueryPayload` (was `QueryPayload` before, stored inside `SignedQuery`); `SignedQuery` now equivalent to `QueryWithParameters<SignedQuery>`. All the parameters are now scale-encoded and versioned instead of being passed as query parameters
- make `SmartContractQuery`, which is now equivalent to `QueryWithParameters<QueryBox>` that was used before, but has filtering support
- move all the post-processing (filterting, sorting, pagination, batching) to a single function (`LazyQueryOutput::apply_postprocessing`), introduce a new type for a post-processed query output
- add an integration test using the filtering (`ProcessedQueryOutput`)

### Linked issue

Closes #4423 

### Checklist

- [ ] make CI pass

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-02 13:12:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4543" class=".btn">#4543</a>
            </td>
            <td>
                <b>
                    fix: Report if a request to check peer status in test_network fails
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Warn if a peer status request is failed. Helped me debug my misconfigured proxy failing tests when ran in IDE...

This also refactors a function a bit, because IMO it was a bit hard to read with the fold and `map_or`

### Linked issue

Closes #4542

### Benefits

`+` Easier debugging if something went wrong with requests
`-` Can introduce log noise, but shouldn't happen if the actual connection to the node is OK

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-02 13:04:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4541" class=".btn">#4541</a>
            </td>
            <td>
                <b>
                    refactor!: Use multihash format for private keys
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">config-changes</span>
            </td>
            <td>
                ## Description

Added support for encoding/decoding private keys to `multihash` module, and replaced each occurence of `PRIVATE_KEY_ALGORITHM`/`PRIVATE_KEY_PAYLOAD` pair to `PRIVATE_KEY` in multihash format

### Linked issue

Closes #4412

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
        Created At 2024-05-02 12:13:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4539" class=".btn">#4539</a>
            </td>
            <td>
                <b>
                    chore(deps): bump serde from 1.0.199 to 1.0.200
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [serde](https://github.com/serde-rs/serde) from 1.0.199 to 1.0.200.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/serde-rs/serde/releases">serde's releases</a>.</em></p>
<blockquote>
<h2>v1.0.200</h2>
<ul>
<li>Fix formatting of &quot;invalid type&quot; and &quot;invalid value&quot; deserialization error messages containing NaN or infinite floats (<a href="https://redirect.github.com/serde-rs/serde/issues/2733">#2733</a>, thanks <a href="https://github.com/jamessan"><code>@​jamessan</code></a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/serde-rs/serde/commit/cc865ac5236c094275b10bff4fa41e561b3e359f"><code>cc865ac</code></a> Release 1.0.200</li>
<li><a href="https://github.com/serde-rs/serde/commit/2d973c1805dd9b613e89cc2375130a23f18ffa73"><code>2d973c1</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/serde/issues/2733">#2733</a> from jamessan/nan-decimal</li>
<li><a href="https://github.com/serde-rs/serde/commit/6ca499b2dd3d520903095b202770eba2720ba9b5"><code>6ca499b</code></a> Only format Unexpected::Float with decimal point if it is finite</li>
<li>See full diff in <a href="https://github.com/serde-rs/serde/compare/v1.0.199...v1.0.200">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=serde&package-manager=cargo&previous-version=1.0.199&new-version=1.0.200)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-01 16:13:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4538" class=".btn">#4538</a>
            </td>
            <td>
                <b>
                    fix: Remove nested option on `TransactionEventFilter::block_height`
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
        Created At 2024-05-01 14:16:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4536" class=".btn">#4536</a>
            </td>
            <td>
                <b>
                    ci: trigger PR CI on lockfile updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Trigger PR CI when `.lock` files are updated. 

### Benefits

pytests will run on dependabot version updates

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
        Created At 2024-05-01 08:27:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4535" class=".btn">#4535</a>
            </td>
            <td>
                <b>
                    chore(deps): bump base64 from 0.22.0 to 0.22.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [base64](https://github.com/marshallpierce/rust-base64) from 0.22.0 to 0.22.1.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/marshallpierce/rust-base64/blob/master/RELEASE-NOTES.md">base64's changelog</a>.</em></p>
<blockquote>
<h1>0.22.1</h1>
<ul>
<li>Correct the symbols used for the predefined <code>alphabet::BIN_HEX</code>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/e14400697453bcc85997119b874bc03d9601d0af"><code>e144006</code></a> v0.22.1</li>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/64cca59ddbb4c43244a8f38629b59960ffe36bc0"><code>64cca59</code></a> Merge pull request <a href="https://redirect.github.com/marshallpierce/rust-base64/issues/271">#271</a> from JobanSD/patch-1</li>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/838355e0ac5fb8237ec9b96be5edb011bff00275"><code>838355e</code></a> Correct BinHex 4.0 alphabet according to specifications</li>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/bf15ccf30af8bb6b1f326fffa025d7b0aaa3342f"><code>bf15ccf</code></a> Merge pull request <a href="https://redirect.github.com/marshallpierce/rust-base64/issues/270">#270</a> from marshallpierce/mp/clippy</li>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/fc6aabee8afaf8b2f4cfb12df4cf461bcf9b003d"><code>fc6aabe</code></a> Appease clippy</li>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/9a518a2d5d028068d4bf83ebf437f7a3575e640e"><code>9a518a2</code></a> Merge pull request <a href="https://redirect.github.com/marshallpierce/rust-base64/issues/267">#267</a> from bdura/patch-1</li>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/d96c80f242e3080a03fd1c079730e17373ef0eb6"><code>d96c80f</code></a> Merge branch 'marshallpierce:master' into patch-1</li>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/e8e4a22761614cab33d838b354c946427d136db8"><code>e8e4a22</code></a> docs: fix trailing ``` in mod.rs example</li>
<li>See full diff in <a href="https://github.com/marshallpierce/rust-base64/compare/v0.22.0...v0.22.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=base64&package-manager=cargo&previous-version=0.22.0&new-version=0.22.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-01 06:31:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4534" class=".btn">#4534</a>
            </td>
            <td>
                <b>
                    chore(dependabot): follow conventional commits
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Linked issue

Related to #4502.

<!-- Link if e.g. JIRA issue or  from another repository -->

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
        Created At 2024-05-01 06:29:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4533" class=".btn">#4533</a>
            </td>
            <td>
                <b>
                    ci: Set up PR labeler for I1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Label PRs targeting `iroha1-main` with `iroha1`

### Linked issue

Linked to #4501 

<!-- Link if e.g. JIRA issue or  from another repository -->

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
        Created At 2024-04-30 09:39:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4532" class=".btn">#4532</a>
            </td>
            <td>
                <b>
                    [ci] #4501: Remove `iroha2` labeler matcher
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2-dev</span><span class="chip">CI</span>
            </td>
            <td>
                ## Description

Stop labeling PRs with the `iroha2` label. 

### Linked issue

Linked to #4501.

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
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
        Created At 2024-04-30 09:25:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4531" class=".btn">#4531</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump faker from 24.11.0 to 25.0.0 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2-dev</span><span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [faker](https://github.com/joke2k/faker) from 24.11.0 to 25.0.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/joke2k/faker/releases">faker's releases</a>.</em></p>
<blockquote>
<h2>Release v25.0.0</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v25.0.0/CHANGELOG.md">CHANGELOG.md</a>.</p>
<h2>Release v24.14.1</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v24.14.1/CHANGELOG.md">CHANGELOG.md</a>.</p>
<h2>Release v24.14.0</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v24.14.0/CHANGELOG.md">CHANGELOG.md</a>.</p>
<h2>Release v24.13.0</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v24.13.0/CHANGELOG.md">CHANGELOG.md</a>.</p>
<h2>Release v24.12.0</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v24.12.0/CHANGELOG.md">CHANGELOG.md</a>.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/joke2k/faker/blob/master/CHANGELOG.md">faker's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/joke2k/faker/compare/v24.14.1...v25.0.0">v25.0.0 - 2024-04-28</a></h3>
<ul>
<li>Drop support for Python 3.7. Thanks <a href="https://github.com/kloczek"><code>@​kloczek</code></a>.</li>
</ul>
<h3><a href="https://github.com/joke2k/faker/compare/v24.14.0...v24.14.1">v24.14.1 - 2024-04-28</a></h3>
<ul>
<li>Include type stubs in release.</li>
</ul>
<h3><a href="https://github.com/joke2k/faker/compare/v24.13.0...v24.14.0">v24.14.0 - 2024-04-25</a></h3>
<ul>
<li>Add job provider for <code>cs_CZ</code>. Thanks <a href="https://github.com/george0st"><code>@​george0st</code></a>.</li>
</ul>
<h3><a href="https://github.com/joke2k/faker/compare/v24.12.0...v24.13.0">v24.13.0 - 2024-04-25</a></h3>
<ul>
<li>Add geo provider for <code>sk_SK</code>. Thanks <a href="https://github.com/george0st"><code>@​george0st</code></a>.</li>
<li>Clean up data in <code>sk_SK</code> job provider. Thanks <a href="https://github.com/george0st"><code>@​george0st</code></a>.</li>
</ul>
<h3><a href="https://github.com/joke2k/faker/compare/v24.11.0...v24.12.0">v24.12.0 - 2024-04-25</a></h3>
<ul>
<li>Remove offensive word from <code>pl_PL</code> lorem provider. Thanks <a href="https://github.com/Rey092"><code>@​Rey092</code></a>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/joke2k/faker/commit/7f5dc148afdcf06dee08381a4f85e082da2346b4"><code>7f5dc14</code></a> Bump version: 24.14.1 → 25.0.0</li>
<li><a href="https://github.com/joke2k/faker/commit/bcd3c693851906803aa5be04af31148d0741782c"><code>bcd3c69</code></a> :pencil: Update CHANGELOG.md</li>
<li><a href="https://github.com/joke2k/faker/commit/9402b8fbff281fcdcab3b978c7bc39e9723d5158"><code>9402b8f</code></a> fix pip cache</li>
<li><a href="https://github.com/joke2k/faker/commit/3aba828ec78afe79903aec9241db9efe049723bc"><code>3aba828</code></a> fix pip cache</li>
<li><a href="https://github.com/joke2k/faker/commit/5b3ef9cc9543d97dab8498e4f840084ce1883b89"><code>5b3ef9c</code></a> fix pip cache</li>
<li><a href="https://github.com/joke2k/faker/commit/a09f0681e45023fa0ac1b8a4e2a408aa2bc5ea71"><code>a09f068</code></a> :lipstick: format code</li>
<li><a href="https://github.com/joke2k/faker/commit/d6c08140f56ccb39edb899064de89139c31a7330"><code>d6c0814</code></a> drop python&lt;=3.7 support (<a href="https://redirect.github.com/joke2k/faker/issues/2030">#2030</a>)</li>
<li><a href="https://github.com/joke2k/faker/commit/2049e02c01aa1deda40af44fe84c07933f134c3e"><code>2049e02</code></a> Fix link formatting in CHANGELOG.md (<a href="https://redirect.github.com/joke2k/faker/issues/2036">#2036</a>)</li>
<li><a href="https://github.com/joke2k/faker/commit/971b8b62c1002c3994e9854372f8a24ebb4ffb68"><code>971b8b6</code></a> Bump version: 24.14.0 → 24.14.1</li>
<li><a href="https://github.com/joke2k/faker/commit/d76e3f0fcd5f5d2b816a5613e495ec51f937bc64"><code>d76e3f0</code></a> :pencil: Update CHANGELOG.md</li>
<li>Additional commits viewable in <a href="https://github.com/joke2k/faker/compare/v24.11.0...v25.0.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=faker&package-manager=pip&previous-version=24.11.0&new-version=25.0.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-29 16:34:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4530" class=".btn">#4530</a>
            </td>
            <td>
                <b>
                    [chore]: Bump pytest from 8.0.0 to 8.2.0 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2-dev</span><span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.0.0 to 8.2.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>8.2.0</h2>
<h1>pytest 8.2.0 (2024-04-27)</h1>
<h2>Deprecations</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12069">#12069</a>: A deprecation warning is now raised when implementations of one of the following hooks request a deprecated <code>py.path.local</code> parameter instead of the <code>pathlib.Path</code> parameter which replaced it:</p>
<ul>
<li><code>pytest_ignore_collect</code>{.interpreted-text role=&quot;hook&quot;} - the <code>path</code> parameter - use <code>collection_path</code> instead.</li>
<li><code>pytest_collect_file</code>{.interpreted-text role=&quot;hook&quot;} - the <code>path</code> parameter - use <code>file_path</code> instead.</li>
<li><code>pytest_pycollect_makemodule</code>{.interpreted-text role=&quot;hook&quot;} - the <code>path</code> parameter - use <code>module_path</code> instead.</li>
<li><code>pytest_report_header</code>{.interpreted-text role=&quot;hook&quot;} - the <code>startdir</code> parameter - use <code>start_path</code> instead.</li>
<li><code>pytest_report_collectionfinish</code>{.interpreted-text role=&quot;hook&quot;} - the <code>startdir</code> parameter - use <code>start_path</code> instead.</li>
</ul>
<p>The replacement parameters are available since pytest 7.0.0.
The old parameters will be removed in pytest 9.0.0.</p>
<p>See <code>legacy-path-hooks-deprecated</code>{.interpreted-text role=&quot;ref&quot;} for more details.</p>
</li>
</ul>
<h2>Features</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/11871">#11871</a>: Added support for reading command line arguments from a file using the prefix character <code>@</code>, like e.g.: <code>pytest @tests.txt</code>. The file must have one argument per line.</p>
<p>See <code>Read arguments from file &lt;args-from-file&gt;</code>{.interpreted-text role=&quot;ref&quot;} for details.</p>
</li>
</ul>
<h2>Improvements</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/11523">#11523</a>: <code>pytest.importorskip</code>{.interpreted-text role=&quot;func&quot;} will now issue a warning if the module could be found, but raised <code>ImportError</code>{.interpreted-text role=&quot;class&quot;} instead of <code>ModuleNotFoundError</code>{.interpreted-text role=&quot;class&quot;}.</p>
<p>The warning can be suppressed by passing <code>exc_type=ImportError</code> to <code>pytest.importorskip</code>{.interpreted-text role=&quot;func&quot;}.</p>
<p>See <code>import-or-skip-import-error</code>{.interpreted-text role=&quot;ref&quot;} for details.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/11728">#11728</a>: For <code>unittest</code>-based tests, exceptions during class cleanup (as raised by functions registered with <code>TestCase.addClassCleanup &lt;unittest.TestCase.addClassCleanup&gt;</code>{.interpreted-text role=&quot;meth&quot;}) are now reported instead of silently failing.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/11777">#11777</a>: Text is no longer truncated in the <code>short test summary info</code> section when <code>-vv</code> is given.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12112">#12112</a>: Improved namespace packages detection when <code>consider_namespace_packages</code>{.interpreted-text role=&quot;confval&quot;} is enabled, covering more situations (like editable installs).</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/9502">#9502</a>: Added <code>PYTEST_VERSION</code>{.interpreted-text role=&quot;envvar&quot;} environment variable which is defined at the start of the pytest session and undefined afterwards. It contains the value of <code>pytest.__version__</code>, and among other things can be used to easily check if code is running from within a pytest run.</p>
</li>
</ul>
<h2>Bug Fixes</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12065">#12065</a>: Fixed a regression in pytest 8.0.0 where test classes containing <code>setup_method</code> and tests using <code>@staticmethod</code> or <code>@classmethod</code> would crash with <code>AttributeError: 'NoneType' object has no attribute 'setup_method'</code>.</p>
<p>Now the <code>request.instance &lt;pytest.FixtureRequest.instance&gt;</code>{.interpreted-text role=&quot;attr&quot;} attribute of tests using <code>@staticmethod</code> and <code>@classmethod</code> is no longer <code>None</code>, but a fresh instance of the class, like in non-static methods.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/6bd3f313447290380cbc2db30fb9ee5cca7eb941"><code>6bd3f31</code></a> Tweak changelog for 8.2.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/9b6219b5e89af237e5bc80354d405d2b5c2fc8a0"><code>9b6219b</code></a> Prepare release version 8.2.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/835765c9d31e0a86c6028f983b28d32c82a759c4"><code>835765c</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12130">#12130</a> from bluetech/fixtures-inline</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/7e7503c0b015f61d9d21d3b5f55990b7fcd683f7"><code>7e7503c</code></a> unittest: report class cleanup exceptions (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12250">#12250</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/882c4da2f37702b00bdbd3b6c74e9821d33e0204"><code>882c4da</code></a> fixtures: inline <code>fail_fixturefunc</code></li>
<li><a href="https://github.com/pytest-dev/pytest/commit/2e8fb9f1401d727e20f004326752fd1922f9c601"><code>2e8fb9f</code></a> fixtures: extract a <code>_check_fixturedef</code> method</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/acf2971f46a9518b3552d48ea9541a1951c2b207"><code>acf2971</code></a> fixtures: inline <code>_getnextfixturedef</code> into <code>_get_active_fixturedef</code></li>
<li><a href="https://github.com/pytest-dev/pytest/commit/3c77aec1dac0894ec4ca774b71ec91c85cf91dd1"><code>3c77aec</code></a> fixtures: move &quot;request&quot; check early</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/d217d68cde0c34d619862f15c773ecc02ecdaabe"><code>d217d68</code></a> fixtures: inline <code>_compute_fixture_value</code></li>
<li><a href="https://github.com/pytest-dev/pytest/commit/530be285751143febe54b8974b234eed5eb8b079"><code>530be28</code></a> fixtures: use early return in <code>_get_active_fixturedef</code></li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/8.0.0...8.2.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=8.0.0&new-version=8.2.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-29 16:33:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4529" class=".btn">#4529</a>
            </td>
            <td>
                <b>
                    [chore]: Bump pytest-xdist from 3.5.0 to 3.6.1 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2-dev</span><span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-xdist](https://github.com/pytest-dev/pytest-xdist) from 3.5.0 to 3.6.1.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-xdist/blob/master/CHANGELOG.rst">pytest-xdist's changelog</a>.</em></p>
<blockquote>
<h1>pytest-xdist 3.6.1 (2024-04-28)</h1>
<h2>Bug Fixes</h2>
<ul>
<li><code>[#1071](https://github.com/pytest-dev/pytest-xdist/issues/1071) &lt;https://github.com/pytest-dev/pytest-xdist/issues/1071&gt;</code>_: Add backward compatibility for deadlock issue with the <code>execnet</code> new <code>main_thread_only</code> &quot;execmodel&quot; triggered when pytest-cov accesses rinfo.</li>
</ul>
<h1>pytest-xdist 3.6.0 (2024-04-19)</h1>
<p>This release was YANKED due to a regression fixed in 3.6.1.</p>
<h2>Features</h2>
<ul>
<li><code>[#1027](https://github.com/pytest-dev/pytest-xdist/issues/1027) &lt;https://github.com/pytest-dev/pytest-xdist/pull/1027&gt;</code>_:<code>pytest-xdist</code> workers now always execute the tests in the main thread.
Previously some tests might end up executing in a separate thread other than <code>main</code> in the workers, due to some internal <code>execnet`` details. This can cause problems specially with async frameworks where the event loop is running in the ``main`` thread (for example </code><a href="https://redirect.github.com/pytest-dev/pytest-xdist/issues/620">#620</a> <a href="https://redirect.github.com/pytest-dev/pytest-xdist/issues/620">pytest-dev/pytest-xdist#620</a>`__).</li>
</ul>
<h2>Bug Fixes</h2>
<ul>
<li>
<p><code>[#1024](https://github.com/pytest-dev/pytest-xdist/issues/1024) &lt;https://github.com/pytest-dev/pytest-xdist/issues/1024&gt;</code>_: Added proper handling of <code>shouldstop</code> (such as set by <code>--max-fail</code>) and <code>shouldfail</code> conditions in workers.
Previously, a worker might have continued executing further tests before the controller could terminate the session.</p>
</li>
<li>
<p><code>[#1028](https://github.com/pytest-dev/pytest-xdist/issues/1028) &lt;https://github.com/pytest-dev/pytest-xdist/issues/1028&gt;</code>_: Fixed compatibility issue between <code>looponfail</code> and editable installs.</p>
</li>
<li>
<p><code>[#620](https://github.com/pytest-dev/pytest-xdist/issues/620) &lt;https://github.com/pytest-dev/pytest-xdist/issues/620&gt;</code>_: Use the new <code>main_thread_only</code> <code>execnet</code> &quot;execmodel&quot; so that code which expects to only run in the main thread will now work as expected.</p>
</li>
<li>
<p><code>[#937](https://github.com/pytest-dev/pytest-xdist/issues/937) &lt;https://github.com/pytest-dev/pytest-xdist/issues/937&gt;</code>_: Fixed a bug where plugin would raise an incompatibility error with <code>--pdb</code> despite using <code>-n0</code>.</p>
</li>
</ul>
<h2>Removals</h2>
<ul>
<li>
<p><code>[#1053](https://github.com/pytest-dev/pytest-xdist/issues/1053) &lt;https://github.com/pytest-dev/pytest-xdist/issues/1053&gt;</code>_: Dropped support for Python 3.7.</p>
</li>
<li>
<p><code>[#1057](https://github.com/pytest-dev/pytest-xdist/issues/1057) &lt;https://github.com/pytest-dev/pytest-xdist/issues/1057&gt;</code>_: pytest&gt;=7.0.0 is now required.</p>
<p>execnet&gt;=2.1.0 is now required.</p>
</li>
</ul>
<h2>Trivial Changes</h2>
<ul>
<li>
<p><code>[#1020](https://github.com/pytest-dev/pytest-xdist/issues/1020) &lt;https://github.com/pytest-dev/pytest-xdist/issues/1020&gt;</code>_: pytest-xdist's <code>setup.py</code> file is removed.</p>
<p>If you relied on this file, e.g. to install pytest using <code>setup.py install</code>,
please see <code>Why you shouldn't invoke setup.py directly &lt;https://blog.ganssle.io/articles/2021/10/setup-py-deprecated.html#summary&gt;</code>_ for alternatives.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-xdist/commit/4dd2978031eaf7017c84a1cc77667379a2b11c64"><code>4dd2978</code></a> Release 3.6.1</li>
<li><a href="https://github.com/pytest-dev/pytest-xdist/commit/b397288b7ed40ac8c55a173566bb881e0adcb546"><code>b397288</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest-xdist/issues/1072">#1072</a> from zmedico/gateway-cache-rinfo</li>
<li><a href="https://github.com/pytest-dev/pytest-xdist/commit/12b3cce0ce4f4cffcc35c0e8369759b71b32c0cc"><code>12b3cce</code></a> Cache execnet gateway rinfo during WorkerController setup</li>
<li><a href="https://github.com/pytest-dev/pytest-xdist/commit/c93a106b3ad466e22d19d814394de0422adf4dca"><code>c93a106</code></a> build(deps): bump hynek/build-and-inspect-python-package (<a href="https://redirect.github.com/pytest-dev/pytest-xdist/issues/1066">#1066</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest-xdist/commit/52e202263827775ad6bcf18a216000aec4412911"><code>52e2022</code></a> [pre-commit.ci] pre-commit autoupdate (<a href="https://redirect.github.com/pytest-dev/pytest-xdist/issues/1073">#1073</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest-xdist/commit/699f939b5cc2d61df9f622d0449a590be216ee7a"><code>699f939</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest-xdist/issues/1070">#1070</a> from pytest-dev/release-3.6.0</li>
<li><a href="https://github.com/pytest-dev/pytest-xdist/commit/80bc0b8e5be6e256c8f49791e08abd5fa2d2d3a2"><code>80bc0b8</code></a> Release 3.6.0</li>
<li><a href="https://github.com/pytest-dev/pytest-xdist/commit/20e3ac774e8fa34b25665ef183b94c9879f98cd1"><code>20e3ac7</code></a> Use execnet main_thread_only execmodel (<a href="https://redirect.github.com/pytest-dev/pytest-xdist/issues/1027">#1027</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest-xdist/commit/0a4238f6da367a9133882d8810a3b556837cb5ae"><code>0a4238f</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest-xdist/issues/1067">#1067</a> from pytest-dev/pre-commit-ci-update-config</li>
<li><a href="https://github.com/pytest-dev/pytest-xdist/commit/068627994f91068fb27269be421385c7cd3ab201"><code>0686279</code></a> [pre-commit.ci] pre-commit autoupdate</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-xdist/compare/v3.5.0...v3.6.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-xdist&package-manager=pip&previous-version=3.5.0&new-version=3.6.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-29 16:32:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4528" class=".btn">#4528</a>
            </td>
            <td>
                <b>
                    [chore]: Bump serial_test from 3.1.0 to 3.1.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2-dev</span><span class="chip">Chore</span><span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                [//]: # (dependabot-start)
⚠️  **Dependabot is rebasing this PR** ⚠️ 

Rebasing might not happen immediately, so don't worry if this takes some time.

Note: if you make any changes to this PR yourself, they will take precedence over the rebase.

---

[//]: # (dependabot-end)

Bumps [serial_test](https://github.com/palfrey/serial_test) from 3.1.0 to 3.1.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/palfrey/serial_test/releases">serial_test's releases</a>.</em></p>
<blockquote>
<h2>v3.1.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix async test functions inside a serial mod block in <a href="https://redirect.github.com/palfrey/serial_test/pull/111">palfrey/serial_test#111</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/palfrey/serial_test/compare/v3.1.0...v3.1.1">https://github.com/palfrey/serial_test/compare/v3.1.0...v3.1.1</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/palfrey/serial_test/commit/b39310b3cff129ab032af0f4ce1c219da540d9b2"><code>b39310b</code></a> 3.1.1</li>
<li><a href="https://github.com/palfrey/serial_test/commit/bf3222814090d9cf1df575b68e7e45cd66f0c5dd"><code>bf32228</code></a> Merge pull request <a href="https://redirect.github.com/palfrey/serial_test/issues/111">#111</a> from palfrey/fix-mod-with-async</li>
<li><a href="https://github.com/palfrey/serial_test/commit/2cb08809ba9a9089dc3c3f17014a4b4b46a10ed8"><code>2cb0880</code></a> Only test async with mod when async is on</li>
<li><a href="https://github.com/palfrey/serial_test/commit/3c258420387224c0c54044a4ac3238b1b8e062c9"><code>3c25842</code></a> Fix async test functions inside a serial mod block</li>
<li>See full diff in <a href="https://github.com/palfrey/serial_test/compare/v3.1.0...v3.1.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=serial_test&package-manager=cargo&previous-version=3.1.0&new-version=3.1.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-29 16:16:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4527" class=".btn">#4527</a>
            </td>
            <td>
                <b>
                    [chore]: Bump serde from 1.0.198 to 1.0.199
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2-dev</span><span class="chip">Chore</span><span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [serde](https://github.com/serde-rs/serde) from 1.0.198 to 1.0.199.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/serde-rs/serde/releases">serde's releases</a>.</em></p>
<blockquote>
<h2>v1.0.199</h2>
<ul>
<li>Fix ambiguous associated item when <code>forward_to_deserialize_any!</code> is used on an enum with <code>Error</code> variant (<a href="https://redirect.github.com/serde-rs/serde/issues/2732">#2732</a>, thanks <a href="https://github.com/aatifsyed"><code>@​aatifsyed</code></a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/serde-rs/serde/commit/147702871760a38d2e97e0cd15d568559876aeda"><code>1477028</code></a> Release 1.0.199</li>
<li><a href="https://github.com/serde-rs/serde/commit/789740be0d2cc1d4e280639039f189cc5d98fb40"><code>789740b</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/serde/issues/2732">#2732</a> from aatifsyed/master</li>
<li><a href="https://github.com/serde-rs/serde/commit/8fe7539bb2b46001f70751f1db60e1a7144f8f3d"><code>8fe7539</code></a> fix: ambiguous associated type in forward_to_deserialize_any!</li>
<li><a href="https://github.com/serde-rs/serde/commit/f6623a36548cfce02f880a33c6d2f420934c95c5"><code>f6623a3</code></a> Ignore cast_precision_loss pedantic clippy lint</li>
<li>See full diff in <a href="https://github.com/serde-rs/serde/compare/v1.0.198...v1.0.199">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=serde&package-manager=cargo&previous-version=1.0.198&new-version=1.0.199)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-29 16:14:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4526" class=".btn">#4526</a>
            </td>
            <td>
                <b>
                    [chore]: Bump libsodium-sys-stable from 1.20.5 to 1.20.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2-dev</span><span class="chip">Chore</span><span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [libsodium-sys-stable](https://github.com/jedisct1/libsodium-sys-stable) from 1.20.5 to 1.20.6.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jedisct1/libsodium-sys-stable/commit/31622bd4380ea8b35d4f1e17d707ed36f4df223b"><code>31622bd</code></a> Update libsodium</li>
<li><a href="https://github.com/jedisct1/libsodium-sys-stable/commit/7a9d205df74cf97d6916a257a8bfd25c5ce56505"><code>7a9d205</code></a> Allow pre-compiled files to be retrieved from a local directory</li>
<li>See full diff in <a href="https://github.com/jedisct1/libsodium-sys-stable/compare/1.20.5...1.20.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=libsodium-sys-stable&package-manager=cargo&previous-version=1.20.5&new-version=1.20.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-29 16:13:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4523" class=".btn">#4523</a>
            </td>
            <td>
                <b>
                    [ci] #4502: Enforce Conventional Commits in PR titles
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2-dev</span><span class="chip">CI</span>
            </td>
            <td>
                ## Description

Enforce Conventional Commits style in PR titles.

### Linked issue

Closes #4502.

### Benefits

See [here](https://www.conventionalcommits.org/en/v1.0.0/#why-use-conventional-commits).

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-29 06:44:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4522" class=".btn">#4522</a>
            </td>
            <td>
                <b>
                    [chore]: Bump serde_with from 3.7.0 to 3.8.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2-dev</span><span class="chip">Chore</span><span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [serde_with](https://github.com/jonasbb/serde_with) from 3.7.0 to 3.8.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/jonasbb/serde_with/releases">serde_with's releases</a>.</em></p>
<blockquote>
<h2>serde_with v3.8.1</h2>
<h3>Fixed</h3>
<ul>
<li>Do not emit <code>schemars(deserialize_with = &quot;...&quot;)</code> annotations, as <code>schemars</code> does not support them (<a href="https://redirect.github.com/jonasbb/serde_with/issues/735">#735</a>)
Thanks to <a href="https://github.com/sivizius"><code>@​sivizius</code></a> for reporting the issue.</li>
</ul>
<h2>serde_with v3.8.0</h2>
<h3>Added</h3>
<ul>
<li>Implement (De)Serialization for Pinned Smart Pointers by <a href="https://github.com/Astralchroma"><code>@​Astralchroma</code></a> (<a href="https://redirect.github.com/jonasbb/serde_with/issues/733">#733</a>)</li>
<li>Implement <code>JsonSchemaAs</code> for <code>PickFirst</code> by <a href="https://github.com/swlynch99"><code>@​swlynch99</code></a>  (<a href="https://redirect.github.com/jonasbb/serde_with/issues/721">#721</a>)</li>
</ul>
<h3>Changed</h3>
<ul>
<li>Bump <code>base64</code> dependency to v0.22 (<a href="https://redirect.github.com/jonasbb/serde_with/issues/724">#724</a>)</li>
<li>Update dev dependencies</li>
</ul>
<h3>Fixed</h3>
<ul>
<li><code>serde_conv</code> regressed and triggered <code>clippy::ptr_arg</code> and add test to prevent future problems. (<a href="https://redirect.github.com/jonasbb/serde_with/issues/731">#731</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jonasbb/serde_with/commit/29ea916ee552a4800c2200fd56376e7e862aa5ad"><code>29ea916</code></a> Bump version to v3.8.1 (<a href="https://redirect.github.com/jonasbb/serde_with/issues/737">#737</a>)</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/13e48a97c28a7a4d5fc8b297ec1d3bb61b5392d6"><code>13e48a9</code></a> Bump version to v3.8.1</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/8869b20ca4112415c068351ae7781df3b570413b"><code>8869b20</code></a> Do not emit schemars(deserialize_with = &quot;...&quot;) (<a href="https://redirect.github.com/jonasbb/serde_with/issues/736">#736</a>)</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/eb77c4043396fb9104c55bc89eb9d1523b10b7e3"><code>eb77c40</code></a> Do not emit schemars(deserialize_with = &quot;...&quot;)</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/7e66d6bba9d853be888c6e9c819e4388301f67dc"><code>7e66d6b</code></a> Bump version to v3.8.0 (<a href="https://redirect.github.com/jonasbb/serde_with/issues/734">#734</a>)</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/4a4fcb3fd4b82bff9e40820e8a44162cfbd08110"><code>4a4fcb3</code></a> Bump version to v3.8.0</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/167e865e407e8f79e56eb8539913521663a96ae5"><code>167e865</code></a> Implement (De)Serialization for Pinned Smart Pointers (<a href="https://redirect.github.com/jonasbb/serde_with/issues/733">#733</a>)</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/04de4ce6d8a26dc755cf31b9e1889d19852c4e51"><code>04de4ce</code></a> Add SerializeAs support for Pin&lt;&amp;'a T&gt; and Pin&lt;&amp;'a mut T&gt;</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/9c2dac75e64a4cbf4db5673ae5a4a7b9039b1d15"><code>9c2dac7</code></a> Implement (De)Serialization for Pinned Smart Pointers</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/9989d8e658c5395277699714a3729614b6853bca"><code>9989d8e</code></a> Add test that serde_conv will not trigger <code>clippy::ptr_arg</code> (<a href="https://redirect.github.com/jonasbb/serde_with/issues/731">#731</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/jonasbb/serde_with/compare/v3.7.0...v3.8.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=serde_with&package-manager=cargo&previous-version=3.7.0&new-version=3.8.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-29 05:38:51 +0000 UTC
    </div>
</div>

