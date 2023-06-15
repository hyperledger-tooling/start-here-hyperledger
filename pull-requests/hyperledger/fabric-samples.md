---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1057" class=".btn">#1057</a>
            </td>
            <td>
                <b>
                    FSAT: Extend sleep time to stabilize integration test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This patch extends the sleep time to wait for starting nginx by following the description on [full-stack-asset-transfer-guide/justfile](https://github.com/hyperledger/fabric-samples/blob/ae9e7e8df8e2932e235a89b79c31dc54c47a3cf6/full-stack-asset-transfer-guide/justfile#L79) to stabilize the intergration test.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-12 08:24:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1056" class=".btn">#1056</a>
            </td>
            <td>
                <b>
                    Minor improvements on test-network-nano-bash
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Fix typos
- Update gitignore
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-12 07:52:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1053" class=".btn">#1053</a>
            </td>
            <td>
                <b>
                    Update token_contract.go, modify the overflow judgment condition for function sub().
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The general overflow judgment condition for function sub is not in every case.
The judgment result is wrong in the condition of b < 0 && q >=0
for example, b = -3, q = 2, diff = -5, it's not overflow,
but if (diff > b) == (b >= 0 && q >= 0) wil be true.

for another example, b = -3, q = maxint, b-q is overflow,
but if (diff > b) == (b >= 0 && q >= 0) wil be false.

I modify this line for making it use the same judgment logic as the function add().
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-08 07:46:26 +0000 UTC
    </div>
</div>

