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
                PR <a href="https://github.com/hyperledger/cacti/pull/2708" class=".btn">#2708</a>
            </td>
            <td>
                <b>
                    fix(docs): add Pull Request Template
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes: #91

adds Pull Request Template on the root directory as guideline for contributors.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-19 05:34:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2707" class=".btn">#2707</a>
            </td>
            <td>
                <b>
                    feat(cactus-plugin-ledger-connector-ethereum): add stress test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                - Return JSON error before checking for Error instance in safeStringifyException
    (for cases when custom errror extends `Error` with `toJSON()` method)
- Move artillery dependency up to the root (since its common tool depdenecy)
- Add web3js http/ws provider options to connector.
- Make http provider optional (can run on ws web3js provider only)
- Don't register async endpoints when WS provider is not available.
- Return 400 for invalid responses from ethereum ledger (to distinguish from connector errors)
- In docker `geth-all-in-one` allow overwriting of default options when starting the ledger.
- Add artillery stress test scripts
    - Template config and artillery functions file
    - Common environment setup file
    - CLI for running the test environment on a separate machine.
    - Jest test to run quickly stress test on same machine.
    - 
Depends on #2631

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-18 10:34:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2706" class=".btn">#2706</a>
            </td>
            <td>
                <b>
                    fix: fix deprecation of deb.nodesource.com/setup_16.x
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Change Description:**

In the Dockerfile, the issue related to NodeJS was addressed by updating the NodeJS installation method to use the new NodeSource installation method. The previous method using `curl -sL https://deb.nodesource.com/setup_16.x | bash -` had become deprecated, so the new method was applied for compatibility with the latest practices.

The specific changes made in the Dockerfile are as follows:

1. Removed the old installation method for NodeJS:

   ```Dockerfile
   # Removed the deprecated NodeJS installation method
   # RUN curl -sL https://deb.nodesource.com/setup_16.x | bash -
   ```

2. Added the new NodeSource installation method:

   ```Dockerfile
   # Added the new NodeSource installation method for NodeJS
   RUN curl -fsSL https://deb.nodesource.com/gpgkey/nodesource-repo.gpg.key | gpg --dearmor -o /usr/share/keyrings/nodesource-archive-keyring.gpg \
       && echo "deb [arch=amd64 signed-by=/usr/share/keyrings/nodesource-archive-keyring.gpg] https://deb.nodesource.com/node bionic main" | tee /etc/apt/sources.list.d/nodesource.list
   ```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-18 07:22:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2705" class=".btn">#2705</a>
            </td>
            <td>
                <b>
                    fix(security): vulnerabilities found in cactus-rust-compiler
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fix will ignore AsymmetricPrivateKey (private-key)

Fixes #2042
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-18 07:06:28 +0000 UTC
    </div>
</div>

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

[skip ci]

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

