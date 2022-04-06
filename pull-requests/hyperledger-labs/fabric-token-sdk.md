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
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/214" class=".btn">#214</a>
            </td>
            <td>
                <b>
                    fix topology sample
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
        Created At 2022-04-06 05:51:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/211" class=".btn">#211</a>
            </td>
            <td>
                <b>
                    nwo token enhancements 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - ability to set custom crypto material generators
- ability to set token chaincode params replace suffix
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-01 07:12:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/210" class=".btn">#210</a>
            </td>
            <td>
                <b>
                    cloning instructions
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
        Created At 2022-03-31 11:18:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/209" class=".btn">#209</a>
            </td>
            <td>
                <b>
                    Refactoring to make services backend agnostic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Hagar Meir <hagar.meir@ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-31 08:08:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/208" class=".btn">#208</a>
            </td>
            <td>
                <b>
                    Add token request extractor to TCC
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Refactor TCC that the tokenRequest extract logic can be injected. This
allows to use alternativ implmentations of the extracting logic other
than the default transient-based logic. A use case for this is, the
FPC-TCC. Currently, FPC does not support transient data, so the
tokenRequest must be provided via function args.

Signed-off-by: Marcus Brandenburger <bur@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 08:45:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/207" class=".btn">#207</a>
            </td>
            <td>
                <b>
                    network.fabric: support FPC
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If the token chaincode is a FPC, then we must pass the token request as an input not via transient.
This, at least, until FPC supports transient: https://github.com/hyperledger/fabric-private-chaincode/issues/666

Signed-off-by: Angelo De Caro <adc@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 07:26:53 +0000 UTC
    </div>
</div>

