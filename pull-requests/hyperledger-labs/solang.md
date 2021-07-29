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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/454" class=".btn">#454</a>
            </td>
            <td>
                <b>
                    Cleanup sema/codegen separation, improve mutability/visibility checks on override
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-29 10:39:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/453" class=".btn">#453</a>
            </td>
            <td>
                <b>
                    Split sema expression into smaller function to reduce stack usage
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
        Created At 2021-07-28 14:35:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/451" class=".btn">#451</a>
            </td>
            <td>
                <b>
                    Reduce the stack frame on the Solana bundle and modifier fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Turns out, the llvm does not take lifetime into consideration when
creating stack frames. All the stack space created with alloca is just
bundled into a single mega stack frame. Unfortunately, this is limited
to 4096 bytes and if the stack frame is larger, then you will get access
violation errors.

The solang_dispatch() function contained the dispatch for every function
in every contract. The dispatch includes the abi decoding; so, split
this into per-contract dispatch.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-26 21:15:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/449" class=".btn">#449</a>
            </td>
            <td>
                <b>
                    Make sure build works with latest solana_rbpf 0.2.14
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
        Created At 2021-07-23 18:10:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/448" class=".btn">#448</a>
            </td>
            <td>
                <b>
                    Unused variable elimination
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements unused variable elimination for the Solang compiler and improves the unused variable detection.

For unused variable detection, this PR improves the following cases:

- Variables inside `format()`
- Functions assigned to local variables
- Storage load
- Usage of methods `address` and `selector`

For the unused variable elimination, the PR allows Solang to remove from the intermediate representation the following cases:

- Variables that have never been read nor assigned.
- Variables that have been assigned but never read.
- Assignments of unused variables, including destructures.
- Assignments of unused variables inside expressions (`a = b + (c = 1)`)

This PR is part of the Linux Foundation mentorship for the Solang compiler. For more information, please refer to the [project plan](https://wiki.hyperledger.org/display/INTERN/Project+plan+-+Solang+compiler+passes+2021).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-23 14:33:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/447" class=".btn">#447</a>
            </td>
            <td>
                <b>
                    Solana bundled contract fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-23 09:33:04 +0000 UTC
    </div>
</div>

