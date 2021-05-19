---
layout: default
title: weaver-dlt-interoperability
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/weaver-dlt-interoperability
---

# weaver-dlt-interoperability <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/weaver-dlt-interoperability){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/55" class=".btn">#55</a>
            </td>
            <td>
                <b>
                    changes to receive serialized protos in base64 and validation on locker/recipient
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-19 10:40:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/54" class=".btn">#54</a>
            </td>
            <td>
                <b>
                    SimpleAsset Bug Fix and Fabric-cli updated to initialize Asset networks.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. A bug in simpleasset where it was never creating new wallets for users has been fixed.
2. Added command to add/register users to fabric-network who can be participate in asset exchange: `fabric-cli user add`.
3. Added command to initialise the bond/token networks: `fabric-cli configure asset add`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-18 10:01:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/53" class=".btn">#53</a>
            </td>
            <td>
                <b>
                    Minor Changes in SimpleAsset Chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Create function accepts date in string  format to be convenient.
2. Renamed FaceValue to Value in TokenAsset.
3. Updated to Go 1.15.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-17 10:35:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/49" class=".btn">#49</a>
            </td>
            <td>
                <b>
                    Fungible and non-fungible asset functions using contractId
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Implements the below non-fungible asset functions:
- IsAssetLockedUsingContractId
- UnLockAssetUsingContractId
- ClaimAssetUsingContractId

Implements the below fungible asset functions:
- LockFungibleAsset
- IsFungibleAssetLocked
- UnLockFungibleAsset
- ClaimFungibleAsset
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-12 20:22:19 +0000 UTC
    </div>
</div>

