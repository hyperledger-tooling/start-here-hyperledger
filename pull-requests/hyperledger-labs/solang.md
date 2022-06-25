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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/894" class=".btn">#894</a>
            </td>
            <td>
                <b>
                    Do not build clang for the release library
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There is no need to build clang for the release LLVM binaries. We can compile and run Solang without clang. I was able to reduce the Linux x86 LLVM tarball from 305 MB to 170 MB.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-24 18:53:29 +0000 UTC
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/885" class=".btn">#885</a>
            </td>
            <td>
                <b>
                    Replace curly quotes with ascii single quote
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We use ascii quotes in diagnostics, these ones were missed.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-21 08:14:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/884" class=".btn">#884</a>
            </td>
            <td>
                <b>
                    Do not give up resolving a file if any errors were found in any file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently, if there are any errors found in any file, then we do not
resolve anything beyond the types.

This is a step towards solang not giving up early when there are errors in the file; we should always continue and resolve as much as possible.

Fixes #830 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 11:20:59 +0000 UTC
    </div>
</div>

