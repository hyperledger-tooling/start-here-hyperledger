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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/692" class=".btn">#692</a>
            </td>
            <td>
                <b>
                    Pushing onto two different arrays causes many reallocations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes an issue raised on discord:

https://discord.com/channels/905194001349627914/905834552965103638/949343674272219226

On Solana, contract storage in storage in account data which is a
continious piece of memory. In order to support growable objects like
dynamic arrays, we have a mini heap implementation. This fixes a problem
in the realloc implementation.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-10 09:14:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/691" class=".btn">#691</a>
            </td>
            <td>
                <b>
                    Resolve assembly expressions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements the semantic analysis of YUL expressions. As we don't analyze YUL statements yet, there are workarounds to avoid warnings during build. There are also some `TODOs` in the code to indicate implementation details I must not forget when creating the analysis of statements.

I added most unity tests, however, a few were too difficult to create, because they required building a complex parse tree. I am going to test those functions as soon as the semantic analysis is complete for YUL.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-09 11:53:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/690" class=".btn">#690</a>
            </td>
            <td>
                <b>
                    Improve msg.sender test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates the test of `msg.sender`, according to the suggestions at issue #679.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-08 11:39:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/688" class=".btn">#688</a>
            </td>
            <td>
                <b>
                    Make u256 the default type for YUL variables
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                After our discussion, I changed the default types for YUL variables to maintain compatibility with EVM.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-04 17:40:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/687" class=".btn">#687</a>
            </td>
            <td>
                <b>
                    Resolve yul literals
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements the semantic analysis of YUL literals. The code is not yet fully integrated into Solang's sema, so there are workarounds to avoid build warnings.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-04 13:21:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/686" class=".btn">#686</a>
            </td>
            <td>
                <b>
                    Refactor unescape function
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The `unescape` function in `sema/expression` could not handle escape constructs, such as `\xf4` and `\u00c3`. This PR fixes such a bug.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-04 11:16:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/685" class=".btn">#685</a>
            </td>
            <td>
                <b>
                    WIP: array of structs should not be array of pointers to struct
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-04 09:51:10 +0000 UTC
    </div>
</div>

