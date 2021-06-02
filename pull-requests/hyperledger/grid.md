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
                PR <a href="https://github.com/hyperledger/grid/pull/728" class=".btn">#728</a>
            </td>
            <td>
                <b>
                    Remove "pub use" and make all diesel modules pub(crate)
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
        Created At 2021-05-28 22:03:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/727" class=".btn">#727</a>
            </td>
            <td>
                <b>
                    Rename a few sdk modules to their singular form
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Renames products, locations, schemas to product, location, schema.

This is not intended to have any functional changes.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-28 19:10:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/726" class=".btn">#726</a>
            </td>
            <td>
                <b>
                    Add feature guards for each REST API endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds several features which guard the REST API endpoint; this
will allow the daemon processes to individually pull in the specific
endpoints supported. It also allows enabling the underlying features
without enabling the associated endpoints.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 21:05:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/725" class=".btn">#725</a>
            </td>
            <td>
                <b>
                    Add "backend" as dependency for "rest-api-actix-web-3"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This was an error in the dependency list for rest-api-actix-web-3 and
isn't intended to be a functional change (other than fixing compilation
if specifying this feature in isolation).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 21:05:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/724" class=".btn">#724</a>
            </td>
            <td>
                <b>
                    Remove newline from error in cli/action/product.rs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also wrap ling at 100 characters.

Signed-off-by: Andrea Gunderson <agunde@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 19:56:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/723" class=".btn">#723</a>
            </td>
            <td>
                <b>
                    Small cleanups for the grid daemon
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
        Created At 2021-05-27 19:34:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/722" class=".btn">#722</a>
            </td>
            <td>
                <b>
                    Update copyright headers in `splinter` module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change updates the copyright headers of files in the `splinter`
module to reflect the current year.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 19:34:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/719" class=".btn">#719</a>
            </td>
            <td>
                <b>
                    Remove sqlite and postgres from rest api feature
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This removes sqlite and postgres from the sdk's rest-api-actix-web-3
feature, which will make it possible to conditionally use the sqlite or
postgresql when using the rest api.

This commit makes BatchList pub, because without pub, it would be
necessary to put a conditional of the underlying implementations being
enabled; it seems cleaner to simply make it pub since it does not seem
intentional to prevent creation of BatchList (which itself is pub).

Features are added to griddle for sqlite/postgres to pull in the
associated sdk features.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 15:01:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/718" class=".btn">#718</a>
            </td>
            <td>
                <b>
                    Rename batch submitter to backend client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The trait formerly known as "BatchSubmitter" was really a client to the backend (Sawtooth or Splinter). This gives it distinction from other batch-related functionality within the sdk and daemon.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-26 21:48:30 +0000 UTC
    </div>
</div>

