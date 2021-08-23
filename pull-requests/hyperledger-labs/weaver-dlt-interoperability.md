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
7. [PENDING] Add Enabling weaver in corda application page to docs.

Fixes:
1. Updated `corda-interop-app` and `fabric-interop-cc` unit tests (expired certs update).

To Test:
Replace `hyperledger-labs` with `sanvenDev` in `url` field of `github.properties`.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-23 06:16:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/141" class=".btn">#141</a>
            </td>
            <td>
                <b>
                    Update rfc for identity management
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
        Created At 2021-08-18 06:33:40 +0000 UTC
    </div>
</div>

