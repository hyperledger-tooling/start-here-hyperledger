---
layout: default
title: indy-sdk-react-native
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-sdk-react-native
---

# indy-sdk-react-native <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-sdk-react-native){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk-react-native/pull/17" class=".btn">#17</a>
            </td>
            <td>
                <b>
                    Feature/revocation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds recipient revocation capabilities for both Android and iOS:
    buildGetRevocRegDefRequest
    parseGetRevocRegDefResponse
    buildGetRevocRegDeltaRequest
    parseGetRevocRegDeltaResponse
    createRevocationState
This is a followup to #15. @TheTreek contributed the Android portions.
This fixes the types of the previous PR and readjusted the method positioning to align with Indy.

All commits should be signed. If there's still issues the repo may be checking for GCP signed keys, not DCO signoff. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-13 18:33:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk-react-native/pull/16" class=".btn">#16</a>
            </td>
            <td>
                <b>
                    Bump path-parse from 1.0.6 to 1.0.7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [path-parse](https://github.com/jbgutierrez/path-parse) from 1.0.6 to 1.0.7.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/jbgutierrez/path-parse/commits/v1.0.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=path-parse&package-manager=npm_and_yarn&previous-version=1.0.6&new-version=1.0.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk-react-native/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-13 01:58:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk-react-native/pull/15" class=".btn">#15</a>
            </td>
            <td>
                <b>
                    Android Revocation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added functions in android to support recipient revocation.

1. buildGetRevocRegDefRequest
2. parseGetRevocRegDefResponse
3. buildGetRevocRegDeltaRequest
4. parseGetRevocRegDeltaResponse
5. createRevocationState

Signed-off-by: Patrick Kenyon <treek.kenyon@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-07 01:21:16 +0000 UTC
    </div>
</div>

