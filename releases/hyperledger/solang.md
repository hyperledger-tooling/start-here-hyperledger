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
                    
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.3.0
                </span>
            </td>
            <td>
                The parser and semantic analysis stage of Solang have gone through
[a security audit](https://github.com/solana-labs/security-audits/blob/master/solang/Trail_of_Bits_Solang_Final_report.pdf). All security issues have been fixed.

### Added
- The CLI now has a `--release` option, which disables printing of errors. [salaheldinsoliman](https://github.com/salaheldinsoliman)
- **Substrate**: chain extensions can be now used. [xermicus](https://github.com/xermicus)

### Fixed
- Solidity error definitions are now parsed. [seanyoung](https://github.com/seanyoung)
- The Ethereum Solidity parser and semantic analysis tests are now run on Solang sema during
  `cargo test`. [seanyoung](https://github.com/seanyoung)
- If a function returns a `storage` reference, then not returning a value explicitly is an error, since
  the reference must refer to an existing storage variable. [seanyoung](https://github.com/seanyoung)
- Many small improvements have been made to the parser and semantic analysis, improving compatibility
  with Ethereum Solidity. [seanyoung](https://github.com/seanyoung) [xermicus](https://github.com/xermicus) [LucasSte](https://github.com/LucasSte)

### Changed
- **Solana**: Addresses are now base58 encoded when formated with `"address:{}".format(address)`. [LucasSte](https://github.com/LucasSte)
- **Substrate**: No longer use the prefixed names for seal runtime API calls, which grants small improvements in contract sizes. [xermicus](https://github.com/xermicus)
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/solang/releases/tag/v0.3.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-05-22 20:24:50 +0000 UTC
    </span>
</div>

