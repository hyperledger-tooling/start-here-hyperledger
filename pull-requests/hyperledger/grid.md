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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/839" class=".btn">#839</a>
            </td>
            <td>
                <b>
                    Add experimental support for Cylinder JWTs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds support for using Cylinder JWTs as an Auth header in requests
to submit batches. This new functionality is guarded behind the
experimental `cylinder-jwt-support` feature. This creates the Signer in
the the `run_splinter` function which is then passed through to the
REST API when that is set up.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-21 20:53:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/838" class=".btn">#838</a>
            </td>
            <td>
                <b>
                    BACKPORT: Add loading indicator for Table
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This load can take a few seconds since we are brute force searching for
Org names. This should be optimized eventually.

Signed-off-by: Darian Plumb <dplumb@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-21 20:28:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/837" class=".btn">#837</a>
            </td>
            <td>
                <b>
                    BACKPORT: Remove namespaces from XML parsing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The namespace numbers are not guaranteed for these XML documents, so we
can't have that namespace prefix hardcoded in the parsing functionality.
`fast-xml-parser` has an option to ignore these namespace prefixes. We
do lose the namespace prefixes in the downloaded XML from the table due
to this.

Signed-off-by: Darian Plumb <dplumb@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-21 20:27:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/836" class=".btn">#836</a>
            </td>
            <td>
                <b>
                    Add release notes for Grid 0.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add release notes for the Grid 0.2 release 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-21 19:56:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/835" class=".btn">#835</a>
            </td>
            <td>
                <b>
                    Update CLAP definitions to align with man pages.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Work done involved verifying that the CLAP definitions align with man
pages. The CLAP definitions were already aligned, but the `--key` option
required updating throughout all of main.rs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-20 18:24:07 +0000 UTC
    </div>
</div>

