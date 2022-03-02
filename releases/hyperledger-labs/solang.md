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
                    
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.1.10
                </span>
            </td>
            <td>
                ## Added
- On Solana, the accounts that were passed into the transactions are listed in
  the `tx.accounts` builtin. There is also a builtin struct `AccountInfo`
- A new common subexpression elimination pass was added, thanks to
  [LucasSte](https://github.com/hyperledger-labs/solang/pull/550)
- A graphviz dot file can be generated from the ast, using `--emit ast-dot`
- Many improvements to the solidity parser, and the parser has been spun out
  in it's own create `solang-parser`.

## Changed
- Solang now uses LLVM 13.0, based on the [Solana LLVM tree](https://github.com/solana-labs/llvm-project/)
- The ast datastructure has been simplified.
- Many bugfixes across the entire tree.
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger-labs/solang/releases/tag/v0.1.10" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-03-01 18:22:55 +0000 UTC
    </span>
</div>

