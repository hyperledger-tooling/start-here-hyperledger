---
layout: default
title: grid
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/grid
---

# grid <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/grid){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1000" class=".btn">#1000</a>
            </td>
            <td>
                <b>
                    Fix adding a new revision to the store
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes a bug when attempting to add a revision to the store when the
version doesn't yet exist. This now proprly creates the new version
first.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 14:59:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/999" class=".btn">#999</a>
            </td>
            <td>
                <b>
                    Update po update contract tests to use new api
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Old API for accepted version number used a string, but the new API uses
an option. This change updates the accepted version number calls in
tests to use the new API so the tests will now pass.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-25 19:47:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/998" class=".btn">#998</a>
            </td>
            <td>
                <b>
                    Make workflow status required for `po create`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The PO create command will panic if no workflow status is passed, and
the CreatePurchaseOrderPayloadBuilder requires it to function. This
change makes clap force the user to pass a workflow status.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-22 16:35:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/996" class=".btn">#996</a>
            </td>
            <td>
                <b>
                    Add alternate_id support to PO state proto
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds support for alternate IDs to the Purchase Order state proto.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 20:33:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/995" class=".btn">#995</a>
            </td>
            <td>
                <b>
                    Add `alternate_id` support to `grid po create` CLI command
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds support for adding alternate IDs to the `grid po create`
    command. Previously, this was omitted due to lack of support in the
    store and protocol code.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 19:56:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/994" class=".btn">#994</a>
            </td>
            <td>
                <b>
                    Base grid-cli on focal instead of sabre-cli
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previously we had a need for sabre cli alongside the grid cli but this is no
longer the case.

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 15:58:05 +0000 UTC
    </div>
</div>

