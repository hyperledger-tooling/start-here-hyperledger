---
layout: default
title: fabric-token-sdk
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-token-sdk
---

# fabric-token-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-token-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/386" class=".btn">#386</a>
            </td>
            <td>
                <b>
                    Transfer metadata rework
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">interoperability</span>
            </td>
            <td>
                - Transfer metadata key does not include txid and metadata counter anymore. It is up to the validator to make sure these keys are used properly
- check that a transfer contains only metadata that has been validated
- extend interop integration tests to orion

Signed-off-by: Angelo De Caro <adc@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-22 10:58:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/385" class=".btn">#385</a>
            </td>
            <td>
                <b>
                    FSC update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Angelo De Caro <adc@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-21 13:47:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/384" class=".btn">#384</a>
            </td>
            <td>
                <b>
                    Add timeout to Network Finality API #383
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                Signed-off-by: Angelo De Caro <adc@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-19 14:44:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/382" class=".btn">#382</a>
            </td>
            <td>
                <b>
                    review htlc terms
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                Signed-off-by: Hagar Meir <hagar.meir@ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-19 12:26:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/381" class=".btn">#381</a>
            </td>
            <td>
                <b>
                    double check the use of NewQuantityFromUInt64 #218
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">cleanup</span>
            </td>
            <td>
                This PR ensures that `token.Quantity` is used properly. Public parameters' precision field must be used when parsing quantities unless it is clear otherwise like in some tests.

Signed-off-by: Angelo De Caro <adc@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-19 08:53:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/380" class=".btn">#380</a>
            </td>
            <td>
                <b>
                    remove "zkat" magic string #107
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">cleanup</span>
            </td>
            <td>
                Signed-off-by: Angelo De Caro <adc@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-18 06:35:58 +0000 UTC
    </div>
</div>

