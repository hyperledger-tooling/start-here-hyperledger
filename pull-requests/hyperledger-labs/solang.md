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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/446" class=".btn">#446</a>
            </td>
            <td>
                <b>
                    Ensure that enherited functions are also added to the abi file
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
        Created At 2021-07-21 14:50:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/445" class=".btn">#445</a>
            </td>
            <td>
                <b>
                    Ensure create contract works on Solana v1.7.3 and later
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
        Created At 2021-07-21 09:47:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/444" class=".btn">#444</a>
            </td>
            <td>
                <b>
                    Generate wasm and contract file for Substrate and other fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #443 

I think @athei asked for this feature too
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-20 09:09:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/442" class=".btn">#442</a>
            </td>
            <td>
                <b>
                    Improve warnings generated for incorrect function mutability
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
        Created At 2021-07-20 07:29:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/441" class=".btn">#441</a>
            </td>
            <td>
                <b>
                    Support immutable keyword
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
        Created At 2021-07-19 08:32:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/440" class=".btn">#440</a>
            </td>
            <td>
                <b>
                    Array codegen fix
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
        Created At 2021-07-18 10:16:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/439" class=".btn">#439</a>
            </td>
            <td>
                <b>
                    Improve error messages and only generate abis for concrete contracts
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
        Created At 2021-07-17 09:21:43 +0000 UTC
    </div>
</div>

