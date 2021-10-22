---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1475" class=".btn">#1475</a>
            </td>
            <td>
                <b>
                    build(yarn): migrate from V1 to V3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We hope to solve issues with this that were plaguing contributors due to
bugs in the much older Yarn 1.x versions that we had to use because Yarn V2
had it's own set of problems when it came to linking the .bin folders for
child packages in a monorepo.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-22 07:28:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1474" class=".btn">#1474</a>
            </td>
            <td>
                <b>
                    test: skip corda v4.7 deploy test due to flakiness
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Corda</span><span class="chip">Flaky-Test-Automation</span><span class="chip">Tests</span>
            </td>
            <td>
                Related to #1473 but does NOT fix it, that is to come at a later point
in time when we have time for a full and proper diagnosis+fix.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-22 04:35:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1472" class=".btn">#1472</a>
            </td>
            <td>
                <b>
                    test: skip flaky fabric 2.2.x deploy cc from JS test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Fabric</span><span class="chip">Developer_Experience</span><span class="chip">Flaky-Test-Automation</span><span class="chip">Tests</span>
            </td>
            <td>
                This is related to #1471 (does not fix it though). In order to enable
faster CI/PR turnaround times we are aggressively eliminating (skipping)
flaky tests and creating issues in the backlog for fixing them later on.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-21 22:46:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1470" class=".btn">#1470</a>
            </td>
            <td>
                <b>
                    test(connector-corda): skip deploy-cordapp-jars-to-nodes-v4.8
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Flaky-Test-Automation</span>
            </td>
            <td>
                Related to #1469

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-21 19:51:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1467" class=".btn">#1467</a>
            </td>
            <td>
                <b>
                    docs: add SECURITY.md file to comply with the HL repo linter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span><span class="chip">Security</span>
            </td>
            <td>
                A 100% knockoff of the Fabric project's SECURITY.md file.

Closes: #662
Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 22:44:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1466" class=".btn">#1466</a>
            </td>
            <td>
                <b>
                    build: reset:node-modules script dry-run parameter dropped
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">dependencies</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                Epic facepalm once again, congratulations to Peter!

The reset:node-modules script had one job, which was to
delete all node_modules directories in the entire repo.
It was on the right track, but the --dry-run flag was forgotten
in among the CLI arguments so this whole time the script was
not working *at all* because of it. Just brilliant... :-)

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 22:39:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1464" class=".btn">#1464</a>
            </td>
            <td>
                <b>
                    feat(common): add Strings#isNonBlank()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span>
            </td>
            <td>
                Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-19 06:53:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1463" class=".btn">#1463</a>
            </td>
            <td>
                <b>
                    feat(plugin-keychain-memory-wasm): add WebAssmebly PoC
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adding a new keychain in-memory plugin that has it's implementation
written in Rust that is then compiled down to WebAssmebly via wasm-pack
and used by the wrapper Typescript code.

This is NOT meant for production because it stores everything in plain
text and also provides zero durability/persistence guarantees given that
it's only storing everything in memory.

The actual news here is that we have a plugin now written in Rust which
is the pre-cursor to us being able to do something similar with the
Weaver relay component as the next phase of a bigger PoC.

The reason why not the entire plugin is implemented in Rust is because
we are unable to hook up ExpressJS request handlers from the Rust code
as far as I could determine. See this link for further details on this:
https://rustwasm.github.io/book/reference/js-ffi.html#from-the-rust-side

Because of the above, the way it works is this:

        +--------+ API Request   +----------+
        | HTTP   |-------------->| ExpressJS|
        | Client |               +----------+
        +--------+               Method|
                                 Call  |
                                       v
        +---------+ Method Call  +----------+
        | Calling |------------->|JS Plugin |
        | Module  |              |Module    |
        +---------+              +----------+
                                   |get()
                                   |set()
                                   |has()
                                   |delete()
                +-------------+    |
                | Wasm Plugin |<---+
                | Module      |
                +-------------+
                        ^
                        |
                        |
                        v
           +------------------------+
           |Rust Native             |
           |HashMap<String, String> |
           +------------------------+

Resolves #1281

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-19 06:47:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1462" class=".btn">#1462</a>
            </td>
            <td>
                <b>
                    build(tools): upgraded sync-npm-deps script to globby v12
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Globby's newer versions use ESM modules which caused problems
when running our TS code with ts-node, the workarounds are now
in place so that the sync-npm-deps script that writes to
tsconfig.json can be used once more (though still not redcommended
because of other technical debt that was recently introduced to
the codebase in the form of non-uniform tsconfig.json files for
some packages)

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-19 01:32:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1460" class=".btn">#1460</a>
            </td>
            <td>
                <b>
                    fix(lint): fix issue #1360
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix warns for issue https://github.com/hyperledger/cactus/issues/1360

Fixes #1360
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-17 14:13:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1459" class=".btn">#1459</a>
            </td>
            <td>
                <b>
                    fix(lint): fix issue #1359
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes https://github.com/hyperledger/cactus/issues/1359 for lint issues in `src/test/typescript/integration/openapi/openapi-validation.test.ts`


#### Previous errors:
packages/cactus-plugin-keychain-vault/src/test/typescript/integration/openapi/openapi-validation.test.ts
  141:12  warning  Unexpected any. Specify a different type  @typescript-eslint/no-explicit-any
  160:16  warning  Unexpected any. Specify a different type  @typescript-eslint/no-explicit-any
  180:16  warning  Unexpected any. Specify a different type  @typescript-eslint/no-explicit-any
  200:16  warning  Unexpected any. Specify a different type  @typescript-eslint/no-explicit-any
  223:12  warning  Unexpected any. Specify a different type  @typescript-eslint/no-explicit-any
  247:12  warning  Unexpected any. Specify a different type  @typescript-eslint/no-explicit-any
  271:12  warning  Unexpected any. Specify a different type  @typescript-eslint/no-explicit-any
  295:12  warning  Unexpected any. Specify a different type  @typescript-eslint/no-explicit-any
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-17 13:50:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1458" class=".btn">#1458</a>
            </td>
            <td>
                <b>
                    ci: temporarily disable Fabric container image builds
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is necessary because they are being flaky again, potentially
due to the DockerHub rate limits.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-15 19:52:42 +0000 UTC
    </div>
</div>

