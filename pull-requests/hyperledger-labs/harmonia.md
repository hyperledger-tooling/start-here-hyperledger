---
layout: default
title: harmonia
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/harmonia
---

# harmonia <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/harmonia){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/harmonia/pull/59" class=".btn">#59</a>
            </td>
            <td>
                <b>
                    Added claim by proof path to committed EVM asset 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                After committing an EVM asset, the counterparty signs the draft transaction which locks the asset until the committed asset is claimed or reverted.
While both parties can revert the EVM asset, claiming without proofs of notarisation is only possible by the committer/owner of the EVM asset. The recipient must present proofs that the draft transaction was notarised in order to claim the EVM asset.
This PR adds the possibility to collect EVM signatures from Corda parties that verify and attest that a certain signature over the draft transaction hash belongs to a certain public key. These signatures can be used by the EVM asset recipient to claim the EVM asset independently from the EVM asset owner.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-24 16:08:08 +0000 UTC
    </div>
</div>

