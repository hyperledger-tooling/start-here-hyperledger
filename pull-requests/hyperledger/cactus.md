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
                PR <a href="https://github.com/hyperledger/cactus/pull/1453" class=".btn">#1453</a>
            </td>
            <td>
                <b>
                    chore(maintainer): update maintainer list
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                update maintainer list

This PR corresponds to Issue #1452 

Signed-off-by: Izuru Sato <sato.izuru@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-12 01:24:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1451" class=".btn">#1451</a>
            </td>
            <td>
                <b>
                    chore(release): publish v1.0.0-rc.1
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
        Created At 2021-10-11 18:45:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1449" class=".btn">#1449</a>
            </td>
            <td>
                <b>
                    fix(cmd-socker-server): delete unnecessary files on cmd-socker-server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                resolve #1450 

Signed-off-by: Takuma TAKEUCHI <takeuchi.takuma@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-11 12:18:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1448" class=".btn">#1448</a>
            </td>
            <td>
                <b>
                    docs(nonce-manager): nonce manager investigation report
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Change
 -----------------
1. Added investigation report detailing the research done for issue #1036

Signed-off-by: jagpreetsinghsaan <jagpreet.singh.sasan@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-11 07:42:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1447" class=".btn">#1447</a>
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
        Created At 2021-10-07 11:20:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1446" class=".btn">#1446</a>
            </td>
            <td>
                <b>
                    fix(api-server): fixes issue 1444 invoking the required onPluginInit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In api server the instantiatePlugin function is now calling the required
onPluginInit for each corresponding connector

Closes: #1444
Signed-off-by: Michael Courtin <michael.courtin@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 08:47:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1443" class=".btn">#1443</a>
            </td>
            <td>
                <b>
                    fix(core-api): modifications in openapi specs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Modifies definition of schemas GetKeychainEntryRequestV1 and
DeleteKeychainEntryRequest to add option additionalProperties=false
to them.

Modifies definition of schemas GetKeychainEntryResponseV1 and
DeleteKeychainEntryResponseV1 to remove option
additionalProperties=false.

Signed-off-by: Elena Izaguirre <e.izaguirre.equiza@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 06:47:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1442" class=".btn">#1442</a>
            </td>
            <td>
                <b>
                    feat: option to enable a graceful shutdown via cli
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes: #1223 
Signed-off-by: Travis Payne <travis.payne@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-06 09:48:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1441" class=".btn">#1441</a>
            </td>
            <td>
                <b>
                    fix: openapi validation for keychain-google-sm plugin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Includes tests for endpoints setKeychainEntry, getKeychainEntryV1,
hasKeychainEntryV1 and deleteKeychainEntryV1, each of them with
test cases:
  - Right request
  - Request including an invalid parameter
  - Request without a required parameter

Dependent on #1443

Relationed with #847

Signed-off-by: Elena Izaguirre <e.izaguirre.equiza@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-06 07:15:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1439" class=".btn">#1439</a>
            </td>
            <td>
                <b>
                    feat(connector-quorum): split web3 endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR splits the run transaction web3 endpoint into the 4 different web3 signing types. It also creates 4 new invoke contract methods.

resolve #1248 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-05 10:11:09 +0000 UTC
    </div>
</div>

