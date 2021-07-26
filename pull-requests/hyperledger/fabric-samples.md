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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/465" class=".btn">#465</a>
            </td>
            <td>
                <b>
                    changed all 'complileOnly' to 'implementation' on all fabric-samples for the fabric dependency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                spotted that on the dependencies of all chaincode-java we were doing 'compileOnly 'org.hyperledger.fabric-chaincode-java:fabric-chaincode-shim:2.+'' instead of 'implementation'
This was preventing all java smart contracts to run on VSCode: microfab (used on vscode) does not import fabric while in cli (which uses test-network) it is embeded
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-26 15:47:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/464" class=".btn">#464</a>
            </td>
            <td>
                <b>
                    JSON determinism example for asset-transfer-basic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added features for JSON determinism across languages on the asset-transfer-basic sample
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-26 15:20:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/463" class=".btn">#463</a>
            </td>
            <td>
                <b>
                    Add ERC1155 chaincode in Go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This pull request adds ERC1155 chaincode written in Go.

ERC20 is the standard for fungible tokens. ERC721 is the standard for non-fungible tokens. ERC1155 is the standard for multiple tokens (both fungible and non-fungible). [More information about ERC1155 standard can be found here.](https://eips.ethereum.org/EIPS/eip-1155)

### Architecture
Our implementation aims for high throughput by minimizing key collision. We utilized batching and distributed the balance over multiple keys. Since ERC1155 is account-based, the interface of the chaincode is account-based. However, since the balances are distributed over multiple keys, the chaincode has a model similar to a UTXO-based chaincode internally.

In this chaincode, one organization has a minter/burner role just like in the [ERC20 example in this repository](https://github.com/hyperledger/fabric-samples/tree/main/token-erc-20).

We used unsigned integers for transfer amounts contrary to signed integers used [in the ERC20 example](https://github.com/hyperledger/fabric-samples/tree/main/token-erc-20). Is there any reason to use signed integers in Fabric chaincodes? If not, it's okay. If there is a reason, please let me know and I will change the type of integers.

### Functions Implemented
The following required functions of ERC1155 are implemented:
- safeTransferFrom
- safeBatchTransferFrom
- balanceOf
- balanceOfBatch
- setApprovalForAll
- isApprovedForAll

Note: We omitted "safe" prefix from "TransferFrom" in the implementation because it is related to some issue about backwards compatibility with older smart contracts.
Note: TransferFrom is used to send a single token type between two users. BatchTransferFrom is used to send multiple tokens between two users. So, BatchTransferFrom is a more general form of TransferFrom. Ethereum defined two functions instead of one because this reduces gas costs. Since there is no gas cost in Fabric, implementing these two functions is unnecessary. Nevertheless, we implemented both of them to to conform the ERC1155 standard.

### Additional Functions Implemented
We also implemented the following additional functions. I also explained our reasoning behind adding these functions:
- Optional Metadata URI extension: 
Defined in ERC1155 but not required. Allows one to set a URI for tokens and get the URI.
  - SetURI
  - URI
- Mint/Burn extension: 
Although Mint / Burn are not required, they are necessary to change the supply of tokens, create new fungible or non-fungible tokens. In a real implementation, they will be implemented unless the supply of the tokens is fixed beforehand. MintBatch / BurnBatch is only implemented to complement the TransferFrom/BatchTransferFrom. Actually, using only MintBatch and BurnBatch would be enough.
  - Mint
  - MintBatch
  - Burn
  - BurnBatch
- Extra/utility functions
  - BatchTransferFromMultiRecipient: We defined this function. It is only required if a person wants to send tokens to multiple persons in a blockchain block. If a person doesn't use this function and create two transactions in a single block, there will be key conflicts because the chaincode will try to decrement the balance of the sender twice in a block and this causes a key conflict in Fabric [just like explained in here](https://github.com/hyperledger/fabric-samples/tree/main/high-throughput). This problem does not exist in Ethereum because, in Ethereum, the transactions are ordered before they are executed.
  - BroadcastTokenExistence: Explained in ERC1155 but it is not required. It is only used if a token minter wants to announce the existence of a token without minting it.
  - ClientAccountID: This function is special for Fabric because we do not have wallet addresses in Fabric and users need to know their account ID to transfer tokens.
  - ClientAccountBalance: A shorthand for BalanceOf function.

Signed-off-by: Baran Kılıç <baran.kilic@boun.edu.tr>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-26 14:57:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/462" class=".btn">#462</a>
            </td>
            <td>
                <b>
                    Genesis Block error, fixed.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Genesis Block error due  to  missing profile in configtx.yaml file.
When you run the present program, it creates a genesis block which doesn't  look right, plus I couldn't find where the genesis block was being created in the present network.sh file in test-network folder. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-25 12:52:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/461" class=".btn">#461</a>
            </td>
            <td>
                <b>
                    Update asset-transfer-basic go chaincode dependencies (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update asset-transfer-basic go chaincode dependencies to latest
commits from release-2.2 dependency branches.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-22 21:44:17 +0000 UTC
    </div>
</div>

