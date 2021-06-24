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
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/30" class=".btn">#30</a>
            </td>
            <td>
                <b>
                    clear version for the stack figure? #28
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
        Created At 2021-06-24 10:14:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/29" class=".btn">#29</a>
            </td>
            <td>
                <b>
                    Decouple unmarshaling from receiver and export bulk unmarshaling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                To support enhanced versions of fabtoken where we have issues / transfers co-existing with
other operations, one might want to implement a driver that classifies whether a token request
is a vanilla token request or carries enhanced operations.

In case it is a vanilla token request, the enhanced driver may route the token request to
the existing vanilla fabtoken driver, else to handle the advanced operations.

For that to work, I am exporting the unmarshaling functions of the fabtoken driver in order
to facilitate cross driver invocation.

Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-24 09:50:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/26" class=".btn">#26</a>
            </td>
            <td>
                <b>
                    additional documentation
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
        Created At 2021-06-21 13:15:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/23" class=".btn">#23</a>
            </td>
            <td>
                <b>
                    additional documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                + some refactoring

Signed-off-by: Angelo De Caro <adc@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-20 07:20:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/21" class=".btn">#21</a>
            </td>
            <td>
                <b>
                    additional documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - more documentation
- more function comments
- ttxcc wallet's support functions return nil instead of panicing

Signed-off-by: Angelo De Caro <adc@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-18 17:43:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/20" class=".btn">#20</a>
            </td>
            <td>
                <b>
                    removing deps to `view/driver` #18
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
        Created At 2021-06-18 13:16:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/19" class=".btn">#19</a>
            </td>
            <td>
                <b>
                    Refactor Platform Folder Structure #16
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
        Created At 2021-06-18 07:21:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/17" class=".btn">#17</a>
            </td>
            <td>
                <b>
                    additional documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - additional documentation
- integration test, basics: issuance process

Signed-off-by: Angelo De Caro <adc@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-17 14:16:31 +0000 UTC
    </div>
</div>

