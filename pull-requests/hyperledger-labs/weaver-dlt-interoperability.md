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
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/154" class=".btn">#154</a>
            </td>
            <td>
                <b>
                    Fabric Interoperation Chaincode Refactoring and Augmentation for Access Controls, and Logging Improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Separated Go mock testing functions into a separate `testutils` library (Go package).
- Added access control logic to Fabric Interop CC asset management module to allow invocation requests only from other application chaincodes; also associated HTLC units with a chaincode ID for isolation of locks within chaincode namespaces.
- Fixed logging behavior in relay and in the Corda Interop App to print complex payloads as Base64 strings rather than as byte arrays.
- Added support in Fabric CLI to run chaincodes other than `simplestate` for data sharing.
- Updated testnets for compatibility with the above changes and ran end-to-end tests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-06 22:11:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/152" class=".btn">#152</a>
            </td>
            <td>
                <b>
                    Fabric CLI changes for asset-exchange using Go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR includes:

- user registration/enrollment using go-sdk
- 'fabric-cli user add ' command in go-cli
- Minor typos in docs and in fabric-cli for node
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-01 19:50:54 +0000 UTC
    </div>
</div>

