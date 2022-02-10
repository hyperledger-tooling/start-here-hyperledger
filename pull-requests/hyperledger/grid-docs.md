---
layout: default
title: grid-docs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/grid-docs
---

# grid-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/grid-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid-docs/pull/312" class=".btn">#312</a>
            </td>
            <td>
                <b>
                    Update schemaspy java dependency version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The dep version was updated in response to a log4j vulnerability.
https://github.com/schemaspy/schemaspy/issues/819

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 22:08:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid-docs/pull/311" class=".btn">#311</a>
            </td>
            <td>
                <b>
                    Fix API doc path for building website
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change fixes the file path used to locate the API docs when
building the site. This change removes the `references` level in the
path.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 21:28:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid-docs/pull/304" class=".btn">#304</a>
            </td>
            <td>
                <b>
                    Fix left sidebar for 0-4 docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change updates the left sidebar for the 0-4 section of the docs to
correctly show v0.3 as the "Latest" release and "Stable", rather than
"In Development".

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-07 15:01:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid-docs/pull/303" class=".btn">#303</a>
            </td>
            <td>
                <b>
                    Add API and DB schema docs for 0-4
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
        Created At 2022-02-04 22:32:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid-docs/pull/302" class=".btn">#302</a>
            </td>
            <td>
                <b>
                    Update Upgrading Smart Contracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds a warning for users to save their keys before rebuilding the
daemons. Also fixes a typo.

Signed-off-by: Chris Eckhardt <eckhardt@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-03 20:05:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid-docs/pull/301" class=".btn">#301</a>
            </td>
            <td>
                <b>
                    Update Creating Schemas
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Corrects section on updating schemas, fixes minor issues in text,
and adds the schema update permission to the Using Pike page.
Updates 0.3, 0.4, and 0.2.

Signed-off-by: Chris Eckhardt <eckhardt@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-03 18:00:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid-docs/pull/300" class=".btn">#300</a>
            </td>
            <td>
                <b>
                    Update `grid keygen` man page
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds the KEY_NAME argument to the grid keygen man page.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-03 16:59:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid-docs/pull/299" class=".btn">#299</a>
            </td>
            <td>
                <b>
                    Fix permissions for using Grid Location
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change fixes the line in the `Creating Locations` guide used to
create the role with permissions to create, update, and delete a
location. Previously, the list of permissions was broken up by a `\` to
allow it to span multiple lines. However, this was creating a space in
the `location::can-delete-location` permission that disabled Grid from
being able to recognize this permission. This change removes the back
slash and keeps the permissions on one line, which still allows for
linting to pass and does not cause a space to occur in the permissions
string.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-03 16:53:37 +0000 UTC
    </div>
</div>

