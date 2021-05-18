---
layout: default
title: fabric-gateway
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-gateway
---

# fabric-gateway <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-gateway){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/118" class=".btn">#118</a>
            </td>
            <td>
                <b>
                    Make it easier to submit string arguments in Go client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Since strings are more common than bytes as transaction function arguments, make the following naming changes in the Go client API:
- WithStringArguments(args ...string) -> WithArguments(args ...string)
- WithArgument(args ...[]byte) -> WithBytesArguments(args ...[]byte)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-14 15:04:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/117" class=".btn">#117</a>
            </td>
            <td>
                <b>
                    More Node API doc polishing
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
        Created At 2021-05-13 11:32:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/116" class=".btn">#116</a>
            </td>
            <td>
                <b>
                    Update Node API doc readme
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Align content more closely with other language API documentation homepages, and include a code example.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-12 16:50:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/115" class=".btn">#115</a>
            </td>
            <td>
                <b>
                    Better curve support in Node client signing implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Use the parameters (namedCurve) Object Identifier from the elliptic curve private key to pick the correct curve from a set of supported key types, instead of always using the P-256 curve.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-12 12:47:37 +0000 UTC
    </div>
</div>

