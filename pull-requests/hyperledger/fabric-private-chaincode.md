---
layout: default
title: fabric-private-chaincode
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-private-chaincode
---

# fabric-private-chaincode <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-private-chaincode){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/721" class=".btn">#721</a>
            </td>
            <td>
                <b>
                    Upgrade yq from v3.x to v4.x
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Some example scripts still use an older version of yq. To run the example scripts properly newer version of yq is added.

<!--  Thanks for sending a pull request!  Here are some tips for you:

1. If this is your first time, please read our code of conduct and contributor guidelines: 
     https://github.com/hyperledger/fabric-private-chaincode/blob/main/CONTRIBUTING.md
     https://github.com/hyperledger/fabric-private-chaincode/blob/main/CODE_OF_CONDUCT.md
   In particular pay attention to the git workflows
      https://docs.google.com/document/d/1sR7YV3pSYN3NEFiW-2fUqtpsJeJrpC0EWUVtEm0Blcg/edit#heading=h.kwcug3pkefak
2. Fill out below sections.
3. Label the PR with the label of any component this PR touches.
4. ALso don't forget to sign your comments before submitting. 
   Github will complain if there is no DCO but it's easier if we don't have to hunt you down to fix that :-)

-->

**What this PR does / why we need it**: Upgrades the yq V3.x to yq v4.x

**Which issue(s) this PR fixes**:
- upgrades the yq from v3.x to v4.x 
- updates the yq codes in the list of files below :
 - `./samples/deployment/test-network/setup.sh`
 - `./samples/deployment/fabric-smart-client/the-simple-testing-network/env.sh`
 - `./samples/deployment/test-network/update-connection.sh`
 - `./samples/deployment/test-network/fabric-samples/test-network-nano-bash/README.md`
 -  `./README.md`
 - `./utils/docker/dev_peer_cc-builder/Dockerfile`
 - `./utils/docker/base-dev/Dockerfile`

Fixes #719 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-04 10:44:47 +0000 UTC
    </div>
</div>

