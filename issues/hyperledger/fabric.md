---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/fabric/issues/2976" class=".btn">2976</a>
            </td>
            <td>
                <b>
                    Include the chaincode hash when installing an already existing chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span>
            </td>
            <td>
                When installing a new chaincode on the peer you do get the package id of the chaincode which is good... this allows customers to use that data to go through the approve/commit steps.

However the issue is when they are reinstalling an existing chaincode there is nothing in the response to indicate the package id(hash). Install in that case returns a message that the chaincode already exists. We should include the package id of the chaincode in the response when it is already installed on the peer.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 14:04:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/fabric/issues/2916" class=".btn">2916</a>
            </td>
            <td>
                <b>
                    Add Java example to chaincode as external service documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">docs</span><span class="chip">good first issue</span>
            </td>
            <td>
                Per stackoverflow post https://stackoverflow.com/questions/69115892/hyperledger-fabric-java-chaincode-timeout-expired-while-starting-chaincode  , it appears Java chaincode is missing from chaincode as an external service doc topic:
https://hyperledger-fabric.readthedocs.io/en/latest/cc_service.html#writing-chaincode-to-run-as-an-external-service

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 15:56:40 +0000 UTC
    </div>
</div>

