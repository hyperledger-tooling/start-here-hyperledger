---
layout: default
title: solang
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1013" class=".btn">#1013</a>
            </td>
            <td>
                <b>
                    Fix random test failure in test_mul_within_range
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If gen_biguint() generated a 0, then the sub(1) will cause the test to fail.

See https://github.com/hyperledger/solang/actions/runs/3044527275/jobs/4905014572

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-13 12:03:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1012" class=".btn">#1012</a>
            </td>
            <td>
                <b>
                    Add semantic information to CFG
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR should help @salaheldinsoliman implement overflow detection for constants in the CFG. It adds information about the origin of each instruction to the CFG. Each instruction is now classified either as from Solidity, Yul or Codegen.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-12 21:19:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1011" class=".btn">#1011</a>
            </td>
            <td>
                <b>
                    Fix function calls via contract name
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                Disallow direct access to functions (and constants) except for base contracts. This is not valid in `solc` but was allowed in solang.

Fixes #1007 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-12 12:16:22 +0000 UTC
    </div>
</div>

