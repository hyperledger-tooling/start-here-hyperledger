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
                The parser and semantic analysis stage of Solang have gone through
[a security audit](https://github.com/solana-labs/security-audits/blob/master/solang/Trail_of_Bits_Solang_Final_report.pdf). All security issues have been fixed.

### Added
- The CLI now has a `--release` option, which disables printing of errors [salaheldinsoliman](https://github.com/salaheldinsoliman)
- **Substrate**: chain extensions can be now used.
  [xermicus](https://github.com/xermicus)

### Fixed
- Solidity error definitions are now parsed.
  [seanyoung](https://github.com/seanyoung)
- The Ethereum Solidity parser and semantic analysis tests are now run on Solang sema during
  `cargo test`.
  [seanyoung](https://github.com/seanyoung)
- If a function returns a `storage` reference, then not returning a value explicitly is an error, since
  the reference must refer to an existing storage variable.
  [seanyoung](https://github.com/seanyoung)
- Many small improvements have been made to the parser and semantic analysis, improving compatibility
  with Ethereum Solidity.
  [seanyoung](https://github.com/seanyoung)
  [xermicus](https://github.com/xermicus)
  [LucasSte](https://github.com/LucasSte)

### Changed
- **Solana**: Addresses are now base58 encoded when formated with `"address:{}".format(address)`.
  [LucasSte](https://github.com/LucasSte)
- **Substrate**: No longer use the prefixed names for seal runtime API calls, which grants small improvements in contract sizes. [xermicus](https://github.com/xermicus)

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

