---
layout: default
title: solang
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/866" class=".btn">#866</a>
            </td>
            <td>
                <b>
                    Submodules are now required to run tests
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
        Created At 2022-06-09 07:19:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/865" class=".btn">#865</a>
            </td>
            <td>
                <b>
                    Fix deletion of address from mappings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes the deletion of addresses on mappings, which was causing the compiler to crash.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-08 20:32:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/864" class=".btn">#864</a>
            </td>
            <td>
                <b>
                    Release v0.1.12 Cairo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Added
- Added spl-token integration for Solana
- Solang now generates code for inline assembly, including many Yul builtins

### Changed
- The documentation has been re-arranged for readability.
- The solang parser can parse the same syntax as Ethereum Solidity 0.8.

### Fixed
- Fixed many parser issues. Now solang-parser parses all files in the
  Ethereum Solidity test suite. First run
  `git submodule update --init --recursive` to fetch the test files, and
  then run the test with `cargo test --workspace`.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-08 19:25:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/863" class=".btn">#863</a>
            </td>
            <td>
                <b>
                    Fix right side of the Loc of ContractDefinition
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix the location of contract definition so it matches the entire definition, not just the name and base contracts.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-08 17:47:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/862" class=".btn">#862</a>
            </td>
            <td>
                <b>
                    Move to latest solana-rbpf crate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This crate is used for solana tests. The version used before this commit has an security issue:

Solana solana_rbpf before 0.2.29 has an addition integer overflow via invalid ELF program headers. elf.rs has a panic via a malformed eBPF program.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-08 09:01:37 +0000 UTC
    </div>
</div>

