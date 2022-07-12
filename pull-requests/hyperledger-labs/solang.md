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
                    [WIP] Update seal debug message
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

