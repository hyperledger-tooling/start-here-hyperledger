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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2673" class=".btn">#2673</a>
            </td>
            <td>
                <b>
                    test(cmd-api-server): fix CVE-2023-37903 - vm2 Sandbox Escape vulnerability
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There is no fix for the vm2 package's vulnerability and it is also no longer
maintained so a fix is not coming either.
Based on this and the fact that artillery's newer updates also did not
move away from using vm2 (as a transitive dependency) it is best to
just delete the artillery based benchmark for now. The longer term
and more robust solution is probably to have JMeter tests defined.
The downside of this is that it is harder to maintain them because
it's not NodeJS/Typescript technology stack but we already suffer
from this due to needing the JVM for Corda development tasks
therefore it is not as big of an overhead as it seems.

https://github.com/hyperledger/cacti/issues/2672

Fixes #2671

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-10 05:21:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2670" class=".btn">#2670</a>
            </td>
            <td>
                <b>
                    docs(examples): fix Mongoose Prototype Pollution vulnerability
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Both mongoose and the mongodb NodeJS driver dependency appeared to be
completely unused so instead of upgrading I just removed them.

Fixes #2669

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-10 04:55:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2668" class=".btn">#2668</a>
            </td>
            <td>
                <b>
                    docs(example-cbdc-bridging-backend): fix CVE-2020-36632
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Upgraded hardhat to newer versions which don't depend on flat at all.

Fixes #2667

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-10 04:24:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2666" class=".btn">#2666</a>
            </td>
            <td>
                <b>
                    docs(examples): fix CVE-2022-37601 - upgrade to Angular v16
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The new versions allow for loader-utils to be upgraded to non-vulnerable
versions so these are now fixed:

CVE ID: CVE-2022-37601
GHSA ID: GHSA-76p3-8jx3-jpfq

https://github.com/hyperledger/cacti/security/dependabot/257
https://github.com/advisories/GHSA-76p3-8jx3-jpfq

Fixes #2665

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-10 03:58:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2664" class=".btn">#2664</a>
            </td>
            <td>
                <b>
                    chore(deps): upgrade @lerna-lite/* to v2.5.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In addition to the @lerna-lite upgrade:
1. Also upgraded @commitlint/* to the current latest
2. Deleted some npm scripts that were not used anymore.
3. The canary publish script no longer run the CI (it was a huge overhead)

Fixes #2663

[skip ci]

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-10 03:06:35 +0000 UTC
    </div>
</div>

