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
                    V0.2.1: Rio
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.2.1
                </span>
            </td>
            <td>
                
## Added
- The Anchor IDL data structure is now generated for every Solana contract, although the actual IDL json file is not yet saved.
[LucasSte](https://github.com/LucasSte)

## Changed
- The Solana target now utilizes eight byte Anchor discriminators for function dispatch instead
of the four byte Ethereum selectors. [LucasSte](https://github.com/LucasSte)
- The deployment of contracts on Solana now follows the same scheme as Anchor. [seanyoung](https://github.com/seanyoung)
- Compares between rational literals and integers are not allowed. [seanyoung](https://github.com/seanyoung)
- Overriding the function selector value is now done using the `@selector([1, 2, 3, 4])`
  syntax, and the old syntax `selector=hex"12345678"` has been removed.
- `msg.sender` was not implemented correctly on Solana, and
  [has now been removed](https://solang.readthedocs.io/en/latest/targets/solana.html#msg-sender-solana).
  [seanyoung](https://github.com/seanyoung)
- Solang now uses LLVM 14. [LucasSte](https://github.com/LucasSte)

## Fixed
- Many bugs have been fixed by [seanyoung](https://github.com/seanyoung), [LucasSte](https://github.com/LucasSte)
  and [xermicus](https://github.com/xermicus)
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/solang/releases/tag/v0.2.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-01-05 19:56:06 +0000 UTC
    </span>
</div>

