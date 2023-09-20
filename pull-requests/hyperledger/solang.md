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
                PR <a href="https://github.com/hyperledger/solang/pull/1546" class=".btn">#1546</a>
            </td>
            <td>
                <b>
                    bugfix config file templates
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
        Created At 2023-09-20 15:12:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1545" class=".btn">#1545</a>
            </td>
            <td>
                <b>
                    add hint to install ninja
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
        Created At 2023-09-19 11:46:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1544" class=".btn">#1544</a>
            </td>
            <td>
                <b>
                    Fix mutability check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1493 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-18 20:49:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1543" class=".btn">#1543</a>
            </td>
            <td>
                <b>
                    Add ecrecover() builtin for EVM
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes https://github.com/hyperledger/solang/issues/1536
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-17 16:32:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1542" class=".btn">#1542</a>
            </td>
            <td>
                <b>
                    Solana: Implement a CLI Command for Program Deployment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description:
This pull request implements `solang solana deploy` command


Example: 
```bash
solang solana deploy --output-json flipper.so
```

### Checklist
- [x] Tested the new commands using a shell script `integration/solana/cli_test.sh`
- [x] Added documentation
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-17 15:17:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1541" class=".btn">#1541</a>
            </td>
            <td>
                <b>
                    Format source code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We are importing `forge-fmt` for two reasons:
 - This ensures that forge-fmt uses the latest solang-parser crate, and we only have one version of solang-parser in solang binary
 - This makes it possible to publish the solang crate to crates.io, since forge-fmt is not on crates.io and no git depdendencies are allowed
 - We requested feedback from Foundry on their discord server but received no feedback 

This feature is enabled with the help of  [forge-fmt](https://github.com/foundry-rs/foundry/tree/master/crates/fmt). 

Cc: @gakonst @DaniPopes 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-17 04:46:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1540" class=".btn">#1540</a>
            </td>
            <td>
                <b>
                    Implement Go To Declaration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                -  gives a list of contract methods that the given contract method overrides.
-  only returns the methods belonging to the immediate parent contracts.
-  handles multiple inheritance.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-17 02:20:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1539" class=".btn">#1539</a>
            </td>
            <td>
                <b>
                    solc allows @param tag for return values
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                @return should be used, warn about this.

https://github.com/hyperledger/solang/issues/1533
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-16 09:40:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1531" class=".btn">#1531</a>
            </td>
            <td>
                <b>
                    Verify account space specified in annotation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">solana</span>
            </td>
            <td>
                On Solana, we can specify the space necessary for a contract's data account in the constructor with an annotation. We do not verify, however, if the declared space is enough to hold all the contract variables. As a consequence, we could call the constructor without any issue using a very small space value and hit other runtime errors later.

PS: I found it unpleasant to keep iterating over the constructor annotations to find the one we were looking for, so I replaced the vector by a struct to hold the permitted annotations.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-14 22:35:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1530" class=".btn">#1530</a>
            </td>
            <td>
                <b>
                    Permit memory-safe flag on assembly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes https://github.com/hyperledger/solang/issues/1526
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-14 14:59:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1529" class=".btn">#1529</a>
            </td>
            <td>
                <b>
                    Add support for custom tags
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes https://github.com/hyperledger/solang/issues/1524
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-14 14:33:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1528" class=".btn">#1528</a>
            </td>
            <td>
                <b>
                    Allow using {func} for type to use library functions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes https://github.com/hyperledger/solang/issues/1525
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-14 14:05:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1527" class=".btn">#1527</a>
            </td>
            <td>
                <b>
                    Fix type(int256).min in comparisons
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When resolving comparisons, we don't know what the types of the operands are so we resolve with `ResolveTo::Unknown`. In this path, there is an mistake in the bounds check for negative integers.

Fixes https://github.com/hyperledger/solang/issues/1523
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-14 12:00:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1522" class=".btn">#1522</a>
            </td>
            <td>
                <b>
                    Fix recursive struct issue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Structs that contains themselves in a dynamic array are not recursive and do not have infinite size, as in the example below:
```solidity
struct C {
    C [2][3][][2] m;
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-13 22:32:00 +0000 UTC
    </div>
</div>

