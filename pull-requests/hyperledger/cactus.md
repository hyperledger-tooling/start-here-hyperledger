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
                PR <a href="https://github.com/hyperledger/cactus/pull/1249" class=".btn">#1249</a>
            </td>
            <td>
                <b>
                    feat(keychain-azure-kv): complete request handler and endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1010 

_______________________________________
This is might be a duplicate PR that Jeff's #1206 is working on, I'm opening a new PR since I do not have collaborator rights yet. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-20 15:31:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1244" class=".btn">#1244</a>
            </td>
            <td>
                <b>
                    feat(besu): support besu v21.1.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolve #982 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-19 12:28:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1243" class=".btn">#1243</a>
            </td>
            <td>
                <b>
                    feat(vault-keychain): add support for vault transit secret engine
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add support for following method to `PluginKeychainVault` class
- `transitSign` : sign digest using private key stored in vault server
- `transitNewKey` : create a new key
- `transitGetPub` : return `pem` encoded public key 
- `transitRotateKey` : rotate private key

For now it support `EC` (of size 256 , 384 , 521 ) only

Signed-off-by: Pritam Singh <pkspritam16@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-18 20:07:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1242" class=".btn">#1242</a>
            </td>
            <td>
                <b>
                    docs(tools): fix besu all-in-one docker-compose #1241
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span><span class="chip">Besu</span><span class="chip">dependencies</span>
            </td>
            <td>
                Fixes #1241

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-18 19:28:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1240" class=".btn">#1240</a>
            </td>
            <td>
                <b>
                    docs: update faq documentation and incorporate Quick-Start-Topics section
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span>
            </td>
            <td>
                Structure FAQ.md into two sections:
- Quick-Start Topics
- Other Topics

Adding a new topic for API-Server 'UnauthorizedError' to the Quick-Start Topics 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-18 12:27:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1238" class=".btn">#1238</a>
            </td>
            <td>
                <b>
                    fix(yarn-npm-replace): replace npm with yarn in Dockerfile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Improve Dockernization by replacement of npm with yarn.
This PR is a fix regarding Issue #1237
Signed-off-by: Shingo Fujimoto <shingo_fujimoto@fujitsu.com>

Update by Peter:
(this is the syntax that GitHub parses to link the issue and the PR together for automatic issue closure once the PR is merged)
Fixes #1237 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-18 03:28:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1235" class=".btn">#1235</a>
            </td>
            <td>
                <b>
                    test: reduce artillery runtime to 1 minute from 10
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1146

Signed-off-by: Youngone Lee <youngone.lee@accenture.com>

___________________________________________________________________________

Although the original issue mentioned that the artillery runtime was 10 minutes, it might have been at 5 minutes. I'm not sure if I've altered the correct code for this issue but I edited the avgLatency. Please let me know if there's something else I should have done!! 

It also looks like this testcase wasn't passing the tests (this was before I made any changes), do you want me to make a separate issue to fix the failing test cases? @petermetz 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-17 15:27:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1234" class=".btn">#1234</a>
            </td>
            <td>
                <b>
                    test: adding quorum multip test ledger Dockerfile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This code allows for building of the a quorum multi party docker image that allows for private transactions to be tested.

Related to #951 


Signed-off-by: Travis Payne <travis.payne@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-17 10:23:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1232" class=".btn">#1232</a>
            </td>
            <td>
                <b>
                    chore(deps): project-wide upgrade August, 2021
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">SPIKE</span><span class="chip">dependencies</span>
            </td>
            <td>
                1. Updated how Husky is configured to match the new version.
2. Had to migrate the custom checks tooling to Ecmascript Modules
because globby's latest version uses them and now we must too.
3. Restricted the custom checks to only run on NodeJS v14 and newer
because on Node v12 the custom checks do not work anymore due to
the ESM migration.

Dependencies that were NOT upgraded to the latest:
1. jose
2. express-openapi-validator
3. prettier

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-17 04:46:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1230" class=".btn">#1230</a>
            </td>
            <td>
                <b>
                    chore(release): publish v0.8.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-17 03:07:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1229" class=".btn">#1229</a>
            </td>
            <td>
                <b>
                    refactor(cmd-api-server): migrate container to ubuntu-20.04
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">API_Server</span><span class="chip">dependencies</span>
            </td>
            <td>
                1. Makes the base image of the API server ubuntu-20.04
2. Upgrades the NodeJS version to v16

Published a version of this commit to ghcr as well, built it 
with this command:

DOCKER_BUILDKIT=1 docker build \
  --build-arg NPM_PKG_VERSION=fix-1226 \
  -f ./packages/cactus-cmd-api-server/Dockerfile . \
  -t cas \
  -t cactus-api-server

Tagged as:
ghcr.io/hyperledger/cactus-cmd-api-server:2021-08-15--refactor-1222

Fixes #1222

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-16 05:33:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1228" class=".btn">#1228</a>
            </td>
            <td>
                <b>
                    fix(cmd-api-server): add missing deps remove unused ones #1226
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">API_Server</span><span class="chip">dependencies</span>
            </td>
            <td>
                Fixes #1226

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-16 04:53:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1225" class=".btn">#1225</a>
            </td>
            <td>
                <b>
                    fix(examples): front-end packages missing browserify polyfills #1224
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">dependencies</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                The webpack build done by the Angular CLI (ng) was broken due to a few
different issues combined together:
1. After upgrading to Angular v12 IE 11 is no longer supported which
necessitated the explicit configuration in the browserlist rc config
file accordingly so that the compilation process does not try to support
a browser for which the build is broken to begin with.
2. polyfills had to be added via customizing the webpack configuration
used by the Angular CLI internally which is now being done by using a
custom builder as specified in the angular.json file. This is the new
method of dealing with these kind of issues after the ng eject command
was deprecated a while back. The webpack.config.overrides.js files
that are beind added in this commit contain only the overrides (as the
name suggests) not the entire webpack configuration that the Angular
CLI uses internally to build the front end packages.

Fixes #1224

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-16 02:39:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1221" class=".btn">#1221</a>
            </td>
            <td>
                <b>
                    test: ensure .test suffix on mTLS tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span>
            </td>
            <td>
                These are likely the last test files that we have forgotten to
refactor to have a .test suffix which improves developer experience
on account of IDE support and easier filtering of files.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-14 03:56:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1220" class=".btn">#1220</a>
            </td>
            <td>
                <b>
                    ci: remove retries from ci.sh
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The tests are still not 100% stable, but a lot more stable and
the retries might not be needed anymore.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-14 03:44:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1219" class=".btn">#1219</a>
            </td>
            <td>
                <b>
                    test(tools): besu multi-party AIO container image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">Besu</span><span class="chip">dependencies</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                Works with a modified (forked) version of quorum-dev-quickstart
See https://github.com/ConsenSys/quorum-dev-quickstart/pull/72

On the fork we added an extra commit that removes the usage of
tput (which is a low impact change because all
it is being used for is to make text in the terminal bold for cosmetic
purposes).

This is published on the public registry as:
ghcr.io/hyperledger/cactus-besu-all-in-one-multi-party:2021-08-13--private-tx

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-13 23:42:37 +0000 UTC
    </div>
</div>

