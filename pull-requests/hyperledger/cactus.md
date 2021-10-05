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
                PR <a href="https://github.com/hyperledger/cactus/pull/1404" class=".btn">#1404</a>
            </td>
            <td>
                <b>
                    Made changes and fixed linter warnings in issues listed under batch 1/26
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Made changes in all the files as listed under batch 11/26 assigned to me. Kindly review the PR and let me know if there are any amendments to be made
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1392" class=".btn">#1392</a>
            </td>
            <td>
                <b>
                    fix(plugin-ledger-connector-quorum): no keychain endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Endpoint invoke-contract without keychain was failing because,
on deploy, network information was saved inside the contractJson
object, which was keeping it on memory and for this reason it was
not failing calling the connector.

2. Now, when no keychain is used, instead of save the contracts
addresses in memory indexed by contractName, this parameter
should be sent in the request to avoid that there can only be a
single instance for each contract name. When keychain is used,
contract address is still saved indexed by contractName.

3. Openapi specs were changed to consider these changes,
including remove fields that are inside the contractJSON object
and definition of this object structure.

4. Includes openapi validation test for new endpoints.

Signed-off-by: Elena Izaguirre <e.izaguirre.equiza@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-30 14:08:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1391" class=".btn">#1391</a>
            </td>
            <td>
                <b>
                    docs: adding example for besu private transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                

Closes: 1213
Signed-off-by: Travis Payne <travis.payne@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-30 14:07:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1390" class=".btn">#1390</a>
            </td>
            <td>
                <b>
                    fix(cmd-api-server): enable version selection in plugins
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                cactus-cmd-api-server can now import plugins specifying
the npm package version as a plugin option

cmd-api-server: add missing dependency bluebird

closes #839 and #840

Signed-off-by: Elena Izaguirre <e.izaguirre.equiza@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-30 07:14:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1389" class=".btn">#1389</a>
            </td>
            <td>
                <b>
                    docs(examples): add npm version build arg to supply-chain app container
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span><span class="chip">dependencies</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                This will enable us to have an automated image publishing pipeline set up
later down the line as our automation capabilities increase.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 19:49:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1388" class=".btn">#1388</a>
            </td>
            <td>
                <b>
                    feat: allows for constructor args in quorum contract deploy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes: #962
Signed-off-by: Travis Payne <travis.payne@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 16:16:17 +0000 UTC
    </div>
</div>

