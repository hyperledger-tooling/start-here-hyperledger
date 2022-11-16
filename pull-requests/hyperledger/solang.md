---
layout: default
title: solang
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1070" class=".btn">#1070</a>
            </td>
            <td>
                <b>
                    Improve naming
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Rename `send_events` to `emits_events` (`emits_events` is used elsewhere)
- Rename `AllocDynamicArray` to `AllocDynamicBytes` (allocates `Type::DynamicBytes` or `Type::String`)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-16 12:04:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1068" class=".btn">#1068</a>
            </td>
            <td>
                <b>
                    improved parser recovery
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Improved Solang-parser resilience. 
Signed-off-by: salaheldinsoliman <salaheldin_sameh@aucegypt.edu>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-12 15:28:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1067" class=".btn">#1067</a>
            </td>
            <td>
                <b>
                    Ensure trailing - on scientific notation is not parsed as part of number
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ```
function test() external {
    uint256 b = 500;
    uint256 a1 = 1e18-b;
    uint256 a2 = 1e18- b;
}
```

Fixes https://github.com/hyperledger/solang/issues/1065

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-12 09:46:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1066" class=".btn">#1066</a>
            </td>
            <td>
                <b>
                    Documentation cleanup and rename Ternary to ConditionalOperator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I read through our documentation - only got halfway through!

Just because a conditional operator takes three parameters does not mean it should be called ternary. It's just not very descriptive. Also, we might invent another operator which also takes three operators.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-11 16:14:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1064" class=".btn">#1064</a>
            </td>
            <td>
                <b>
                    Substrate: Fix events with topics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #970 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-11 10:24:02 +0000 UTC
    </div>
</div>

