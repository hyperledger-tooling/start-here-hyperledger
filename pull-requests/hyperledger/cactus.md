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
                PR <a href="https://github.com/hyperledger/cactus/pull/1413" class=".btn">#1413</a>
            </td>
            <td>
                <b>
                    feat(connector-sawtooth): add the docker environment of Validator on connector-sawtooth-socketio
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                resolve #1326

Signed-off-by: Takuma TAKEUCHI <takeuchi.takuma@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-04 10:35:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1412" class=".btn">#1412</a>
            </td>
            <td>
                <b>
                    feat(connector-go-ethereum): add the docker environment of Validator on connector-go-ethereum-socketio
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                resolve #1326 

Signed-off-by: Takuma TAKEUCHI <takeuchi.takuma@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-04 10:00:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1411" class=".btn">#1411</a>
            </td>
            <td>
                <b>
                    refactor(cmd-server-socketio): refactor the verifier socket.io channel and verifierFactory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                resolve #1322 #1324

Signed-off-by: Takuma TAKEUCHI <takeuchi.takuma@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-04 09:22:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1410" class=".btn">#1410</a>
            </td>
            <td>
                <b>
                    fix(tools): add docker network on tools/docker/sawtooth ledger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                resolve #1409 

Signed-off-by: Takuma TAKEUCHI <takeuchi.takuma@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-04 08:54:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1408" class=".btn">#1408</a>
            </td>
            <td>
                <b>
                    fix(tools): fix the wallet config of fabcar chaincode on tools/docker/fabric ledger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                resolve #1311

Signed-off-by: Takuma TAKEUCHI <takeuchi.takuma@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-04 08:07:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1406" class=".btn">#1406</a>
            </td>
            <td>
                <b>
                    fix(webpack): prod build chokes on upgraded ssh2 binaries #1405
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                This removes all webpack minified builds entirely. This has the
benefits of faster and stabler builds.
What we lose is efficiency of deployments in resource constrained
environments where the bundle size would make a difference but
the idea here is to crawl, walk and then run with having these
minified bundles enabled being the running part of the equation.

Root cause
==========

If you update the yarn lock file to the latest & greatest it breaks the
webpack prod build at the moment with this beauty:

ERROR in ../../node_modules/ssh2/lib/protocol/crypto/build/Release/sshcrypto.node 1:0
Module parse failed: Unexpected character '' (1:0)
You may need an appropriate loader to handle this file type, currently no
loaders are configured to process this file. See https://webpack.js.org/concepts#loaders
(Source code omitted for this binary file)
 @ ../../node_modules/ssh2/lib/protocol/crypto.js 30:12-60
 @ ../../node_modules/ssh2/lib/client.js 34:29-60
 @ ../../node_modules/ssh2/lib/index.js 27:10-32
 @ ../../node_modules/docker-modem/lib/ssh.js 1:13-35
 @ ../../node_modules/docker-modem/lib/modem.js 6:8-24
 @ ../../node_modules/dockerode/lib/docker.js 2:10-33
 @ ./src/main/typescript/besu/besu-test-ledger.ts 8:36-56
 @ ./src/main/typescript/public-api.ts 20:25-59
 @ ./src/main/typescript/index.ts 13:13-36
To Reproduce

rm yarn.lock && yarn && yarn configure && yarn build

Fixes #1405

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-02 23:20:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1404" class=".btn">#1404</a>
            </td>
            <td>
                <b>
                    style: #1350 lint fixes for batch 1/26
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added lint fixes for batch 1/26 or #1350  issue
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-02 14:10:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1403" class=".btn">#1403</a>
            </td>
            <td>
                <b>
                    Fixed linter error in config-service.ts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixed unexpected type any by casting configSchema to Record
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-02 02:44:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1402" class=".btn">#1402</a>
            </td>
            <td>
                <b>
                    deprecate rotateEncryptionKeys method #1108
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                refactor(keychain): deprecate rotateEncryptionKeys method #1108

Found 6 locations of the method:
This pull request removes the method from 6/6 locations
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-01 23:09:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1398" class=".btn">#1398</a>
            </td>
            <td>
                <b>
                    Fix: lint warning fix batch 26/26 #1375
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Lint warning fix for batch 26/26 minus #251. #251 is in previous PR with #1374
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-01 21:33:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1397" class=".btn">#1397</a>
            </td>
            <td>
                <b>
                    Fix: lint warning fix for any to unknown #1374
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Lint fix for batch 25/26. + No.251 and No.240 (In the same file) 

Fixes #1374 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-01 21:05:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1396" class=".btn">#1396</a>
            </td>
            <td>
                <b>
                    docs: add cross-references to BUILD.md and CONTRIBUTING.md #1394
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Document updates for issue #1394
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-01 20:54:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1395" class=".btn">#1395</a>
            </td>
            <td>
                <b>
                    style: open source day batch 3 #1352
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Submitting fixes for Issue #1352, minus fix for ID 30. I am coordinating with another contributor before committing the fix for issue  ID 30.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-01 19:53:39 +0000 UTC
    </div>
</div>

