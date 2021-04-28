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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2760" class=".btn">#2760</a>
            </td>
            <td>
                <b>
                    refactor: cleanup JSON-LD contexts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR:
* simplifies new JSON-LD document loader:
  - support for `WithContextFS` was removed (in practice it didn't justify itself)
  - "core" set of embedded contexts was defined (extra contexts can be preloaded using `WithExtraContexts`)
* replaces the following contexts:
  - `https://trustbloc.github.io/context/vc/credentials-v1.jsonld` -> `https://w3id.org/security/jws/v1`
  - `https://trustbloc.github.io/context/vc/examples-v1.jsonld` -> `https://w3id.org/vc-revocation-list-2020/v1` (only in BDD tests - this allows to remove it from the main embedded set)

Closes #2751

Signed-off-by: Andriy Holovko <andriy.holovko@gmail.com>



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-27 10:57:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2759" class=".btn">#2759</a>
            </td>
            <td>
                <b>
                    feat: vc wallet EDV storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - if wallet user provides EDV settings during profile creation for
storage then wallet will create internal EDV client instance for storing
wallet contents
- for now, encryption and MAC key IDs has to be provided by client user
during profile creation/update
- closes #2757

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-26 22:46:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2755" class=".btn">#2755</a>
            </td>
            <td>
                <b>
                    fix: presentation-exchange schema.uri matching
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">aip 2.0</span><span class="chip">bug</span>
            </td>
            <td>
                The `schema.uri` in presentation definitions should be the full URI to the type's definition (jsonschema or jsonld), not just the context. [Reference](https://github.com/decentralized-identity/presentation-exchange/issues/134#issuecomment-721624167).

TODO - #2756 

Signed-off-by: George Aristy <george.aristy@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-26 15:13:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2753" class=".btn">#2753</a>
            </td>
            <td>
                <b>
                    fix: presexch - CreateVP() matching schema URI algo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">aip 2.0</span><span class="chip">bug</span>
            </td>
            <td>
                CreateVP() was matching the definitions schema.uri against the VC's credentialSchema property instead of the context.

Reference: [this thread](https://github.com/decentralized-identity/presentation-exchange/issues/134#issuecomment-721624167).

Signed-off-by: George Aristy <george.aristy@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-22 19:28:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2750" class=".btn">#2750</a>
            </td>
            <td>
                <b>
                    chore(deps): bump ssri from 6.0.1 to 6.0.2 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [ssri](https://github.com/npm/ssri) from 6.0.1 to 6.0.2.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/npm/ssri/blob/v6.0.2/CHANGELOG.md">ssri's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/zkat/ssri/compare/v6.0.1...v6.0.2">6.0.2</a> (2021-04-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>backport regex change from 8.0.1 (<a href="https://github.com/zkat/ssri/commit/b30dfdb">b30dfdb</a>), closes <a href="https://github-redirect.dependabot.com/zkat/ssri/issues/19">#19</a></li>
</ul>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/npm/ssri/commit/b7c8c7c61db89aeb9fbf7596c0ef17071bc216ef"><code>b7c8c7c</code></a> chore(release): 6.0.2</li>
<li><a href="https://github.com/npm/ssri/commit/b30dfdb00bb94ddc49a25a85a18fb27afafdfbb1"><code>b30dfdb</code></a> fix: backport regex change from 8.0.1</li>
<li>See full diff in <a href="https://github.com/npm/ssri/compare/v6.0.1...v6.0.2">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~nlf">nlf</a>, a new releaser for ssri since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ssri&package-manager=npm_and_yarn&previous-version=6.0.1&new-version=6.0.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-go/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-22 13:27:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2749" class=".btn">#2749</a>
            </td>
            <td>
                <b>
                    feat: auth based access wallet store
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - for upcoming EDV integration, wallet interfaces expectes auth token
for accessing wallet contents too.
- `storage.openStore()` occurs during `wallet.Open()` and `store.cloe()`
occurs during `wallet.Close()`
- wallet open will unlock key manager and open database.
- wallet close will remove keyemaner and close database.
- all wallet interfaces now requires auth token.
- wallet content based VDR will expect auth token.
- Closes #2745

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-22 11:34:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2748" class=".btn">#2748</a>
            </td>
            <td>
                <b>
                    feat: Add error messages to providers that don't support query options
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - These new error messages will help ensure that someone won't get unexpected results when using those options in a Query on a storage provider that doesn't support them.
- The unit tests have been updated to avoid calling the new common storage Query tests that use those unsupported options.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-21 21:44:09 +0000 UTC
    </div>
</div>

