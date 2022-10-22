---
layout: default
title: fabric-smart-client
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-smart-client
---

# fabric-smart-client <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-smart-client){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/426" class=".btn">#426</a>
            </td>
            <td>
                <b>
                    NWO to only use Fabric Binaries
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                follow-on from #423 as merge mess meant I needed to open a new PR
Signed-off-by: Dave Kelsey <d_kelsey@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-21 15:29:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/422" class=".btn">#422</a>
            </td>
            <td>
                <b>
                    Minor updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                - correct a trace point that was incorrect
- update to include 0.0.0.0 in the x509 SAN fields, for the Ubuntu WSL2 distribution the standard x509 certificates fail validation.

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-19 08:12:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/421" class=".btn">#421</a>
            </td>
            <td>
                <b>
                    enhancement pack
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">enhancement</span><span class="chip">Fabric</span><span class="chip">orion</span>
            </td>
            <td>
                - NWO fabric and orion: ability to remove the vault of FSC nodes
- Introduce the `PostStart` interface. PostStart allows a platform to start services after all the other platforms have been started. This feature has been introduce to allow platforms to add hookups in the fabric and orion commit pipelines before the pipelines start. Fabric and Orion commit pipelines are now activated in post-start.
- fabric chaincode: when querying a chiancode, discovery performs now a `peer query` and not an `endorser query`.
- Fabric and Orion Committer: if the status of a transaction is requested, if this transaction does not exist in the vault but its envelope exists, then the envelope is loaded into the vaul.

The changes to the commit pipelines and `PostStart` allow a node to rebuild its vault if the KVS has not been compromised.

Used by: https://github.com/hyperledger-labs/fabric-token-sdk/pull/406
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-18 14:31:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/420" class=".btn">#420</a>
            </td>
            <td>
                <b>
                    sample config with doc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a sample core.yaml file for fsc and fabric-driver, for discussion to add and improve the associated documentation
Signed-off-by: Dave Kelsey <d_kelsey@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-18 08:54:10 +0000 UTC
    </div>
</div>

