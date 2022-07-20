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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/929" class=".btn">#929</a>
            </td>
            <td>
                <b>
                    Arrays' outer dimension is the only one allowed to be dynamic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR defaults the last dimension of multidimensional arrays as the only one that can be dynamic. It fixes issue #903 only for Solana.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-19 18:22:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/928" class=".btn">#928</a>
            </td>
            <td>
                <b>
                    When pushing new element onto array, do not free existing data
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This data will be stale and may lead to corruption.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-19 16:13:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/927" class=".btn">#927</a>
            </td>
            <td>
                <b>
                    codegen: print the require error string for target substrate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Since we have now debug prints working in substrate, error strings from `require` assertions can be appended the debug message buffer. This should make debugging during contract development much easier.

This should pass integration tests as soon as they use an up-to-date substrate version.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-19 13:28:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/925" class=".btn">#925</a>
            </td>
            <td>
                <b>
                    Fix parsing of `uint x = 1 /** foo */ + 2;`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                DocComments should not be stored in the parse tree.

There are two commits, the first fixes an issue with  the existing doccomment parsing (and adjusts the test results).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-18 11:55:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/924" class=".btn">#924</a>
            </td>
            <td>
                <b>
                    Improve slice support and add `create_program_address()` solana builtin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Wire up `create_program_address` for Solana. 
 - This solana system calls uses slices. The data pointer is 64 bit and and the length is also 64 bit
 - This system call takes an array of slices, of any length. The length is another system call parameter
 
So, we make the following changes:
 - `bytes` can be implicitly cast to a slice of `bytes1`. This requires runtime code.
 - a string or hex literal can be implicitly cast to a slice of `bytes1`
 - We introduce a new array length "any fixed length", which we use a parameter type to the system call.
 - We introduce a new system call which can be imported using `import {create_program_address} from 'solana';`
 - Tests for this system call (both mock solana and against a running local node).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-18 08:09:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/921" class=".btn">#921</a>
            </td>
            <td>
                <b>
                    Refactor strength reduce
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In my Borsh Encoding PR #906, strength reduce was overflowing the stack for some complex encoding cases. This PR decreases the stack size from 2KB to 768 bytes for the `reaching_values` function and from 9KB to 800 bytes for the `expression_values` function.

This PR also includes a refactoring in the strength reduce files.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-15 18:45:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/920" class=".btn">#920</a>
            </td>
            <td>
                <b>
                    Do not resolve the arguments to overloaded functions/event emit twice
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This covers to overloaded functions, constructors, methods, and event emit.

This solves some issues wrt to slice support which is covered in a future PR.

Fixes #779 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-15 08:20:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/919" class=".btn">#919</a>
            </td>
            <td>
                <b>
                    Refactor size_of function
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The function `Type::size_of` is currently only used for calculation how much size a type occupies in storage. We do not utilize it to estimate the size of an item in the memory. This PR updates the function's name to properly represent what it returns and updates its description to encourage proper usage.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-13 15:16:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/918" class=".btn">#918</a>
            </td>
            <td>
                <b>
                    Fix load of vector of strings from storage on Solana
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Loading a vector of strings from storage was not working correctly. When we accessed the first element of the loaded array, we would get the wrong length, and consequently the wrong string. This PR fixes this problem.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-13 13:48:57 +0000 UTC
    </div>
</div>

