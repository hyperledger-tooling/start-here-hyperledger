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
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/35" class=".btn">#35</a>
            </td>
            <td>
                <b>
                    tokengen: add ability to generate artifacts #34
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - added a new command to tokengen to generate artifacts (copied from the smart client)
- fix to Makefile
- added sampleconfig folder with topologies

Signed-off-by: Angelo De Caro <adc@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-25 08:16:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/31" class=".btn">#31</a>
            </td>
            <td>
                <b>
                    [WIP] Owner encodes a type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-24 12:55:29 +0000 UTC
    </div>
</div>

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

