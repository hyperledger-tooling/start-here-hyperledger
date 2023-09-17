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
                PR <a href="https://github.com/hyperledger/cacti/pull/2694" class=".btn">#2694</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump protobufjs from 6.11.3 to 6.11.4 in /weaver/samples/fabric/fabric-cli
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [protobufjs](https://github.com/protobufjs/protobuf.js) from 6.11.3 to 6.11.4.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/protobufjs/protobuf.js/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=protobufjs&package-manager=npm_and_yarn&previous-version=6.11.3&new-version=6.11.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-09-17 01:29:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2692" class=".btn">#2692</a>
            </td>
            <td>
                <b>
                    docs(weaver): tutorial documentation updates and additions of license declarations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Fixed various links, path names, and package names, and corrected typos, in the Weaver tutorial documents. This was done after following the instructions outlined in the docs to manually run sample applications.
- Added Apache-2 license declarations to various source files in the `weaver` folder where they were missing. The main `weaver` folder already contains a `LICENSE.md` file, so this just covers all of our bases.
- Updated README instructions in various folders, wherever they were out of date.
- Updated version numbers in some template configuration files to `2.0.0-alpha.1`.

There is no code change in this PR. Just changes in Markdown files and addition of comments to source files.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-15 14:45:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2690" class=".btn">#2690</a>
            </td>
            <td>
                <b>
                    build(corda-sample): upgrade corda token sdk version to 1.2.5 to fix …
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …the build

This fixes the failing corda (weaver part) workflows.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-14 05:17:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2687" class=".btn">#2687</a>
            </td>
            <td>
                <b>
                    docs(examples): fix CVE-2022-25858 - Terser insecure regular expression ReDoS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [skip ci]

Fixes #2686

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-11 22:27:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2685" class=".btn">#2685</a>
            </td>
            <td>
                <b>
                    fix(cmd-socketio-server): fix Prototype Pollution in nconf
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                Depends on #2562 - build(deps): fix npm (grpc) build on NodeJS v20.4.0

Fixes #2684

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-11 21:24:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2683" class=".btn">#2683</a>
            </td>
            <td>
                <b>
                    fix(cmd-api-server): fix CVE-2023-36665 protobufjs Prototype Pollution vuln
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Upgraded all imports of protobufjs to non-vulnerable
versions (v7.2.5)

Fixes #2682

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-11 20:56:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2681" class=".btn">#2681</a>
            </td>
            <td>
                <b>
                    build(codegen): fix URL of OpenAPI generator jar v6.6.0 not 6.3.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [skip ci]

Fixes #2680

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-10 18:14:53 +0000 UTC
    </div>
</div>

