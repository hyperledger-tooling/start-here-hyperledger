---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/422" class=".btn">#422</a>
            </td>
            <td>
                <b>
                    refactor(redux-store)/deleteProof
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - renamed wrong function name from: `ProofThunks.deleteCredential` -> `ProofThunks.deleteProof`

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-10 11:13:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/421" class=".btn">#421</a>
            </td>
            <td>
                <b>
                    feat(redux-store): delete credentialRecord and proofRecord
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Able to delete credentialRecord and proofRecord like the connectionRecord
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-10 09:54:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/420" class=".btn">#420</a>
            </td>
            <td>
                <b>
                    Documentation - Agent setup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As usual, needs some linguistics review
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-10 02:47:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/419" class=".btn">#419</a>
            </td>
            <td>
                <b>
                    Fix/mediator transports
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR has code that corrects issues related to mediation.
Corrections
- multiple restarts with the same mediation invitation 
- second sorting of connection transport services based on inbound services
- multiple outbound transport support
  - add transport is now register transport, which allows using multiple types of transport.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-05 14:31:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/417" class=".btn">#417</a>
            </td>
            <td>
                <b>
                    build(deps): bump tar from 4.4.13 to 4.4.15
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [tar](https://github.com/npm/node-tar) from 4.4.13 to 4.4.15.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/npm/node-tar/commit/843c897e6844f70a34bb115df6c8a9b60112aaf5"><code>843c897</code></a> 4.4.15</li>
<li><a href="https://github.com/npm/node-tar/commit/46fe35083e2676e31c4e0a81639dce6da7aaa356"><code>46fe350</code></a> Remove paths from dirCache when no longer dirs</li>
<li><a href="https://github.com/npm/node-tar/commit/df3aa4d10253a886be82519acb901b446ca3feeb"><code>df3aa4d</code></a> 4.4.14</li>
<li><a href="https://github.com/npm/node-tar/commit/6d2801396fbad917ab8332ec8e91ff3d15bc22c6"><code>6d28013</code></a> add publishConfig tag</li>
<li><a href="https://github.com/npm/node-tar/commit/efc6bb0dbd54df8c7285d7aac12bba959b8387a6"><code>efc6bb0</code></a> fix: strip absolute paths more comprehensively</li>
<li>See full diff in <a href="https://github.com/npm/node-tar/compare/v4.4.13...v4.4.15">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tar&package-manager=npm_and_yarn&previous-version=4.4.13&new-version=4.4.15)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-javascript/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-03 21:47:10 +0000 UTC
    </div>
</div>

