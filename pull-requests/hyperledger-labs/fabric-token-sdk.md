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
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/123" class=".btn">#123</a>
            </td>
            <td>
                <b>
                    Resolve data races in ZKAT-DLOG transfers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit resolves data races in the ZKAT-DLOG transfers via refactoring the code to use local variables instead of field variables, hence making local variables reference-able only from the goroutine that created them and not shared across goroutines.

Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-19 11:37:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/122" class=".btn">#122</a>
            </td>
            <td>
                <b>
                    reduce deps to platform/fabric
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
        Created At 2021-10-15 13:49:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/121" class=".btn">#121</a>
            </td>
            <td>
                <b>
                    Added FPC support to Token Topology
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
        Created At 2021-10-15 11:56:51 +0000 UTC
    </div>
</div>

