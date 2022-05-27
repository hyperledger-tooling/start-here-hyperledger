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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/848" class=".btn">#848</a>
            </td>
            <td>
                <b>
                    Ensure the documentation can be built
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add CI test for the docs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-24 15:13:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/844" class=".btn">#844</a>
            </td>
            <td>
                <b>
                    Refactor Solang docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR splits the old `language.rst` file into multiple files so that the user can see the sections on the navigation bar. I also re-organized the order of items in the bar.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-23 14:29:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/843" class=".btn">#843</a>
            </td>
            <td>
                <b>
                    Allow types to be called error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                solc allows this too.

Found in https://github.com/hyperledger-labs/solang/pull/787

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-21 07:45:44 +0000 UTC
    </div>
</div>

