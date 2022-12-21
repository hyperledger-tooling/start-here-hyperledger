---
layout: default
title: fabric-operations-console
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-operations-console
---

# fabric-operations-console <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-operations-console){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/347" class=".btn">#347</a>
            </td>
            <td>
                <b>
                    Fixing chaincode instantiation filtering
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nikhil Modem [Nikhil.Modem@ibm.com](mailto:Nikhil.Modem@ibm.com)

#### Type of change

- Bug fix

#### Description
- Filtering of peers to be used to submit an instantiation or upgrade to was broken due to the way policy msp id's were retrieved from a peer
- Fixed the lodash get to retrieve the identities properly
- Added some logic to the mapping to extract just the msp id string from the Uint8Array that is returned
- Also removed some logging that was left in from a previous PR


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-19 12:48:19 +0000 UTC
    </div>
</div>

