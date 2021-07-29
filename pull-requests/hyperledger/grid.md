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
                PR <a href="https://github.com/hyperledger/grid/pull/885" class=".btn">#885</a>
            </td>
            <td>
                <b>
                    Keygen updates
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
        Created At 2021-07-27 20:18:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/847" class=".btn">#847</a>
            </td>
            <td>
                <b>
                    Add REST API specification for Purchase Order
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Darian Plumb <dplumb@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-26 19:25:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/846" class=".btn">#846</a>
            </td>
            <td>
                <b>
                    BACKPORT 0-2: Add bash completion for newly stabilized subcommands
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
        Created At 2021-07-23 15:59:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/845" class=".btn">#845</a>
            </td>
            <td>
                <b>
                    Add bash completion for newly stabilized subcommands
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
        Created At 2021-07-22 18:59:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/844" class=".btn">#844</a>
            </td>
            <td>
                <b>
                    Update release notes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds notes for the product table indicator and XML parsing namespaces.

Signed-off-by: Darian Plumb <dplumb@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-22 17:11:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/843" class=".btn">#843</a>
            </td>
            <td>
                <b>
                    Update CLI Format syntax in Man Pages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Noticed that the grid-docs didn't correctly format some values in tags.
These changes remedy the problem.

Signed-off-by: Kevin Johnson <kevin_johnson@cargill.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-22 16:37:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/842" class=".btn">#842</a>
            </td>
            <td>
                <b>
                    BACKPORT: Update CLI Format syntax in Man Pages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Noticed that the grid-docs didn't correctly format some values in tags.
These changes remedy the problem.

Signed-off-by: Kevin Johnson <kevin_johnson@cargill.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-22 15:07:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/841" class=".btn">#841</a>
            </td>
            <td>
                <b>
                    Create PO revision man pages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Man pages based off of REST API spec from the purchase order hackathon.

Signed-off-by: Kevin Johnson <kevin_johnson@cargill.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-22 13:28:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/840" class=".btn">#840</a>
            </td>
            <td>
                <b>
                    Fix some incorrect migration data
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a migration folder to both the sqlite and postgres migration modules to correct a few migration data inconsistencies. Mainly, this addresses two issues: 

- Down unused tables in the newly added `up.sql` file
   (This includes tables meant to store circuit data that are currently not being used to store any data)
- Correctly down some tables that are incorrectly downed in their respective migration modules 
    (The tables are downed in the original migration file using the command `DROP` rather than `DROP TABLE`)  
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-22 13:22:37 +0000 UTC
    </div>
</div>

