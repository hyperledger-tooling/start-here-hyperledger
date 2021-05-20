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

