---
layout: default
title: blockchain-carbon-accounting
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-carbon-accounting
---

# blockchain-carbon-accounting <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-carbon-accounting){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/380" class=".btn">#380</a>
            </td>
            <td>
                <b>
                    Bump openzeppelin/contracts to 4.4.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                    This commit address a low severity vulnerability in openzeppelin contracts 3.3.0/3.4.1. Should respond to [PR 374](https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/374) and [PR 375](https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/375) 
    Requires upgrading to solidity ^0.8.0 - now using compiler version 0.8.3:
        - Derived contract must override function "supportsInterface" (see new overrides in derived contracts)
        - Require changing getChainId() (DAOToken/Governor contracts) from pure to view
        - uint(-1) changec to type(uint).max
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-03 12:23:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/379" class=".btn">#379</a>
            </td>
            <td>
                <b>
                    New CarbonTracker contract and TokenTypeId (4) for NET network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                TokenTypeId=4 for carbon Tokens issued (voluntarily) by registered industry of the Net Emission Token (NET) Network. This supply side token and CarbonTracker contract will enable shared emission inventories across organizations and  embedded emission tracking.

Short summary of the CarbonTracker contract features:
- a NFT using ERC721Upgradeable template create carbon trackers
- Each NFT is used to track the unique emission profile of a product/facility based on NETs
- NETs in each NFTs can be linked to previous NFT connect emission profiles (embedded emissions)

Major additions/changes to the NetEmissionTokenNetwork contract:
- update _beforeTokenTransfer hook consumerOrDealer modifier for from/to addresses
- Applies modifier to super.safeTransfer/super._mint/super._burn
- If tokenTypeId == 4 require receiverApproved before sending tokens.

Signed-off-by: brioux <Bertrand.rioux@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-02 15:50:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/377" class=".btn">#377</a>
            </td>
            <td>
                <b>
                    chore(chaincode): Remove old chaincode and rearrange files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR closes #51. It makes the following changes:
* Deletes the `chaincode/go`, `chaincode/node` and `emissions_calc_test` directories
* Moves the `typescript`, `packaging` and `deploy` directories into a new `emissionscontract` directory
* Modifies Ansible script to use new file path
* Modifies CI workflow to use new file paths
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-28 18:43:28 +0000 UTC
    </div>
</div>

