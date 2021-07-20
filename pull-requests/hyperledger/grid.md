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
                PR <a href="https://github.com/hyperledger/grid/pull/834" class=".btn">#834</a>
            </td>
            <td>
                <b>
                    Reqwest Client SDK Move wip - do not merge
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
        Created At 2021-07-19 20:13:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/833" class=".btn">#833</a>
            </td>
            <td>
                <b>
                    Remove namespaces from XML parsing
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
        Created At 2021-07-19 19:57:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/832" class=".btn">#832</a>
            </td>
            <td>
                <b>
                    Add Product table loading indicator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add a loading indicator on the products table. This load can take a few seconds since we are brute force searching for Org names. This should be optimized eventually, but either way we should add an indicator when we are loading data.

Signed-off-by: Darian Plumb <dplumb@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-19 19:53:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/831" class=".btn">#831</a>
            </td>
            <td>
                <b>
                    BACKPORT: Fix agent-role update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport to 0.2

This fixes an issue with updating a role that belongs to an agent. The
pike_agent_role_assoc table was not updating correctly when roles that
already belonged to an agent were updated.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-16 20:25:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/830" class=".btn">#830</a>
            </td>
            <td>
                <b>
                    BACKPORT: Update Sawtooth dockerfile for grid_pike
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                backport to 0.2

This updates the `pike-contract-builder` for the Sawtooth example
Docker-compose file to account for the name change from `pike` to
`grid-pike`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-16 20:22:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/829" class=".btn">#829</a>
            </td>
            <td>
                <b>
                    Fix agent-role update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes an issue with updating a role that belongs to an agent. The
pike_agent_role_assoc table was not updating correctly when roles that
already belonged to an agent were updated.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-16 17:21:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/828" class=".btn">#828</a>
            </td>
            <td>
                <b>
                    Update Sawtooth dockerfile for grid_pike
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updates the `pike-contract-builder` for the Sawtooth example
Docker-compose file to account for the name change from `pike` to
`grid-pike`.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-15 20:39:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/827" class=".btn">#827</a>
            </td>
            <td>
                <b>
                    Remove un-imported memory module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change removes the `memory` module from the SchemaStore. This
module was previously meant to be removed, but the only item removed was
the corresponding import statement in the SchemaStore's mod.rs file.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-15 19:04:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/826" class=".btn">#826</a>
            </td>
            <td>
                <b>
                    Revert "Merge pull request #820 from Cargill/dnewh-batches-accessors"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This reverts commit 01ca80c250bf94aab817d9ea11ca26e7a9c192aa, reversing
changes made to f24bb577d23bae563ff1c7daf2f3222d20e078d4.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 19:49:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/825" class=".btn">#825</a>
            </td>
            <td>
                <b>
                    Move Grid features to default in CLI and gridd
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In the CLI and gridd we want the default experience to include all Grid business functionality. This set of commits moves pike, product, schema, and location to default for these two components.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 17:45:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/824" class=".btn">#824</a>
            </td>
            <td>
                <b>
                    Stabilize scabbard-event-restart
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change stabilizes the feature "scabbard-event-restart" by removing the feature.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 17:01:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/823" class=".btn">#823</a>
            </td>
            <td>
                <b>
                    Change location family name and version to constants in CLI
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
        Created At 2021-07-13 20:21:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/822" class=".btn">#822</a>
            </td>
            <td>
                <b>
                    Small Pike CLI fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A few small fixes for stabilization
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-13 19:24:05 +0000 UTC
    </div>
</div>

