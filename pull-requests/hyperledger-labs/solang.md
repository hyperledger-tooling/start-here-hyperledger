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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/886" class=".btn">#886</a>
            </td>
            <td>
                <b>
                    Ensure storing array literal in storage works correctly on substrate and ewasm
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes https://github.com/hyperledger-labs/solang/issues/859

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-21 14:39:30 +0000 UTC
    </div>
</div>

