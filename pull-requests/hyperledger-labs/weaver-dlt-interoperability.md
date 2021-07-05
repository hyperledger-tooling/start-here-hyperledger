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
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/105" class=".btn">#105</a>
            </td>
            <td>
                <b>
                    Data Transfer Protocol Augmentations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Augmented the `WriteExternalState` API spec in the Fabric Interop CC to verify an array of views rather than just a single view.
Accordingly, augmented the `interopFlow` function in the Fabric Interop Node SDK.
Tweaked access control logic in the Fabric Interop CC to check MSP IDs instead of certificates for organizations (CAs).
Updated Fabric CLI to use the updated Fabric Interop Node SDK API.
Tested Fabric-Fabric and Fabric-Corda data transfer flows using the testnet.
Updated documentation.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-05 17:37:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/104" class=".btn">#104</a>
            </td>
            <td>
                <b>
                    Besu test network: initial commit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added scripts for spinning up a new Besu test network. Also, added a Readme on this.

Close #91 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-02 17:55:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/103" class=".btn">#103</a>
            </td>
            <td>
                <b>
                    Added Instructions for Relay configuration, updated driver's readme.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. `relay-config.md` added in `core/relay`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-02 12:53:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/95" class=".btn">#95</a>
            </td>
            <td>
                <b>
                    Return Signatures along with payload from corda-interop-app and modified corda-client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Now `GetExternalStateByLinearId` returns a JSON String, with proof consisting of list of signatures along with payload.
2. Modified client app, to read the new return object from `GetExternalStateByLinearId`.
3. Improved corda client app, to use env variables instead of hard coded values.

(1) was a requirement from Marcopolo demo.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-29 10:03:00 +0000 UTC
    </div>
</div>

