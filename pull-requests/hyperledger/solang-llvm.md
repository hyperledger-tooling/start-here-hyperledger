---
layout: default
title: solang-llvm
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/solang-llvm
---

# solang-llvm <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/solang-llvm){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang-llvm/pull/20" class=".btn">#20</a>
            </td>
            <td>
                <b>
                    Use newer SBF target rather than BPF
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Solana's LLVM fork has a new SBF target which should be used rather than the BPF target.

Note that this creates a new ci image called `ci-2`, so that we can switch to the newer version of the CI image in a solang PR. This means there is should be no breakage.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-04 12:57:07 +0000 UTC
    </div>
</div>

