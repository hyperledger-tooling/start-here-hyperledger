---
layout: default
title: solang
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/855" class=".btn">#855</a>
            </td>
            <td>
                <b>
                    Yul documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds documentation for Yul. Changes in `docs/conf.py` were necessary to support a new linter for both Solidity and Yul.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-31 12:09:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/854" class=".btn">#854</a>
            </td>
            <td>
                <b>
                    Fix links in diagnostics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Links to documentation in diagnostics were broken by a documentation reorg
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-30 13:58:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/853" class=".btn">#853</a>
            </td>
            <td>
                <b>
                    Cache LLVM on Mac builders
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-29 09:50:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/851" class=".btn">#851</a>
            </td>
            <td>
                <b>
                    Ensure that contracts tests also emit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                WIP:

Now the test fails on tests/contract_testcases/solana/account_meta.sol
The codegen generated a double load on the pubkey in the return (I
think).

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-25 10:24:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/850" class=".btn">#850</a>
            </td>
            <td>
                <b>
                    refactor(arguments): Replace -O command line option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Replace llvm-like -O command with gcc-like
optimization
commands
according
to
https://llvm.org/doxygen/CodeGen_8h_source.html

Limit the command
to
only one argument
(one type of optimization)

Add basic help for the
-O
command to improve usability

BREAKING CHANGE: Optimization command -O now takes GCC-like arguments
(0,1,2 or s and 3)

Closes #534

Signed-off-by: Saladino Belisario <SaladinoBelisario@protonmail.ch>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-25 00:15:12 +0000 UTC
    </div>
</div>

