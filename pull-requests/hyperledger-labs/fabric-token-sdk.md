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
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/598" class=".btn">#598</a>
            </td>
            <td>
                <b>
                    F append tokens
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
        Created At 2024-04-11 13:59:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/597" class=".btn">#597</a>
            </td>
            <td>
                <b>
                    store token request hash in rwsets
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-11 08:44:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/596" class=".btn">#596</a>
            </td>
            <td>
                <b>
                    support for transaction status message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR does the following:
- the dbs contain a status message too
- TxStatus has been converted to int
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-09 08:19:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/595" class=".btn">#595</a>
            </td>
            <td>
                <b>
                    Integration tests with replicas
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
        Created At 2024-04-09 08:15:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/593" class=".btn">#593</a>
            </td>
            <td>
                <b>
                    new finality based on local dbs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-09 04:48:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/592" class=".btn">#592</a>
            </td>
            <td>
                <b>
                    change max token calculation to use big int because high float64 is h…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …andled unreliably across architectures.

Found this out when creating the tokengen params on arm64 and then running the code on amd64... See also https://groups.google.com/g/golang-nuts/c/YxpOo02fT9s?pli=1. I also noticed the original code does -1, whereas I had to -2 to get the same result for a bitlength of 64.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-08 15:10:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/590" class=".btn">#590</a>
            </td>
            <td>
                <b>
                    tokengen: print commit version, time, and modified flag
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-08 10:52:30 +0000 UTC
    </div>
</div>

