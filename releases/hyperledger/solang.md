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
                    Alexandria
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.2.2
                </span>
            </td>
            <td>
                ### Added
- Solidity mappings can now have named key and named value types. [seanyoung](https://github.com/seanyoung)

### Changed
- Solang now uses LLVM 15. [LucasSte](https://github.com/LucasSte)
- Solidity on Solana now required the Anchor framework for the client code, and the `@solana/solidity.js`
  Typescript library is no longer compatible with Solidity.
- When casting hex literal numbers into the `bytesN` type, the hex literal may use leading zeros to match the size
with the according `bytesN`, which aligns solang with `solc`. [xermicus](https://github.com/xermicus)

### Fixed
- Many bugs have been fixed by [seanyoung](https://github.com/seanyoung), [LucasSte](https://github.com/LucasSte)
  and [xermicus](https://github.com/xermicus)
- Typos throughout the code have been fixed. [omahs](https://github.com/omahs)

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/solang/releases/tag/v0.2.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-02-20 18:07:51 +0000 UTC
    </span>
</div>

