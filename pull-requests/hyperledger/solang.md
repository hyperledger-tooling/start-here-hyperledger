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
                PR <a href="https://github.com/hyperledger/solang/pull/1319" class=".btn">#1319</a>
            </td>
            <td>
                <b>
                    v0.3.0 Venice
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The parser and semantic analysis stage of Solang have been through [a security audit](https://github.com/solana-labs/security-audits/blob/master/solang/Trail_of_Bits_Solang_Final_report.pdf). All security issues have been fixed.

### Added
- The CLI now has a `--release` option which disables printing of errors
- On Substrate, chain extensions can be now used. [xermicus](https://github.com/xermicus)

### Fixed
- Solidity error definitions are now parsed. [seanyoung](https://github.com/seanyoung)
- The Ethereum Solidity parser and semantic analysis tests are now run on Solang sema during `cargo test`. [seanyoung](https://github.com/seanyoung)
- If a function returned a `storage` reference, then not returning a value explicitly is an error, since the reference must post refer to an existing variable. [seanyoung](https://github.com/seanyoung)
- Many small improvements have been made to the parser and semantic analysis, improving compatibility with Ethereum Solidity.

### Changed
- Addresses are now base58 encoded when formated with `"address:{}".format(address)`. [LucasSte](https://github.com/LucasSte)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-19 15:10:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1317" class=".btn">#1317</a>
            </td>
            <td>
                <b>
                    `this` is not a keyword
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `this` should not be a keyword, and variables can be named `this` although this will hide the usual `this` which gives the current contract.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-19 11:01:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1316" class=".btn">#1316</a>
            </td>
            <td>
                <b>
                    Refactor Solang's CLI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Refactor Solang's CLI to prepare to parse CLI arguments easily from a `toml` file.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-19 02:29:50 +0000 UTC
    </div>
</div>

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

