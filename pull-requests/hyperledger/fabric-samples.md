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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/466" class=".btn">#466</a>
            </td>
            <td>
                <b>
                    Fix typo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Tatsuya Sato <tatsuya.sato.so@hitachi.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-30 03:50:34 +0000 UTC
    </div>
</div>

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

### Example commands

```bash
#!/usr/bin/env bash

set -x #echo on

cd fabric-samples/test-network

echo "Clean up any existing network"
./network.sh down

echo "Start test network"
./network.sh up createChannel -ca

echo "Deploy ERC1155 chaincode. The path must point to the root folder of the chaincode"
./network.sh deployCC -ccn erc1155 -ccp ../token-erc-1155/chaincode-go/ -ccl go

echo "Set Fabric config path"
export FABRIC_CFG_PATH=${PWD}/../config/

echo "Add Fabric CLI utilities to path"
export PATH=${PWD}/../bin:$PATH


echo "As Org1 Certificate Authority"
export FABRIC_CA_CLIENT_HOME=${PWD}/organizations/peerOrganizations/org1.example.com/

echo "Create and register Person1 to Org1"
echo "Register a new indentity"
fabric-ca-client register --caname ca-org1 --id.name person1 --id.secret person1pw --id.type client --tls.certfiles "${PWD}/organizations/fabric-ca/org1/tls-cert.pem"

echo "Generate the identity certificates and MSP folder"
fabric-ca-client enroll -u https://person1:person1pw@localhost:7054 --caname ca-org1 -M "${PWD}/organizations/peerOrganizations/org1.example.com/users/person1@org1.example.com/msp" --tls.certfiles "${PWD}/organizations/fabric-ca/org1/tls-cert.pem"

echo "Copy the Node OU configuration file into the identity MSP folder"
cp "${PWD}/organizations/peerOrganizations/org1.example.com/msp/config.yaml" "${PWD}/organizations/peerOrganizations/org1.example.com/users/person1@org1.example.com/msp/config.yaml"

echo "As Org2 Certificate Authority"
export FABRIC_CA_CLIENT_HOME=${PWD}/organizations/peerOrganizations/org2.example.com/

echo "Create and register Person2 to Org2"
fabric-ca-client register --caname ca-org2 --id.name person2 --id.secret person2pw --id.type client --tls.certfiles "${PWD}/organizations/fabric-ca/org2/tls-cert.pem"
fabric-ca-client enroll -u https://person2:person2pw@localhost:8054 --caname ca-org2 -M "${PWD}/organizations/peerOrganizations/org2.example.com/users/person2@org2.example.com/msp" --tls.certfiles "${PWD}/organizations/fabric-ca/org2/tls-cert.pem"
cp "${PWD}/organizations/peerOrganizations/org2.example.com/msp/config.yaml" "${PWD}/organizations/peerOrganizations/org2.example.com/users/person2@org2.example.com/msp/config.yaml"

echo "Create and register Person3 to Org2"
fabric-ca-client register --caname ca-org2 --id.name person3 --id.secret person3pw --id.type client --tls.certfiles "${PWD}/organizations/fabric-ca/org2/tls-cert.pem"
fabric-ca-client enroll -u https://person3:person3pw@localhost:8054 --caname ca-org2 -M "${PWD}/organizations/peerOrganizations/org2.example.com/users/person3@org2.example.com/msp" --tls.certfiles "${PWD}/organizations/fabric-ca/org2/tls-cert.pem"
cp "${PWD}/organizations/peerOrganizations/org2.example.com/msp/config.yaml" "${PWD}/organizations/peerOrganizations/org2.example.com/users/person3@org2.example.com/msp/config.yaml"

echo "Create and register Person4 to Org2"
fabric-ca-client register --caname ca-org2 --id.name person4 --id.secret person4pw --id.type client --tls.certfiles "${PWD}/organizations/fabric-ca/org2/tls-cert.pem"
fabric-ca-client enroll -u https://person4:person4pw@localhost:8054 --caname ca-org2 -M "${PWD}/organizations/peerOrganizations/org2.example.com/users/person4@org2.example.com/msp" --tls.certfiles "${PWD}/organizations/fabric-ca/org2/tls-cert.pem"
cp "${PWD}/organizations/peerOrganizations/org2.example.com/msp/config.yaml" "${PWD}/organizations/peerOrganizations/org2.example.com/users/person4@org2.example.com/msp/config.yaml"

echo "Create and register Person5 to Org2"
fabric-ca-client register --caname ca-org2 --id.name person5 --id.secret person5pw --id.type client --tls.certfiles "${PWD}/organizations/fabric-ca/org2/tls-cert.pem"
fabric-ca-client enroll -u https://person5:person5pw@localhost:8054 --caname ca-org2 -M "${PWD}/organizations/peerOrganizations/org2.example.com/users/person5@org2.example.com/msp" --tls.certfiles "${PWD}/organizations/fabric-ca/org2/tls-cert.pem"
cp "${PWD}/organizations/peerOrganizations/org2.example.com/msp/config.yaml" "${PWD}/organizations/peerOrganizations/org2.example.com/users/person5@org2.example.com/msp/config.yaml"


echo "As Person1 from Org1"
export CORE_PEER_TLS_ENABLED=true
export CORE_PEER_LOCALMSPID="Org1MSP"
export CORE_PEER_MSPCONFIGPATH=${PWD}/organizations/peerOrganizations/org1.example.com/users/person1@org1.example.com/msp
export CORE_PEER_TLS_ROOTCERT_FILE=${PWD}/organizations/peerOrganizations/org1.example.com/peers/peer0.org1.example.com/tls/ca.crt
export CORE_PEER_ADDRESS=localhost:7051
export TARGET_TLS_OPTIONS=(-o localhost:7050 --ordererTLSHostnameOverride orderer.example.com --tls --cafile "${PWD}/organizations/ordererOrganizations/example.com/orderers/orderer.example.com/msp/tlscacerts/tlsca.example.com-cert.pem" --peerAddresses localhost:7051 --tlsRootCertFiles "${PWD}/organizations/peerOrganizations/org1.example.com/peers/peer0.org1.example.com/tls/ca.crt" --peerAddresses localhost:9051 --tlsRootCertFiles "${PWD}/organizations/peerOrganizations/org2.example.com/peers/peer0.org2.example.com/tls/ca.crt")

echo "Client Account ID for Person1"
peer chaincode query -C mychannel -n erc1155 -c '{"function":"ClientAccountID","Args":[]}'

# Client Account ID is a base64-encoded concatenation of the issuer and subject from the client identity's enrolment certificate.
# You can decode it with the following command:
# echo "eDUwOTo6Q049cGVyc29uMSxPVT1jbGllbnQsTz1IeXBlcmxlZGdlcixTVD1Ob3J0aCBDYXJvbGluYSxDPVVTOjpDTj1jYS5vcmcxLmV4YW1wbGUuY29tLE89b3JnMS5leGFtcGxlLmNvbSxMPUR1cmhhbSxTVD1Ob3J0aCBDYXJvbGluYSxDPVVT" | base64 --decode
echo "Client Account IDs"
export P1="eDUwOTo6Q049cGVyc29uMSxPVT1jbGllbnQsTz1IeXBlcmxlZGdlcixTVD1Ob3J0aCBDYXJvbGluYSxDPVVTOjpDTj1jYS5vcmcxLmV4YW1wbGUuY29tLE89b3JnMS5leGFtcGxlLmNvbSxMPUR1cmhhbSxTVD1Ob3J0aCBDYXJvbGluYSxDPVVT"
export P2="eDUwOTo6Q049cGVyc29uMixPVT1jbGllbnQsTz1IeXBlcmxlZGdlcixTVD1Ob3J0aCBDYXJvbGluYSxDPVVTOjpDTj1jYS5vcmcyLmV4YW1wbGUuY29tLE89b3JnMi5leGFtcGxlLmNvbSxMPUh1cnNsZXksU1Q9SGFtcHNoaXJlLEM9VUs="
export P3="eDUwOTo6Q049cGVyc29uMyxPVT1jbGllbnQsTz1IeXBlcmxlZGdlcixTVD1Ob3J0aCBDYXJvbGluYSxDPVVTOjpDTj1jYS5vcmcyLmV4YW1wbGUuY29tLE89b3JnMi5leGFtcGxlLmNvbSxMPUh1cnNsZXksU1Q9SGFtcHNoaXJlLEM9VUs="
export P4="eDUwOTo6Q049cGVyc29uNCxPVT1jbGllbnQsTz1IeXBlcmxlZGdlcixTVD1Ob3J0aCBDYXJvbGluYSxDPVVTOjpDTj1jYS5vcmcyLmV4YW1wbGUuY29tLE89b3JnMi5leGFtcGxlLmNvbSxMPUh1cnNsZXksU1Q9SGFtcHNoaXJlLEM9VUs="
export P5="eDUwOTo6Q049cGVyc29uNSxPVT1jbGllbnQsTz1IeXBlcmxlZGdlcixTVD1Ob3J0aCBDYXJvbGluYSxDPVVTOjpDTj1jYS5vcmcyLmV4YW1wbGUuY29tLE89b3JnMi5leGFtcGxlLmNvbSxMPUh1cnNsZXksU1Q9SGFtcHNoaXJlLEM9VUs="

echo "Person P1 from the organization 1 calls the MintBatch function in order to create 100 token1s, 200 token2s, 300 token3s, 150 token4s, 100 token5s, 100 token6s."
peer chaincode invoke "${TARGET_TLS_OPTIONS[@]}" -C mychannel -n erc1155 -c "{\"function\":\"MintBatch\",\"Args\":[\"$P1\",\"[1,2,3,4,5,6]\",\"[100,200,300,150,100,100]\"]}" --waitForEvent

echo "Query the tokens of Person1"
peer chaincode query -C mychannel -n erc1155 -c "{\"function\":\"BalanceOfBatch\",\"Args\":[\"[\\\"$P1\\\",\\\"$P1\\\",\\\"$P1\\\",\\\"$P1\\\",\\\"$P1\\\",\\\"$P1\\\"]\",\"[1,2,3,4,5,6]\"]}"

echo "Person P1 calls TransferFrom in order to send Person P2 six token3s."
peer chaincode invoke "${TARGET_TLS_OPTIONS[@]}" -C mychannel -n erc1155 -c "{\"function\":\"TransferFrom\",\"Args\":[\"$P1\",\"$P2\",\"3\",\"6\"]}" --waitForEvent

echo "New Balance of Person1 for token3"
peer chaincode query -C mychannel -n erc1155 -c "{\"function\":\"BalanceOf\",\"Args\":[\"$P1\",\"3\"]}"

echo "As Person2 from Organization 2"
export FABRIC_CFG_PATH=$PWD/../config/
export CORE_PEER_TLS_ENABLED=true
export CORE_PEER_LOCALMSPID="Org2MSP"
export CORE_PEER_MSPCONFIGPATH=${PWD}/organizations/peerOrganizations/org2.example.com/users/person2@org2.example.com/msp
export CORE_PEER_TLS_ROOTCERT_FILE=${PWD}/organizations/peerOrganizations/org2.example.com/peers/peer0.org2.example.com/tls/ca.crt
export CORE_PEER_ADDRESS=localhost:9051

echo "New Balance of Person2 for token3"
peer chaincode query -C mychannel -n erc1155 -c "{\"function\":\"BalanceOf\",\"Args\":[\"$P2\",\"3\"]}"

echo "As Person1 from Org1"
export CORE_PEER_TLS_ENABLED=true
export CORE_PEER_LOCALMSPID="Org1MSP"
export CORE_PEER_MSPCONFIGPATH=${PWD}/organizations/peerOrganizations/org1.example.com/users/person1@org1.example.com/msp
export CORE_PEER_TLS_ROOTCERT_FILE=${PWD}/organizations/peerOrganizations/org1.example.com/peers/peer0.org1.example.com/tls/ca.crt
export CORE_PEER_ADDRESS=localhost:7051
export TARGET_TLS_OPTIONS=(-o localhost:7050 --ordererTLSHostnameOverride orderer.example.com --tls --cafile "${PWD}/organizations/ordererOrganizations/example.com/orderers/orderer.example.com/msp/tlscacerts/tlsca.example.com-cert.pem" --peerAddresses localhost:7051 --tlsRootCertFiles "${PWD}/organizations/peerOrganizations/org1.example.com/peers/peer0.org1.example.com/tls/ca.crt" --peerAddresses localhost:9051 --tlsRootCertFiles "${PWD}/organizations/peerOrganizations/org2.example.com/peers/peer0.org2.example.com/tls/ca.crt")


echo "Person P1 calls BatchTransferFrom in order to send Person P2 six token3s, three token4s, and one token2s."
peer chaincode invoke "${TARGET_TLS_OPTIONS[@]}" -C mychannel -n erc1155 -c "{\"function\":\"BatchTransferFrom\",\"Args\":[\"$P1\",\"$P2\",\"[3,4,2]\",\"[6,3,1]\"]}" --waitForEvent

echo "Person P1 calls BatchTransferFromMultiReceipent in order to send:"
echo "- six token5s to person P3,"
echo "- six token3s  to person P4,"
echo "- three token4s to person P2," 
echo "- two token2s to person P5 and"
echo "- three token6s to person P2." 
peer chaincode invoke "${TARGET_TLS_OPTIONS[@]}" -C mychannel -n erc1155 -c "{\"function\":\"BatchTransferFromMultiRecipient\",\"Args\":[\"$P1\",\"[\\\"$P3\\\",\\\"$P4\\\",\\\"$P2\\\",\\\"$P5\\\",\\\"$P2\\\"]\",\"[5,3,4,2,6]\",\"[6,6,3,2,3]\"]}" --waitForEvent

echo "Shut down network"
./network.sh down
```

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

