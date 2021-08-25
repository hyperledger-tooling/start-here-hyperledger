---
layout: default
title: minifabric
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/minifabric
---

# minifabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/minifabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/minifabric/pull/263" class=".btn">#263</a>
            </td>
            <td>
                <b>
                    revert #239, couchdb version  v.3 => hyperledger/fabric-couchdb:latest to support legacy fabric-version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #239 changed couchdb version from fabric-couchdb:latest to couchdb:3

the background of #239:
- fabric-couchdb became deprecated and recent fabric supports couchdb:3 officially.

the reason of revert #239:
 - to use couchdb:3, it needs FAB-17993 in peer which legacy fabric doesn't have.
 - recent fabric version still supports fabric-couchdb,  so simply revert it.

for supporting variety of versions (legacy to recent), version-image matrix will be needed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-25 01:30:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/minifabric/pull/262" class=".btn">#262</a>
            </td>
            <td>
                <b>
                    Fix: Anchorupdate - replaced deprecated configtxgen -outputAnchorPeer…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As discussed in #247 replaced deprecated `configtxgen -outputAnchorPeersUpdate` in `anchorupdate.j2` with `configtxlator`

Signed-off-by: Dilum Bandara <dilum.bandara@ieee.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-24 10:21:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/minifabric/pull/261" class=".btn">#261</a>
            </td>
            <td>
                <b>
                    fix java chaincode to work with current fabric versions.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                close #260
tested and worked with following fabric versions
- 1.4.4 (current minimum supported version by minifab)
- 2.0    ( first 2.0 series)
- 2.3.2 ( latest )

so, other version can work with this PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-22 04:13:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/minifabric/pull/259" class=".btn">#259</a>
            </td>
            <td>
                <b>
                    Change latest Fabric version from 2.2.0 to 2.3.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Changed the current Fabric release version number in the docs from 2.2.0 to 2.3.0
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-20 23:08:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/minifabric/pull/258" class=".btn">#258</a>
            </td>
            <td>
                <b>
                    Fixed issue described in issue 257
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Tong Li <litong01@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-20 12:28:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/minifabric/pull/256" class=".btn">#256</a>
            </td>
            <td>
                <b>
                    update docs/DeployOntoK8S.md for reordering instrucction
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                proxy environment variable is set     x after ingress install    o before ingress install

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-19 08:11:11 +0000 UTC
    </div>
</div>

