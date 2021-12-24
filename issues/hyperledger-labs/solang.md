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
                Issue <a href="https://github.com/hyperledger-labs/solang/issues/581" class=".btn">581</a>
            </td>
            <td>
                <b>
                    Using SipHash with private node key
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">help wanted</span>
            </td>
            <td>
                I came across this section in the documentation:

> Solidity takes the keccak 256 hash of the key and the storage slot, and simply uses that to find the entry. There are no hash collision chains. This scheme is simple and avoids “hash flooding” attacks where the attacker chooses data which hashes to the same hash collision chain, making the hash table very slow; it will behave like a linked list.
>
> In order to implement mappings in memory, a new scheme must be found which avoids this attack. Usually this is done with SipHash, but this cannot be used in smart contracts since there is no place to store secrets. Collision chains are needed since memory has a much smaller address space than the 256 bit storage slots.
>
> Any suggestions for solving this are very welcome!

But it makes me wonder, why not use SipHash and have each node create its own private key? As long as they process transactions from the beginning without changing this private key, that should work, right?

Maybe I'm missing something though.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-27 20:30:41 +0000 UTC
    </div>
</div>

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

