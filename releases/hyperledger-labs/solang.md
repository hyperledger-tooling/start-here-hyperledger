---
layout: default
title: solang
parent: Hyperledger Labs
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger-labs/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v0.1.12: Cairo Release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.1.12
                </span>
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

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger-labs/solang/releases/tag/v0.1.12" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-06-09 07:33:08 +0000 UTC
    </span>
</div>

