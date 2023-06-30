---
layout: default
title: solang
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v0.3.1 Göttingen
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.3.1
                </span>
            </td>
            <td>
                ### Added
- Write environment configuration into Substrate metadata. [xermicus](https://github.com/xermicus)
- Tornado cash as an exemplary integration test for Substrate chain extensions. [xermicus](https://github.com/xermicus)
- `is_contract` runtime API is available as a builtin for Substrate. [xermicus](https://github.com/xermicus)
- The `wasm-opt` optimizer now optimizes the Wasm bytecode on the Substrate target. [xermicus](https://github.com/xermicus)
- Call flags are now available for Substrate. [xermicus](https://github.com/xermicus)
- Read compiler configurations from toml file. [salaheldinsoliman](https://github.com/salaheldinsoliman)
- Accounts declared with `@payer(my_account)` can be accessed with the
  syntax `tx.accounts.my_account`. [LucasSte](https://github.com/LucasSte)
- `delegatecall()` builtin has been added for Substrate. [xermicus](https://github.com/xermicus)
- `get_contents_of_file_no` for Solang parser. [BenTheKush](https://github.com/BenTheKush)
- `set_code_hash()` builtin has been aded for Substrate. [xermicus](https://github.com/xermicus)

### Fixed
- Diagnostics do not include large numbers anymore. [seanyoung](https://github.com/seanyoung)
- Correctly parse and resolve `require(i < 2**255)`. [seanyoung](https://github.com/seanyoung)
- Virtual function are available for call. [xermicus](https://github.com/xermicus)
- Allow `.wrap()` and `.unwrap()` user defined type methods in constants. [xermicus](https://github.com/xermicus)
- `@inheritdoc` now works with bases of bases. [seanyoung](https://github.com/seanyoung)
- Allow destructures to assign to storage variables. [seanyoung](https://github.com/seanyoung)
- Do not allow push and pop in fixed length arrays. [LucasSte](https://github.com/LucasSte)
- Improve unused variable elimination to remove unused arrays. [LucasSte](https://github.com/LucasSte)
- Salt argument should be of type `bytes32`. [seanyoung](https://github.com/seanyoung)
- Allow return vallues to be ignored in try-catch statements. [seanyoung](https://github.com/seanyoung)
- Optimize modifiers' CFGs. [xermicus](https://github.com/xermicus)
- Fix an error whereby building large contracts would cause an LLVM error. [LucasSte](https://github.com/LucasSte)
- A constructor for a Solana contract cannot run twice on the same data account. [seanyoung](https://github.com/seanyoung)
- Split the `call` and `deploy` dispatches on Substrate. [xermicus](https://github.com/xermicus)

### Changed
-  Minimum Supported Rust Version (MSRV) is Rust `1.68`.
- `@payer` annotation declares an account in a constructor. [LucasSte](https://github.com/LucasSte)
- Do not allow `.call()` functions in functions declared as view. [seanyoung](https://github.com/seanyoung)
- Storage accessor function matches solc, and returns struct members if the sole return value is a single struct [seanyoung](https://github.com/seanyoung)
- **breaking** Constructor annotations above a constructor can either declare an account or receive a literal parameter. [LucasSte](https://github.com/LucasSte)
  ```
  contract MyContract {
    @payer(acc) // Declares account acc
    @space(2+3) // Only literals or constant expressions allowed
    @seed(myseed) // NOT ALLOWED
    constructor(bytes myseed) {}
  }
  ```
- Annotations placed before constructor arguments refer to the latter. [LucasSte](https://github.com/LucasSte)
  ```
  contract MyContract {
    @payer(acc) // Declares account acc
    @space(2+3) // Only literals or constant expressions allowed
    constructor(@seed bytes myseed) {}
    // When an annotations refers to a parameter, the former must appear right before the latter.
  }
  ```
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/solang/releases/tag/v0.3.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-06-30 17:24:31 +0000 UTC
    </span>
</div>

