---
layout: default
title: solang
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1079" class=".btn">#1079</a>
            </td>
            <td>
                <b>
                    Switch `ink!` dependency to beta release
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
        Created At 2022-11-22 13:19:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1078" class=".btn">#1078</a>
            </td>
            <td>
                <b>
                    Use named fields for casts in ast::Expression
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
        Created At 2022-11-21 08:46:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1077" class=".btn">#1077</a>
            </td>
            <td>
                <b>
                    Validate documentation examples on CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR moves most of our solidity code blocks into dedicated examples. Snippets that should work for all our targets go into the `/examples` directory, and target specific ones into `/examples/target`. I implemented a test to check that all examples successfully compile, in parallel.

Also a lot of examples contained syntactical errors, I fixed everything. Additionally they are now correctly formatted.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-18 17:20:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1075" class=".btn">#1075</a>
            </td>
            <td>
                <b>
                    Fix bytes() cast from fixed length and vice versa
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
        Created At 2022-11-18 13:33:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1074" class=".btn">#1074</a>
            </td>
            <td>
                <b>
                    Use IndexMap for enum declaration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previously, we had a `HashMap<String, (Loc, usize)>` to save the items of an enumeration. Retrieving the item name having its index is awful, so I changed the structure to `IndexMap<String, Loc>`, from which we can retrieve its name and Loc when we index it with an `usize`.

The context for this PR is that I need to retrieve the item name from its index when generating the Anchor IDL from a Solidity contract.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-17 18:59:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1072" class=".btn">#1072</a>
            </td>
            <td>
                <b>
                    Rename ast::Expression::AllocDynamicArray to AllocDynamicBytes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The CFG expression was already renamed, rename the AST expression to match.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-17 10:50:06 +0000 UTC
    </div>
</div>

