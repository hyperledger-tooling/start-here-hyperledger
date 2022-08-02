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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/947" class=".btn">#947</a>
            </td>
            <td>
                <b>
                    Allow seeds to be passed to external calls for program signing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This allows a program to sign for itself when calling another program. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-02 15:10:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/946" class=".btn">#946</a>
            </td>
            <td>
                <b>
                    Bump solang-parser version for crate publish
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Foundry would like a new version
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-02 15:03:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/945" class=".btn">#945</a>
            </td>
            <td>
                <b>
                    Implement assignment to selector and address in Yul
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements assignment to an external function's selector and address in Yul, using the existing infrastructure in Solang.
The logic behind this is going to be used for Borsh decoding and brought up issue #944.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-01 13:31:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/943" class=".btn">#943</a>
            </td>
            <td>
                <b>
                    Merge readbuffer builtins
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR merges all the `codegen::Builtin::Read<type>` builtin type with a single `codegen::Builitin::ReadFromBuffer`, because they are all implemented equally in emit. This streamlines the development of `abi.decode` with Borsh encoding.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-28 17:27:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/942" class=".btn">#942</a>
            </td>
            <td>
                <b>
                    Enable initialization of arrays with array literals
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR enables the initialization of both dynamic memory and dynamic storage arrays with array literals. The limitation is that this works only for single dimensional arrays. It fixes issue #810.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-28 14:40:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/941" class=".btn">#941</a>
            </td>
            <td>
                <b>
                    Deploy does not want the program account
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This was changed in @solana/solidity 0.0.20 but the example here was not
updated.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-28 13:52:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/940" class=".btn">#940</a>
            </td>
            <td>
                <b>
                    Update installation instructions for MacOS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds the new installation instructions for MacOS on our documentation and our readme file. It also adds a new item to the release checklist to remind us of updating the cask file at each new release.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-28 12:54:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/939" class=".btn">#939</a>
            </td>
            <td>
                <b>
                    Update substrate links
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                All the links were broken.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-28 11:08:49 +0000 UTC
    </div>
</div>

