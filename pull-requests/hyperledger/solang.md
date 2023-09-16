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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1519" class=".btn">#1519</a>
            </td>
            <td>
                <b>
                    Verify magic number in fallback
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Presently, we do not check the magic number when we enter a fallback function. If it modifies or read the data account, a malefactor can forge an account so that the function would read or write malicious data. This PR fixes such an issue.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-12 19:59:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1518" class=".btn">#1518</a>
            </td>
            <td>
                <b>
                    Polkadot: Implemented Node Interactions in Solang's CLI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description:
This pull request implements `Polkadot` node interactions into `Solang`'s CLI, allowing users to:
- `upload`
- `instantiate`
- `call`
- `remove`  

### Key features include:
- Network Name Parameter: Allows users to specify the Polkadot network by name.

Example: `solang polkadot upload --suri //Alice --network rococo -x --output-json flipper.contract`

### Checklist
- [x] Tested the new commands using a shell script `integration/polkadot/cli_test.sh`.
- [x] Added documentation for the newly implemented commands.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-10 10:15:50 +0000 UTC
    </div>
</div>

