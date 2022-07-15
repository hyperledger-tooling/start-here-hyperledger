---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3278" class=".btn">#3278</a>
            </td>
            <td>
                <b>
                    chore(deps): bump actions/setup-node from 2.4.0 to 3.4.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [actions/setup-node](https://github.com/actions/setup-node) from 2.4.0 to 3.4.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/setup-node/releases">actions/setup-node's releases</a>.</em></p>
<blockquote>
<h2>Fix pnpm output and node-version  output issues</h2>
<p>In scope of this release we fixed bugs related to the pnpm 7.5.1 output issue from <code>pnpm store path</code> <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/545">actions/setup-node#545</a>. Moreover we fixed the issue with falling on node-version output <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/540">actions/setup-node#540</a>.</p>
<h2>Add support for asdf format and update actions/cache version to 3.0.0</h2>
<p>In scope of this release we updated <code>actions/cache</code> package as the new version contains fixes for <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/526">caching error handling</a>. Moreover, we added support for asdf format as Node.js version file <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/373">actions/setup-node#373</a>. Besides, we introduced new output <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/534">node-version</a> and added <code>npm-shrinkwrap.json</code> to dependency file patterns: <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/439">actions/setup-node#439</a></p>
<h2>Add support for lts/-n aliases</h2>
<p>In scope of this release we added support for <code>lts/-n</code> aliases, improve logic for <code>current</code>, <code>latest</code> and <code>node</code> aliases to handle them from <code>toolcache</code>, update <code>ncc</code> package.</p>
<h3>Support of lts/-n aliases</h3>
<ul>
<li>Related pull request: <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/481">actions/setup-node#481</a></li>
<li>Related issue: <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/26">actions/setup-node#26</a></li>
</ul>
<pre lang="yaml"><code>steps:
- uses: actions/checkout@v3
- uses: actions/setup-node@v3
  with:
    node-version: lts/-1
- run: npm ci
- run: npm test
</code></pre>
<h3>Minor improvements</h3>
<ul>
<li>Update zeit/ncc to vercel/ncc: <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/476">actions/setup-node#476</a></li>
<li>Get latest version from cache if exists: <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/496">actions/setup-node#496</a></li>
</ul>
<h2>Add current, node, latest aliases</h2>
<p>In scope of this release we added new aliases to install the latest Node.js version. <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/483">actions/setup-node#483</a></p>
<pre lang="yml"><code>steps:
- uses: actions/checkout@v3
- uses: actions/setup-node@v3
  with:
    node-version: current
- run: npm ci
- run: npm test
</code></pre>
<h2>Update actions/cache version to 2.0.2</h2>
<p>In scope of this release we updated <code>actions/cache</code> package as the new version contains fixes related to GHES 3.5 (<a href="https://github-redirect.dependabot.com/actions/setup-node/pull/460">actions/setup-node#460</a>)</p>
<h2>Add caching support on GHES 3.5</h2>
<p>In scope of this release we added <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/452">support for caching from GHES 3.5</a> and fixed download issue for files &gt; 2GB during restore. Besides, we updated <code>actions/cache</code> dependency to 2.0.0 version.</p>
<h2>v3.0.0</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/setup-node/commit/2fddd8803e2f5c9604345a0b591c3020ee971a93"><code>2fddd88</code></a> fixing pnpm output issue (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/545">#545</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/ad8542ca5eddfadd434c12500073d0cfe51ca1c7"><code>ad8542c</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/540">#540</a> from dmitry-shibanov/fix-error-node-version</li>
<li><a href="https://github.com/actions/setup-node/commit/3d11add77113802f5dc907ae13379fa7ffdcd839"><code>3d11add</code></a> remove unused import</li>
<li><a href="https://github.com/actions/setup-node/commit/072a2e3b100f5d9394c602616700b044ce5e72f8"><code>072a2e3</code></a> add trim and silent true</li>
<li><a href="https://github.com/actions/setup-node/commit/28ad38fe0624edc69ffde19aa0a6b8be0573641f"><code>28ad38f</code></a> add try catch</li>
<li><a href="https://github.com/actions/setup-node/commit/48de4c13f6f686eebe0d350838793fffd4421b26"><code>48de4c1</code></a> change to streams</li>
<li><a href="https://github.com/actions/setup-node/commit/aab7cc882a63a6e74f0d36e92552d03d190d4e7e"><code>aab7cc8</code></a> add silent</li>
<li><a href="https://github.com/actions/setup-node/commit/5b949b50c3461bbcd5a540b150c368278160234a"><code>5b949b5</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/373">#373</a> from ganta/add-support-for-asdf-format-as-node-versio...</li>
<li><a href="https://github.com/actions/setup-node/commit/09ba51f18e18a3756fea1f54d09c6745c064491d"><code>09ba51f</code></a> README.md: Encourage testing on current Node.js (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/533">#533</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/b3ca1ac971f58028968bf4f3199547ade2bb277d"><code>b3ca1ac</code></a> Support npm-shrinkwrap.json out-of-the-box (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/439">#439</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/actions/setup-node/compare/v2.4.0...v3.4.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=actions/setup-node&package-manager=github_actions&previous-version=2.4.0&new-version=3.4.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-15 08:16:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3277" class=".btn">#3277</a>
            </td>
            <td>
                <b>
                    feat: add did document support for alsoKnownAs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Chris Abernethy <brownoxford@gmail.com>

**Title:**
Add `alsoKnownAs` support to DID document

**Description:**
Implement support for `alsoKnownAs` DID document element [as described in DID Core v1](https://www.w3.org/TR/did-core/#dfn-alsoknownas)

**Summary:**
Add `AlsoKnownAs` element to `did.Doc` and populate value in `did.ParseDocument()`
Add `AlsoKnownAs` element to `did.rawDoc` and populate value in `did.Doc.JSONBytes()`
Add `did.populateRawAlsoKnownAs()` helper function to convert `alsoKnownAs` from `[]string` to `[]interface{}`
Add `alsoKnownAs` to schemas used for DID Schema Validation


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-14 16:44:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3276" class=".btn">#3276</a>
            </td>
            <td>
                <b>
                    Feat split wallet command
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
Split wallet command.

**Summary:**

Factor walletlite.Command form vcwallet.Command. It can now be used in the lite version of an agent that does not require didcomm functionality.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-14 11:10:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3275" class=".btn">#3275</a>
            </td>
            <td>
                <b>
                    feat: CL Anoncreds Crypto API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
CL Anoncreds Crypto API

**Description:**

- This is the second PR to support CL in `af-go` [#180](https://github.com/hyperledger/aries-framework-go/issues/180)
- This PR adds support for CL Anoncreds on Crypto API level (currently, for `tinkcrypto`)
- This PR contains implementation of CL for `tinkcrypto`
- `remotecrypto` changes will be introduced in the one of the latest PRs

**Summary:**

- Extended Crypto API with CL methods
- Adopted `libursa` CL primitives for `tinkcrypto` implementation
- Added `ursa` CL verifier functionality 
- Added stubs for `remotecrypto` and `tinkcrypto` for the case where no `ursa` installed
- Added unit tests
- Minor refactoring


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-13 15:02:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3272" class=".btn">#3272</a>
            </td>
            <td>
                <b>
                    refactor: change type of Forward.Msg from byte array to Envelope stru…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
Change Msg field of `Forward` model. Make nested packed forwards while creating forward message

**Summary:**

- Change Msg field of `Forward` from byte array to `Envelope` structure as defined in [protocol](https://github.com/hyperledger/aries-rfcs/blob/main/concepts/0094-cross-domain-messaging/README.md#corerouting10forward)
- Make nested packed forwards(for each routing key) while creating forward message


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-11 12:08:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3271" class=".btn">#3271</a>
            </td>
            <td>
                <b>
                    feat: CL Anoncreds tink primitives
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
CL Anoncreds tink primitives

**Description:**
- This is the first PR to support CL Anoncreds in Aries-framework-go [#180](https://github.com/hyperledger/aries-framework-go/issues/180).
- This PR addresses support of CL Anoncreds on the think crypto primitives level.
- Next PRs will add support for CL crypto to the `pkg/crypto/api` API interface and `pkg/kms` (separate PRs for each).
- CL Anoncreds support is based on the [ursa-wrapper-go](https://github.com/hyperledger/ursa-wrapper-go) as an optional dependency (under the `ursa` build tag).
- Please note, that  [ursa-wrapper-go](https://github.com/hyperledger/ursa-wrapper-go) required `libursa` lib to be installed, that's why `ursa` build tag has been introduced.

**Summary:**
- Adds [ursa-wrapper-go](https://github.com/hyperledger/ursa-wrapper-go) as an optional dependency (under the `ursa` build tag).
- Adds tink crypto primitives and keys for the Issuance flow 
- Adds a separate make unit-test-ursa target 
- Adds a separate job in the CI pipeline to run unit tests with the ursa build tag. As `libursa` is required, the CI job for the `ursa` tag is run in a container (ghcr.io/hyperledger/ursa-wrapper-go/uwg-build for now) where libursa is already installed.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-11 06:25:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3270" class=".btn">#3270</a>
            </td>
            <td>
                <b>
                    feat: add ext db packages to REST Agent (#3269)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ana Maria Franco <afrancoc2000@gmail.com>

**Title:**
Adding extended database packages to the Rest Agent

**Description:**
The Rest Agent doesn't have an easy way to use the [extended package databases](https://github.com/hyperledger/aries-framework-go-ext/tree/ce8776c10037404f5c31a67aced0df6828bc4c28), so, I'm adding the posibility to use them in here.

[Issue 3269](https://github.com/hyperledger/aries-framework-go/issues/3269)

**Summary:**

I'm adding support for the Rest Agent to: couchdb, mongodb, mysql, postgresql, from the [aries-framework-go-ext](https://github.com/hyperledger/aries-framework-go-ext) package, and updating the docs.

Also I ran `go mod tidy -go=1.16 && go mod tidy -go=1.17` and updated the go.mod keeping compatibility with go 1.16. Not sure if compatibility with go 1.16 is still wanted.



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-09 14:28:59 +0000 UTC
    </div>
</div>

