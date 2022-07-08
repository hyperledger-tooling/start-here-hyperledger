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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/909" class=".btn">#909</a>
            </td>
            <td>
                <b>
                    Reduce the number of public items in the crates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Reduce the number of public items in the crates
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-07 13:58:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/907" class=".btn">#907</a>
            </td>
            <td>
                <b>
                    solang version information missing when built outside of git
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The build.rs uses `git describe --tags` to get the version for `solang
--version`. When built outside of git, use the crate version.

This affects the brew build of solang.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-05 10:35:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/906" class=".btn">#906</a>
            </td>
            <td>
                <b>
                    WIP: Borsh encoding
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is a work in progress for the Borsh Encoding. It will allow us to call Rust contracts on Solana.

Task list:

- [x] Implement the encoding
- [x] Create code generation tests
- [ ] Create runtime tests
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-04 22:34:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/905" class=".btn">#905</a>
            </td>
            <td>
                <b>
                    Parse tree should specify if string literal was unicode"foo" (#2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                PR #902 attempted to fix this, but only added this to the lexer, not
the parse tree. This adds a boolean to the parse tree.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-04 08:39:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/904" class=".btn">#904</a>
            </td>
            <td>
                <b>
                    Bump solang-parser version for publish
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Foundry's forge-fmt needs a new solang-parser release.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-03 14:02:00 +0000 UTC
    </div>
</div>

