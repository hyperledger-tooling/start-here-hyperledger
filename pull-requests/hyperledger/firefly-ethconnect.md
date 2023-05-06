---
layout: default
title: firefly-ethconnect
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-ethconnect
---

# firefly-ethconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-ethconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/234" class=".btn">#234</a>
            </td>
            <td>
                <b>
                    Use Go 1.19 and update deps
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
        Created At 2023-05-05 20:30:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/233" class=".btn">#233</a>
            </td>
            <td>
                <b>
                    Differentiate bytes vs. fixed bytes in encoding parameters
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes https://github.com/hyperledger/firefly-ethconnect/issues/133

for a `bytes` parameter, to input an empty value, `0x` is the expected value. It fails the packing step and returns the error as described in the issue above.

This fixes that issue by differentiating bytes vs. fixed length bytes, and returns a slice vs. fixed length array respectively
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-04 20:33:31 +0000 UTC
    </div>
</div>

