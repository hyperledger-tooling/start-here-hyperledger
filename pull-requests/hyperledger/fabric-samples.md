---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/923" class=".btn">#923</a>
            </td>
            <td>
                <b>
                    WIP: test network nano bash updated with smartbft consensus
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It requires the configtxgen & orderer smartbft changes from PR https://github.com/hyperledger/fabric/pull/3781

Signed-off-by: Parameswaran Selvam <parselva@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-31 19:19:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/922" class=".btn">#922</a>
            </td>
            <td>
                <b>
                    AssetTransfer Private - Incorrect Endorsement Policy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                For the asset transfer example (https://hyperledger-fabric.readthedocs.io/en/release-2.5/private_data_tutorial.html#pd-use-case)  there are three private data collections, one per org and one shared between the orgs.

The shared collection didn't have an endorsement policy so inherited the chaincodes; this was specifically set away from the default to be OR(Org1MSP,Org2MSP).   The documentation says this is to ensure that either organization can create an asset. Whilst this is strictly correct, it is misleading - it doesn't need to be a chaincode wide policy, but specifically to the shared collection. 

Therefore it is better to leave the chaincode policy at its default and move the specific policy down to the collection. 
With the context of this example as coded, this is exactly functionally the same - but gives a more accurate impression. 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-31 09:41:00 +0000 UTC
    </div>
</div>

