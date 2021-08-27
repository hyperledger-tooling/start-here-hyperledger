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
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/148" class=".btn">#148</a>
            </td>
            <td>
                <b>
                    Fix broken link in README.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-27 09:29:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/147" class=".btn">#147</a>
            </td>
            <td>
                <b>
                    Besu interop contract for ERC20 and HTLC app
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Core network interop contract for ERC20 
2. An application for HTLC across two Besu networks managing ERC20 tokens, possibly of different types

Signed-off-by: Dhinakaran Vinayagamurthy <dhinakaran2705@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-26 11:00:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/146" class=".btn">#146</a>
            </td>
            <td>
                <b>
                    Fixing import path bug in Fabric Interop CC libs/testutils
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: VRamakrishna <vramakr2@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-24 20:40:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/145" class=".btn">#145</a>
            </td>
            <td>
                <b>
                    Augmenting Fabric Interop Chaincode Libraries
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added `utils` and `test` folders to Fabric Interoperation chaincode `libs`. The former contains utility functions to help determine whether a chaincode invocation is coming from a relay or a different chaincode; this will be imported both by the Interoperation Chaincode and sample chaincodes (in `samples`). The latter contains the mock stub code used for unit testing in several different Go packages within Weaver.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-24 14:26:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/144" class=".btn">#144</a>
            </td>
            <td>
                <b>
                    added fabric-cli with commands to exercise asset-exchange in Go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Added below commands:
    - fabric-cli asset exchange-all
    - fabric-cli asset exchange-step
    - fabric-cli chaincode invoke
    - fabric-cli chaincode query
    - fabric-cli configure asset
    - fabric-cli config get
    - fabric-cli config set
    - fabric-cli config set-file
    - fabric-cli env get
    - fabric-cli env set
    - fabric-cli env set-file
2. Also move the go-cli code from `sdks/fabric/go-cli` to `samples/fabric/go-cli`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-24 08:50:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/143" class=".btn">#143</a>
            </td>
            <td>
                <b>
                    Added Corda SDK, and pages for docker based deployment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Added Corda SDK for interoperation.
2. Changed Corda client to use SDK.
3. SDK now uses protos as input for the policies (removing linearId from input files).
4. Updated the policies in `clients/src/main/resources` folder.
5. Added docker based weaver deployment page to docs.
6. Updated relay, drivers envs and instructions to work with docker.
7. Added Enabling weaver in corda application page to docs.
Using env variables to configure corda driver's rpc username and password.

Fixes:
1. Updated `corda-interop-app` and `fabric-interop-cc` unit tests (expired certs update).


Before running Tests, please:
1. Replace `hyperledger-labs` with `sanvenDev` in `url` field of `github.properties`.
2. Run:  `docker rmi ghcr.io/hyperledger-labs/weaver-corda-driver:1.2.3`.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-23 06:16:58 +0000 UTC
    </div>
</div>

