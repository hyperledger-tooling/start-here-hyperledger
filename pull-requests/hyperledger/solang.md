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
                PR <a href="https://github.com/hyperledger/solang/pull/1077" class=".btn">#1077</a>
            </td>
            <td>
                <b>
                    WIP: Validate doc examples
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Move full contract solidity code blocks into dedicated examples (and fix many syntax errors in the process)
- Check for their successful compilation
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-18 17:20:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1075" class=".btn">#1075</a>
            </td>
            <td>
                <b>
                    Fix bytes() cast from fixed length and vice versa
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-18 13:33:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1074" class=".btn">#1074</a>
            </td>
            <td>
                <b>
                    Use IndexMap for enum declaration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previously, we had a `HashMap<String, (Loc, usize)>` to save the items of an enumeration. Retrieving the item name having its index is awful, so I changed the structure to `IndexMap<String, Loc>`, from which we can retrieve its name and Loc when we index it with an `usize`.

The context for this PR is that I need to retrieve the item name from its index when generating the Anchor IDL from a Solidity contract.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-17 18:59:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1072" class=".btn">#1072</a>
            </td>
            <td>
                <b>
                    Rename ast::Expression::AllocDynamicArray to AllocDynamicBytes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The CFG expression was already renamed, rename the AST expression to match.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-17 10:50:06 +0000 UTC
    </div>
</div>

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

