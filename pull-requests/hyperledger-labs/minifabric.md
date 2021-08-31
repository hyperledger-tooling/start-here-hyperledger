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
                PR <a href="https://github.com/hyperledger-labs/minifabric/pull/265" class=".btn">#265</a>
            </td>
            <td>
                <b>
                    new alias for chaincode up operation 'ccup'
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                close #251

'minifab ccup' == 'minifab install,approve,commit,initialize,discover,channelquery'
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-25 07:55:28 +0000 UTC
    </div>
</div>

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

