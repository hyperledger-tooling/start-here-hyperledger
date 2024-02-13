---
layout: default
title: indy-besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-besu
---

# indy-besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-besu/pull/22" class=".btn">#22</a>
            </td>
            <td>
                <b>
                    Added smart contract to store mapping between legacy and new DID/Schema/CredDef identifiers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * The contract stores mapping between legacy and new identifiers.
* The contract can be used for parties who are needed to provide a migration form Indy-Ledger
* On data migration, those parties can store mapping and query for resolving of DID/Schema/CredDef by legacy identifier  

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-08 09:01:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-besu/pull/21" class=".btn">#21</a>
            </td>
            <td>
                <b>
                    Schema  and Credential Definition validations in VDR
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added schema and Credential Definition validations to VDR (according to [the previous smart-contracts logic](https://github.com/DSRCorporation/indy-node/blob/096fb303448d644f75c33f6c7dec6a5b192e6774/indy-besu/smart_contracts/contracts/cl/SchemaValidator.sol))
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-07 08:19:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-besu/pull/20" class=".btn">#20</a>
            </td>
            <td>
                <b>
                    Unit tests for VDR
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added unit tests for VDR:
- client
- txn builders, parsers
- some contract methods
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-07 07:59:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-besu/pull/19" class=".btn">#19</a>
            </td>
            <td>
                <b>
                    Revert reason handling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added revert reason handling for VDR

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-06 13:47:50 +0000 UTC
    </div>
</div>

