---
layout: default
title: fablo
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fablo
---

# fablo <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fablo){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/309" class=".btn">#309</a>
            </td>
            <td>
                <b>
                    Add version config for fabric-nodeenv, update Node version warnings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #274 Update Node.js runtime compatibility 

The compatibility information in fabric-chaincode-node 
(https://github.com/hyperledger/fabric-chaincode-node/blob/main/COMPATIBILITY.md)
lists an environment variable that can be used on a peer that 
hosts chaincode to alter the Node.js runtime used. 

This commit adds support for setting that environment variable 
to the fablo global config. It also updates fablo to support fabric version 2.4.2.

Based on some recent patches to fabric-chaincode-node:

https://github.com/hyperledger/fabric-chaincode-node/commit/d9cfc3d0b35fad4ed7e72b8ced370bef32f1d0b9
https://github.com/hyperledger/fabric-chaincode-node/blob/main/release_notes/v2.4.2.txt
"This release corrects the 2.4 nodeenv docker image to be Node 16, and ..."

A node version mapping was added similar to the existing javaenv
mapping to used the fixed fabric-nodeenv docker image if  
2.4 or 2.4.1 are supplied. 
(src/extend-config/extendGlobal.ts)
Probabably "2.4" should be removed from this mapping at such 
time that that image incorporates the fix released in 2.4.2, 
but for now it was added to potentially avoid cases 
where Node v12 is still being unexpected used on the peers. 

The Node.js warning message is also updated to recommend 16 
if the fabric version is 2.4 or higher, and 12 otherwise. 
Referenced existing github issue 274 for this fix. 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-09 18:07:49 +0000 UTC
    </div>
</div>

