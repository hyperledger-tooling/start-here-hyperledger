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
                PR <a href="https://github.com/hyperledger/solang/pull/1315" class=".btn">#1315</a>
            </td>
            <td>
                <b>
                    Virtual functions are available for calls
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Virtual functions may not have a body, but they should still be callable.

Without this fix, the added testcase fails with this error which is wrong:

```
error: unknown function or type '_virtual'
  ┌─ /home/glow/code/solang/tests/contract_testcases/substrate/functions/virtual.sol:3:9
  │
3 │         _virtual();
  │         ^^^^^^^^
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-18 17:23:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1312" class=".btn">#1312</a>
            </td>
            <td>
                <b>
                    Restrict external function callable scope
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                On Solc, external functions can exclusively be called outside a contract. In order for use to accomplish #1251, we need to restrict their scope to can declare and organize the accounts the function needs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-15 21:24:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1311" class=".btn">#1311</a>
            </td>
            <td>
                <b>
                    Remove seal prefixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Since a while ago, the seal runtime API function imports do no longer need the `seal_` prefix. Since in Wasm the import name is found in the contract, it saves a few bytes in contract size. Unprefixed `return`  does not exist, and i left `seal_call` prefixed because it'll overwrite the `call` export.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-15 11:50:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1310" class=".btn">#1310</a>
            </td>
            <td>
                <b>
                    Use solc v0.8.20 testdata
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Ethereum Solidity 0.8.20 has been released. Update our tests to use their latest test files.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-12 17:18:45 +0000 UTC
    </div>
</div>

