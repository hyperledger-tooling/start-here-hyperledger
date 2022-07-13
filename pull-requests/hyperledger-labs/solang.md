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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/917" class=".btn">#917</a>
            </td>
            <td>
                <b>
                    Add Cyrill to maintainers list
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also quickly made the github handles clickable :upside_down_face: 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-13 11:23:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/914" class=".btn">#914</a>
            </td>
            <td>
                <b>
                    Documentation: Clarify that mock VM implementations may omit aspects …
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …not mattering in unit tests

As discussed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-12 10:29:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/913" class=".btn">#913</a>
            </td>
            <td>
                <b>
                    Fix vscode extension build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Looks like @types/vscode 1.69.0 is broken. Do not use this version.

vscode-test has been renamed to @vscode/test-electron, update this too.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-12 09:10:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/912" class=".btn">#912</a>
            </td>
            <td>
                <b>
                    Support length for storage strings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add support for retrieving the length of a string saved in storage. I implemented this to help me debug an issue with Borsh Encoding.

Solc does not support this.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-11 20:19:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/911" class=".btn">#911</a>
            </td>
            <td>
                <b>
                    Update seal debug message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The `seal_println` runtime function was superseded by `seal_debug_message` in Substrate v3.0. This PR makes the `print("...")` builtin work again for current Substrate versions.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-11 13:31:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/910" class=".btn">#910</a>
            </td>
            <td>
                <b>
                    Allow free functions to be imported
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Free functions (ie. functions outside of contracts) where not imported.
Fix this.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 10:12:05 +0000 UTC
    </div>
</div>

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

