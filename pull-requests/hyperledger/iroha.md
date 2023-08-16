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
                PR <a href="https://github.com/hyperledger/iroha/pull/3815" class=".btn">#3815</a>
            </td>
            <td>
                <b>
                    [refactor] #3276: Add `Snapshotter` actor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

Separate wsv snapshots into separate actor.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3276 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

More configuration options.

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [x] Create actor for snapshot creation
- [x] Add periodic snapshots
- [ ] Write snapshot to tmp file
- [ ] Check consistency between `kura` and snapshot
- [ ] Save `finalized_wsv` instead of `wsv`

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
        Created At 2023-08-16 11:07:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3813" class=".btn">#3813</a>
            </td>
            <td>
                <b>
                    [refactor] #3794: Differentiate between smart contract and trigger entrypoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span><span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

- Added `iroha_trigger` crate under `wasm/trigger` directory
- Removed `get_authority()` wasm imports
- Added payloads for smart contract and trigger and corresponging imports
- Removed entrypoint attribute parsing, arguments are mandatory now
- Removed `derive_primitives` crate because it becomed useless and can be replaced with `darling` crate if needed

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3794 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

- Smart contracts and triggers now also follow the idea of payloads, which makes argument expanding easier
- No useless `derive_primitives` crate
- Less thinking when writing triggers and smart contracts, because you don't need to worry about macro attributes

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

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
        Created At 2023-08-15 11:36:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3812" class=".btn">#3812</a>
            </td>
            <td>
                <b>
                    Bump tornado from 6.3.2 to 6.3.3 in /docs/source
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [tornado](https://github.com/tornadoweb/tornado) from 6.3.2 to 6.3.3.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/tornadoweb/tornado/blob/master/docs/releases.rst">tornado's changelog</a>.</em></p>
<blockquote>
<h1>Release notes</h1>
<p>.. toctree::
:maxdepth: 2</p>
<p>releases/v6.3.3
releases/v6.3.2
releases/v6.3.1
releases/v6.3.0
releases/v6.2.0
releases/v6.1.0
releases/v6.0.4
releases/v6.0.3
releases/v6.0.2
releases/v6.0.1
releases/v6.0.0
releases/v5.1.1
releases/v5.1.0
releases/v5.0.2
releases/v5.0.1
releases/v5.0.0
releases/v4.5.3
releases/v4.5.2
releases/v4.5.1
releases/v4.5.0
releases/v4.4.3
releases/v4.4.2
releases/v4.4.1
releases/v4.4.0
releases/v4.3.0
releases/v4.2.1
releases/v4.2.0
releases/v4.1.0
releases/v4.0.2
releases/v4.0.1
releases/v4.0.0
releases/v3.2.2
releases/v3.2.1
releases/v3.2.0
releases/v3.1.1
releases/v3.1.0
releases/v3.0.2
releases/v3.0.1
releases/v3.0.0
releases/v2.4.1
releases/v2.4.0
releases/v2.3.0
releases/v2.2.1
releases/v2.2.0</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tornadoweb/tornado/commit/e4d698433b44f350d4908da9ca2cac475c92dfdc"><code>e4d6984</code></a> Merge pull request <a href="https://redirect.github.com/tornadoweb/tornado/issues/3307">#3307</a> from bdarnell/branch6.3</li>
<li><a href="https://github.com/tornadoweb/tornado/commit/6a9e6fbaf7830b3edae68805211f35f5954292ab"><code>6a9e6fb</code></a> ci: Don't test py312 in branch6.3</li>
<li><a href="https://github.com/tornadoweb/tornado/commit/5c8a9a4fa792f8b18bd26bc7a8335e3bbe837852"><code>5c8a9a4</code></a> Set version to 6.3.3</li>
<li><a href="https://github.com/tornadoweb/tornado/commit/7dfe8b597f2d179334d7b528f61e9449ac131273"><code>7dfe8b5</code></a> httpserver_test: Add ExpectLog to fix CI</li>
<li><a href="https://github.com/tornadoweb/tornado/commit/217295b1dd30f556ea374d62007f6821688f00f0"><code>217295b</code></a> http1connection: Make content-length parsing more strict</li>
<li><a href="https://github.com/tornadoweb/tornado/commit/e3aa6c5e2943242d8ab25448c2798365b3cb9945"><code>e3aa6c5</code></a> Merge pull request <a href="https://redirect.github.com/tornadoweb/tornado/issues/3267">#3267</a> from bdarnell/branch6.3</li>
<li>See full diff in <a href="https://github.com/tornadoweb/tornado/compare/v6.3.2...v6.3.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tornado&package-manager=pip&previous-version=6.3.2&new-version=6.3.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/iroha/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-14 23:34:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3810" class=".btn">#3810</a>
            </td>
            <td>
                <b>
                    [release]: RC19
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Checklist
- [ ] Tests pass
- [x] All crates compile individually
- [x] Changelog
- [x] SDKs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-14 08:02:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3809" class=".btn">#3809</a>
            </td>
            <td>
                <b>
                    [documentation]: Release roadmap
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                The proposed release roadmap submitted for review as a recommendation. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-13 20:17:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3808" class=".btn">#3808</a>
            </td>
            <td>
                <b>
                    [fix] #3529: Fix topology for 3 or less peers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Make `Topology` methods consistent with each other and add bunch of tests.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3529 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Work properly.

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### How to test

1. Run tests

```bash
cargo test --package iroha_core --lib -- sumeragi::network_topology::tests --nocapture 
```

2. Startup iroha with 1-3 peers
```bash
# build iroha
cargo build

# run iroha network
./scripts/test_env 1-3
```

### Checklist

- [x]: Fix topology methods to be consistent
- [x]: Add test to verify

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
        Created At 2023-08-13 11:43:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3807" class=".btn">#3807</a>
            </td>
            <td>
                <b>
                    [documentation]: Formalise the release process
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Added two documents describing the release process and cadence recommendations. 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-12 22:23:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3806" class=".btn">#3806</a>
            </td>
            <td>
                <b>
                    [fix] #3805: Fix iroha graceful shutdown 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Fix shutdown of iroha.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3805 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Iroha shutdown correctly.

### How to test

Check original issues for steps to reproduce.

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
        Created At 2023-08-12 11:26:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3804" class=".btn">#3804</a>
            </td>
            <td>
                <b>
                    [refactor] #3791: Wasm entrypoint payloads
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

Two tasks done.

- Entrypoint name constants moved to the data model
- These constants used on Iroha and Wasm side
- Introduced payloads for different entrypoints

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

- Closes #3757
- Closes #3791
- Openned #3794 
<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

- Better code structure
- Easy to modify entrypoint input arguments

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

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
        Created At 2023-08-11 14:44:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3803" class=".btn">#3803</a>
            </td>
            <td>
                <b>
                    [documentation] #3802: Unicode "kagami crypto" seed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

A small Kagami help update

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

Closes #3802

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
        Created At 2023-08-11 09:13:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3795" class=".btn">#3795</a>
            </td>
            <td>
                <b>
                    [documentation]: Add Configuration RFC document
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Documentation</span><span class="chip">config-changes</span>
            </td>
            <td>
                I think this place is the most convenient to gather the team's feedback.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-11 00:47:21 +0000 UTC
    </div>
</div>

