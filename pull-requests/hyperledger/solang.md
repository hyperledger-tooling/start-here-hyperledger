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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1309" class=".btn">#1309</a>
            </td>
            <td>
                <b>
                    Fix the formatting in the chain extension documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Sorry for this annoyance. I should have checked it before. I just assumed because it rendered it would look fine :grin:
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-11 17:37:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1307" class=".btn">#1307</a>
            </td>
            <td>
                <b>
                    Read compiler configurations from toml file.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1- Refactor `solang.rs`
2- Create a Struct `Configurations`, that can be created from the command line or from a `.toml` file.
3- Create a new subcommand `solang new`, which creates a project directory that includes a solidity example `flipper.sol` and `Solang.toml`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-11 02:10:23 +0000 UTC
    </div>
</div>

