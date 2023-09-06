---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2654" class=".btn">#2654</a>
            </td>
            <td>
                <b>
                    chore(tools): add script to strip out non-production sources
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                To run the script you can execute this on a shell:
    yarn tools:create-production-only-archive

The above will create a temporary clone of the project sources, then
delete a lot of the files that are documentation/test code (e.g. things
that do not go into production). Finally it zips the remaining files
together into something that includes a date & timestamp and the git
hash that the archive was generated from.

There were plans to make the generated zip file also encrypted, but this
is not supported by the library that we are using for compression. The
other library was not necessarily purely Javascript implemented and so
there was some reluctance to use it because of the huge overhead on the
the dependency installation process that we already have from packages
that use native code to satisfy their stated purpose.
So, with all that said, encrypting the .zip file is left as a to-do for
later. The issues tracking this feature are here:
1. https://github.com/cthackers/adm-zip/issues/259
2. https://github.com/cthackers/adm-zip/issues/398

Fixes #2652

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-06 01:29:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2653" class=".btn">#2653</a>
            </td>
            <td>
                <b>
                    feat: Add VSCode extension
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
        Created At 2023-09-02 17:40:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2649" class=".btn">#2649</a>
            </td>
            <td>
                <b>
                    build(deps): upgrade web3js-quorum to v22.4.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Upgraded to v22.4.0 but did not yet delete our hand-built typings
because the ones that v22.4.0 ships with are broken (do not match the
actual implementation forcing programmers to fight the compiler
needlessly)

Fixes #2648

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-31 19:35:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2647" class=".btn">#2647</a>
            </td>
            <td>
                <b>
                    build(deps): bump gopkg.in/yaml.v3 from 3.0.0-20200313102051-9f266ea9e77c to 3.0.0 in /weaver/sdks/fabric/go-sdk
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps gopkg.in/yaml.v3 from 3.0.0-20200313102051-9f266ea9e77c to 3.0.0.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=gopkg.in/yaml.v3&package-manager=go_modules&previous-version=3.0.0-20200313102051-9f266ea9e77c&new-version=3.0.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-30 13:59:51 +0000 UTC
    </div>
</div>

