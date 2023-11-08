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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1631" class=".btn">#1631</a>
            </td>
            <td>
                <b>
                    build(deps): use node's built-in fetch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As now our minimal supported node version is 18, which has a built-in fetch API, this is an attempt to get rid of external `node-fetch` dependency on `@aries-framework/core`.

Credits to @dependabot, who give us the idea!
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-07 20:44:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1630" class=".btn">#1630</a>
            </td>
            <td>
                <b>
                    build(deps): bump react-devtools-core from 4.27.6 to 4.28.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [react-devtools-core](https://github.com/facebook/react/tree/HEAD/packages/react-devtools-core) from 4.27.6 to 4.28.5.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/facebook/react/commits/HEAD/packages/react-devtools-core">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=react-devtools-core&package-manager=npm_and_yarn&previous-version=4.27.6&new-version=4.28.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-javascript/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-07 20:20:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1629" class=".btn">#1629</a>
            </td>
            <td>
                <b>
                    refactor(indy-sdk)!: remove indy-sdk package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Still WIP.

Removes the indy-sdk package and updates all code to now use only the new shared components. Still some work to do related to removing the usage of indy-sdk and making sure all tests work. But this is an initial step.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-07 05:40:15 +0000 UTC
    </div>
</div>

