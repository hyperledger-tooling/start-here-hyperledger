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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/931" class=".btn">#931</a>
            </td>
            <td>
                <b>
                    Update substrate integration test environment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR upgrades the Substrate integration tests to work with an up-to-date Substrate runtime. The individual commits resemble more or less the steps needed to make this work. In summary:
* Switched to the `pullparitytech/contracts-ci-linux:production` image for having a node that will always be up-to-date
* Bump many npm deps in the testing frameworks
* Fix all test specs so the work again with the new runtime and updated deps
* Disable discovered regressions to make the GHA job pass

The regressions are most likely all related to issue #666. As discussed in today's stand up call, the plan is the following:
1. [In this PR] Update the integration test suite to work with current Substrate runtime, disabling any regressions related to runtime changes. This will let us continue to have a green CI setup on main. Based on that, a note in our `README.md` transparently informs what is not working and that we are aware.
2. Priority is on fixing issue #666 (and other potential metadata issues that may be discovered). Ideally this fixes all regressions.
3. Re-enable all tests that were disabled in this PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-20 16:00:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/929" class=".btn">#929</a>
            </td>
            <td>
                <b>
                    Use the dims.last() to retrieve the outer dimension of a multidimensional array
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR changes `dims[0]` to `dims.last()` to retrieve the outer dimension of a multidimensional array. It fixes issue #903 only for Solana.
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
                Wire up `create_program_address` and `try_find_program_address` for Solana. 

 - This solana system calls uses slices. The data pointer is 64 bit and and the length is also 64 bit
 - This system call takes an array of slices, of any length. The length is another system call parameter
 
So, we make the following changes:
 - `bytes` can be implicitly cast to a slice of `bytes1`. This requires runtime code.
 - a string or hex literal can be implicitly cast to a slice of `bytes1`
 - We introduce a new array length "any fixed length", which we use a parameter type to the system call.
 - We introduce a new system call which can be imported using `import {create_program_address} from 'solana';`
 - Tests for this system call (both mock solana and against a running local node).

We also add `tx.program_id` for Solana.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-18 08:09:26 +0000 UTC
    </div>
</div>

