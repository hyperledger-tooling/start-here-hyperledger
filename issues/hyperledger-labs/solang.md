---
layout: default
title: solang
parent: Hyperledger Labs
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger-labs/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger-labs/solang/issues/517" class=".btn">517</a>
            </td>
            <td>
                <b>
                    Is it possible to use LLVM Pass module in Solang?
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">help wanted</span>
            </td>
            <td>
                Hi there!

I'm curious about whether Solang supports loading LLVM Pass module to perform some preprocessing on the generated LLVM-IR.

For instance, we can use LLVM Pass module in clang like this:
`clang -Xclang -load -Xclang ../build/PlacementPass/libLLVMPassname.so demo.c -o demo`

Can Solang do the same thing?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 07:07:24 +0000 UTC
    </div>
</div>

