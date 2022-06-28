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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/899" class=".btn">#899</a>
            </td>
            <td>
                <b>
                    Improve yul tests coverage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                PR #891 introduced a new Yul builtin, but it did not include code generation tests for it, decreasing our code coverage. Code generation tests should test all possible code paths.

This PR includes `extcodesize` to the code generation tests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 13:48:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/898" class=".btn">#898</a>
            </td>
            <td>
                <b>
                    Dirty tracker should track all variables up to point where it is created
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Our `Vartable` tracks variables that need Phi instructions when generating LLVM IR. The way it was designed, our dirty tracker was only considering variables whose number was less than `ns.next_id`, ignoring temporaries created during code generation. This leads to an incorrect management of Phi instructions.

By considering the limit for dirty tracker as the `vartable.next_id`, we account for all variables created up to the point where we create a new dirty tracker. This allows us to remove the manual insertion of temporaries to the phis set.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 13:38:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/896" class=".btn">#896</a>
            </td>
            <td>
                <b>
                    Ensure that parenthesis are added to the parse tree
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                forge fmt uses the solang-parser crate for formatting solidity code.
However, currently parenthesis are not added to the parse tree, which
makes reconstructing the source text difficult.

This means that the parse tree for `(1 + 2) * 3` contains an explicit
node for the parenthesis around the expression `1 + 2`.

See https://discord.com/channels/900503503162724452/975868842125455390/990812142049566770

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-27 09:48:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/895" class=".btn">#895</a>
            </td>
            <td>
                <b>
                    Create universal binary for mac
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-25 09:20:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/893" class=".btn">#893</a>
            </td>
            <td>
                <b>
                    Ensure that codegen is correct for push/pop in if statements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A push or pop may result in a realloc, so we need a phi node for the
array variable.

See https://discord.com/channels/905194001349627914/905834552965103638/989739679320535050

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-24 12:01:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/891" class=".btn">#891</a>
            </td>
            <td>
                <b>
                    Wire up extcodesize for ewasm
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes https://github.com/hyperledger-labs/solang/issues/852

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-23 08:49:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/890" class=".btn">#890</a>
            </td>
            <td>
                <b>
                    Build multiarch containers on linux-arm64, and only on main branch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The multiarch container build on macos is failing often, try on
linux-arm64 in stead.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 20:49:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/888" class=".btn">#888</a>
            </td>
            <td>
                <b>
                    Clarify MacOS installation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I added a few new lines to the documentation to clarify the procedure to download and use the pre-compiled binary on MacOS.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 13:20:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/887" class=".btn">#887</a>
            </td>
            <td>
                <b>
                    Ensure push and subscript works on multi-dimensional arrays
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes https://github.com/hyperledger-labs/solang/issues/860

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 09:47:41 +0000 UTC
    </div>
</div>

