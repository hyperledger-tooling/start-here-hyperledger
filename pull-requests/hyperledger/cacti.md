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

