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
                PR <a href="https://github.com/hyperledger/cactus/pull/898" class=".btn">#898</a>
            </td>
            <td>
                <b>
                    perf: leverage import type syntax to save on bundle size
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Core_API</span><span class="chip">Performance</span><span class="chip">dependent</span>
            </td>
            <td>
                ## Dependencies

Depends on #897 

## Commit to review

Author: Peter Somogyvari <peter.somogyvari@accenture.com>
Author Date: 2021-05-01 16:49:48 -0700
Committer: Peter Somogyvari <peter.somogyvari@accenture.com>
Committer Date: 2021-05-01 17:13:43 -0700 

perf: leverage import type syntax to save on bundle size

We can exclude ExpressJS from the core-api bundles because it is
designed to only ship interfaces for re-use by other packages.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-02 00:18:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/897" class=".btn">#897</a>
            </td>
            <td>
                <b>
                    feat(cmd-api-server): add Socket.IO as transport #297
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">API_Server</span><span class="chip">ConnectionChain</span><span class="chip">Core_API</span><span class="chip">dependent</span><span class="chip">enhancement</span>
            </td>
            <td>
                ## Dependencies

Depends on #896 

## Commit to review

Author: Peter Somogyvari <peter.somogyvari@accenture.com>
Committer: Peter Somogyvari <peter.somogyvari@accenture.com>
Date: 2021-05-01 17:12:11 -0700 

feat(api-client,cmd-api-server): add Socket.IO as transport #297

WORK IN PROGRESS

To-do:
1. Socket provider singleton on client side for connection multiplexing

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-02 00:16:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/896" class=".btn">#896</a>
            </td>
            <td>
                <b>
                    build: webpack ts-loader transpileOnly set to true
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Needed this because otherwise the perfectly valid Typescript code would
not compile when using TS loader in cases when multiple Cactus packages
were depending on types from certain dependencies (example both core-api
and the besu connector would depend on the socketio package and its
"Server" class would be claimed as incompatible by the TS loader
compilation process even when the source files for those types were byte
to byte the same (but the path was different to them because they
existed in different node_modules directories)

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-02 00:10:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/895" class=".btn">#895</a>
            </td>
            <td>
                <b>
                    build: remove npm dep. commitizen to avoid git-cz conflict
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Allegedly fixes the strange git-cz error encountered
while running "npm run commit"

(node:11594) UnhandledPromiseRejectionWarning: TypeError: Cannot convert undefined or null to object
    at Function.keys (<anonymous>)
    at runInteractiveQuestions (//node_modules/git-cz/dist/cz.js:576:10)
    at run (//node_modules/git-cz/dist/cz.js:157:11)
    at exports.prompter (//node_modules/git-cz/dist/cz.js:164:3)
    at //node_modules/commitizen/dist/commitizen/commit.js:598:9
    at //node_modules/fs-extra/lib/mkdirs/mkdirs.js:56:16
    at callback (//node_modules/graceful-fs/polyfills.js:295:20)
    at FSReqCallback.oncomplete (fs.js:184:5)

Hit the same issue, multiple times with it disappearing and then resurfacing with different versions as well, made no sense.

So, I started checking other things and found out that I also had commitizen installed which for some reason declares it's own, conflicting binary also called git-cz that (I'm guessing) may end up being hooked up to ./node_modules/.bin/git-cz randomly depending on the cookie crumbles when you run npm install (which I assume does as much as possible parallelized)

Uninstalled commitizen and right now it's working. Just a theory, but maybe it's right.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>


cc: @travis-payne @TonyRowntree 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-02 00:08:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/894" class=".btn">#894</a>
            </td>
            <td>
                <b>
                    chore(linter): fix warning in isIPluginWebService
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 21:24:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/892" class=".btn">#892</a>
            </td>
            <td>
                <b>
                    fix(github/workflows): dependent issues job name typo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span><span class="chip">dependencies</span>
            </td>
            <td>
                There was a typo in the first fix I attempted so now fixing the fix here
(hopefully)

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 21:13:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/884" class=".btn">#884</a>
            </td>
            <td>
                <b>
                    refactor(consortium-manual): move logic from endpoint to plugin class
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolve #429 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 15:39:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/883" class=".btn">#883</a>
            </td>
            <td>
                <b>
                    refactor(core-api): discontinue web service plugin aspect #350
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: TonyRowntree <33454202+TonyRowntree@users.noreply.github.com>

**Removed**
- WEB_SERVICE PluginAspect


**Added**
- BUSINESS_LOGIC PluginAspect

Resolve #350 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 15:37:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/880" class=".btn">#880</a>
            </td>
            <td>
                <b>
                    feat(api-server): publish API server docker image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">API_Server</span>
            </td>
            <td>
                Adding a hook to publish this to the Hyperledger DockerHub repo.


Resolve #345 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-28 15:47:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/879" class=".btn">#879</a>
            </td>
            <td>
                <b>
                    fix(connector-corda): container image kotlin compilation fails in model
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                This change fixes the compilation error kotlin was throwing when building the docker image.

BREAKING CHANGE: 🧨 We're now using the latest OpenAPI Generator CLI version of 2.2.6, so quite a few autogenerated files have been changed.

- Enums generated by OpenAPI are now lowercase.
- API Clients now need to instantiate a Configuration object and use that as a constructor param.
- Now using Integer as opposed to Number in the OpenAPI config to prevent an error when mapping to BigDecimal

Resolve #763
Resolve #584 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-28 09:49:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/878" class=".btn">#878</a>
            </td>
            <td>
                <b>
                    fix(whitepaper): fix rendering
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolve #339 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-28 07:50:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/875" class=".btn">#875</a>
            </td>
            <td>
                <b>
                    fix(connector-fabric): export IPluginLedgerConnectorFabricOptions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Exports IPluginLedgerConnectorFabricOptions from the Fabric Connector public API 

cc @petermetz 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-27 12:50:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/873" class=".btn">#873</a>
            </td>
            <td>
                <b>
                    docs(htlc-coordinator): added the flow diagram
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolve #603 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-27 06:52:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/870" class=".btn">#870</a>
            </td>
            <td>
                <b>
                    docs(meta): guidelnies for documentation authors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-26 22:46:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/867" class=".btn">#867</a>
            </td>
            <td>
                <b>
                    docs(vscode): added extensions.json file with recommended extensions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: TonyRowntree <33454202+TonyRowntree@users.noreply.github.com>

**Added**

- extensions.json file within the .vscode directory

**Updated**

- .gitignore file to allow extensions.json to be pushed to the repo

Resolve #863  
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-26 12:06:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/865" class=".btn">#865</a>
            </td>
            <td>
                <b>
                    feat(corda): prometheus exporter metrics integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Commit to be reviewed
---	

feat(corda): prometheus exporter metrics integration
	
	Primary Change
	1. The corda ledger connector plugin now includes the prometheus metrics exporter integration
	2. OpenAPI spec now has api endpoint for getting the prometheus metrics

	Refactorings that were also necessary to incorporate 1) and 2)
	3. GetPrometheusMetricsV1 class is created to handle the corresponding api endpoint
	4. IPluginLedgerConnectorCordaOptions interface in PluginLedgerConnectorCorda class now has a prometheusExporter object optional field
	5. The PluginLedgerConnectorCorda class has relevant functions to incorporate prometheus exporter
	6. Updated Readme.md about the prometheus exporter
	7. Updated the test case located at packages/cactus-plugin-ledger-connector-corda/src/test/typescript/integration/deploy-cordapp-jars-to-nodes.test.ts
	8. Updated the OpenAPI spec file to have run-transaction endpoint which currently returns NOT_IMPLEMENTED with 501 code.

Resolve #535

Signed-off-by: Jagpreet Singh Sasan <jagpreet.singh.sasan@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-26 09:37:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/864" class=".btn">#864</a>
            </td>
            <td>
                <b>
                    test(ci): fail ci.sh if git index is not empty
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                the script uses npm ci, which should not cause
any updates to the lock files, therefor currently
the git index is checked only at the end of the
script

Resolves https://github.com/hyperledger/cactus/issues/809

Signed-off-by: Hristiyan Ivanov <hristiyan.d.ivanov@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-26 06:18:27 +0000 UTC
    </div>
</div>

