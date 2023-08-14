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
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/403" class=".btn">#403</a>
            </td>
            <td>
                <b>
                    Initial step to implementing support for invoke command 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes a few issues caused by npm and implements support for invoke command for the simplest use case in issue #390:
1. Fixes errors caused by npm when running tests:
    - Removing unsupported test library for fabric that depends on packages that fail to compile
    - Bumps nodejs version from 12 to 16 at samples/chaincodes/chaincode-kv-node/.nvmrc
    - Removing non-crucial tests from the sample chaincode
       Possible fix for: 
     #348 
     #328

2. Created a new script `chaincode-scripts.sh ` to handle `docker exec` 
3. Created the invoke command for its simplest use case
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-13 20:59:48 +0000 UTC
    </div>
</div>

