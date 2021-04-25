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
                PR <a href="https://github.com/hyperledger/grid/pull/653" class=".btn">#653</a>
            </td>
            <td>
                <b>
                    Update Grid Logo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updates the Grid logo used by the Grid UI. This version has a white
background instead of a transparent one.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-23 17:02:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/652" class=".btn">#652</a>
            </td>
            <td>
                <b>
                    Use "just" recipes during CI builds
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
        Created At 2021-04-22 20:03:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/651" class=".btn">#651</a>
            </td>
            <td>
                <b>
                    Add purchase_order to the list of crates in justfile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-22 20:01:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/650" class=".btn">#650</a>
            </td>
            <td>
                <b>
                    Add cross-cutting db features
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds cross-cutting features to the Grid SDK for the locations, products, and schemas modules. These features control whether the db code for each module gets compiled.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-22 19:34:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/649" class=".btn">#649</a>
            </td>
            <td>
                <b>
                    Update Products Table page
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updates the ProductsTable component per the updated designs for the Product sapling. This uses the other new/updated components. This page now contains a table  that displays products for a chosen service. This table is filterable and product xml files can be downloaded directly from the table.

## Testing

 - Start the splinter example docker containers and run through creating a circuit and adding product to that circuit
 - in a separate terminal navigate to the `ui/grid-ui` directory and run `npm i` and `npm run start`
 - in a separate terminal navigate to the `ui/saplings/product` directory and run `npm i` and `npm run watch`
 - in a browser, navigate to `localhost:3030`, sign in, go to the product sapling
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-21 17:03:43 +0000 UTC
    </div>
</div>

