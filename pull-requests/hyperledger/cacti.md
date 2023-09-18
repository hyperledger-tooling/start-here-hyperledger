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
                PR <a href="https://github.com/hyperledger/cacti/pull/2704" class=".btn">#2704</a>
            </td>
            <td>
                <b>
                    build(setup): remove install-yarn and document new yarn setup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [skip ci]

Fixes #2582

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-18 03:33:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2703" class=".btn">#2703</a>
            </td>
            <td>
                <b>
                    chore(release): set openapi.json versions to v2.0.0-alpha.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Ran the bump script to set all the versions to v2.0.0-alpha.1
2. Ran `yarn codegen` to update the generated code based on the updated
versions (bumps the version in the docs, code comments etc.)

[skip ci]

Fixes #2702

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-18 02:09:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2699" class=".btn">#2699</a>
            </td>
            <td>
                <b>
                    docs(whitepaper): temporarily remove whitepaper
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Removes all the contents except for the document title
2. Updates the version to v2.0
3. Updates the Hyperledger Foundation logo to the current latest as of 2023
4. Adds a disclaimer about the fact that the whitepaper is
being re-worked and where to find the old version.

Related to, but does not conclude the work of #2691

[skip ci]

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-17 23:54:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2698" class=".btn">#2698</a>
            </td>
            <td>
                <b>
                    style: fix unexpected any linter warnings in extendWithT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Used the suggester Record<string, unknown> to replace any

[skip ci]

Closes: #2675
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-17 23:01:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2697" class=".btn">#2697</a>
            </td>
            <td>
                <b>
                    chore: fix linter warning in CreateCorsMiddleware
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Imported CorsOptionsDelegate and CorsRequest and typed corsOptionsDelegate to it

Closes: #2674

Possibly not a chore, but a style issue

[skip ci]
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-17 22:27:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2696" class=".btn">#2696</a>
            </td>
            <td>
                <b>
                    style: fix unexpected any linter w in startCockpitFileServer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The linter warning for unexpected any was fixed with Record<string, unknown>

[skip ci]

Closes: #2677

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-17 21:41:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2695" class=".btn">#2695</a>
            </td>
            <td>
                <b>
                    style: fixes Unexpected any linter W in getHelpText()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The linter warning was fixed with Record<string, unknown> and the types inside the function have been corrected.
The other 7 lines are just linter-errors for empty spaces, that where corrected, although that was not part of the issue, i hope it was ok.

[skip-ci]

Closes: #2678
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-17 19:55:12 +0000 UTC
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

