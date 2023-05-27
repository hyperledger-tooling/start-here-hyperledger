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
                PR <a href="https://github.com/hyperledger/solang/pull/1335" class=".btn">#1335</a>
            </td>
            <td>
                <b>
                    Bump `lalrpop` to 0.20
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <https://github.com/lalrpop/lalrpop/blob/master/RELEASES.md#0200-2023-05-02>

Test changes are due to "expected tokens in failed parses are more accurate".
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-27 14:28:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1332" class=".btn">#1332</a>
            </td>
            <td>
                <b>
                    Update substrate docker to use cargo contract 3.0
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
        Created At 2023-05-26 09:15:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1331" class=".btn">#1331</a>
            </td>
            <td>
                <b>
                    Update link to solang-llvm releases in `installing.rst`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change link to LLVM releases

#1330
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-26 07:25:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1329" class=".btn">#1329</a>
            </td>
            <td>
                <b>
                    Bump lalrpop and other dependencies
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
        Created At 2023-05-25 21:27:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1328" class=".btn">#1328</a>
            </td>
            <td>
                <b>
                    Make GetAddress return a pointer to an address
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In the same lines of #1325, loading addresses in codegen instead of emit allows us to leverage pointers to create `AccountMeta` arrays.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-25 20:41:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1327" class=".btn">#1327</a>
            </td>
            <td>
                <b>
                    chore(docs): fix discord link
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
        Created At 2023-05-25 13:24:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1326" class=".btn">#1326</a>
            </td>
            <td>
                <b>
                    Do not put huge numbers in diagnostics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Displaying huge number will costs lots of memory, cpu and is of no benefit.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-25 10:43:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1325" class=".btn">#1325</a>
            </td>
            <td>
                <b>
                    Load readonly members in codegen
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Whenever I retrieve a `StructMember` of the `AccountInfo` struct, Solang loads the pointer in emit. As a consequence, if I need to use the pointer again in codegen, I must save values on the stack and get their stack address.

For the new Solana account management, we are generating the `AccountMeta` array in codegen after retrieving the account addresses from `AccountInfo`. In this case, it is more efficient to use the pointer directly.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-24 21:05:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1324" class=".btn">#1324</a>
            </td>
            <td>
                <b>
                    Ensure that "require(i < 2**255);" parses correctly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Found with uniswap v3. This change also includes a little refactoring, and now Expression::NotEqual is generated by sema.

Before this change, 

```solidity
require(i < 2**255);
```
Gave the error: value 53919893334301279589334030174039261347274288845081144962207220498432 does not fit into type uint8.

This is because with `ResolveTo::Unknown` the integers default to the smallest size possible.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-23 18:35:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1323" class=".btn">#1323</a>
            </td>
            <td>
                <b>
                    Update to `ink!` v4.2 and bump MSRV to 1.68
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Spared this for after the release. Upgrading to the latest `ink!` version requires a MSRV of `1.68.0`. In my opinion this is fine because `1.69.0` is already out anyways.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-23 15:19:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1322" class=".btn">#1322</a>
            </td>
            <td>
                <b>
                    dev weekly seems gone and update solana installer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update `RELEASE_CHECKLIST.md` with observations releasing v0.3.0.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-23 12:50:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1320" class=".btn">#1320</a>
            </td>
            <td>
                <b>
                    solc does not warn or error for duplicate @param tags
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Make it a warning and add note to previous doc tag, and fix the locations.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-22 11:10:13 +0000 UTC
    </div>
</div>

