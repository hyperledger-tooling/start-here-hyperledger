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
                PR <a href="https://github.com/hyperledger/grid/pull/797" class=".btn">#797</a>
            </td>
            <td>
                <b>
                    Fix various small issues in Pike CLI
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
        Created At 2021-07-02 20:41:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/796" class=".btn">#796</a>
            </td>
            <td>
                <b>
                    Fix Rest API error message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes an error message produced when the Grid daemon verifies the `service_id`. The `service_id` should be present if Grid is running on Splinter and should not be present if Grid is running on Sawtooth. The error message fixed in this PR is produced if the service id is present while on sawtooth and the other instance when it is not present on splinter. In each case, the errors produced stated that the `Circuit ID` was/was not present. However, this message should state `Service ID` as this is actually the value being checked.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-02 15:32:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/795" class=".btn">#795</a>
            </td>
            <td>
                <b>
                    Add grid organization `list` and `show` commands 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change adds commands to list organizations and to show a specific organization based on the `org_id`. This also adds the man page entries for each of these commands.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-02 14:50:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/794" class=".btn">#794</a>
            </td>
            <td>
                <b>
                    Fix line wrapping in display_role()
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
        Created At 2021-07-01 18:01:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/793" class=".btn">#793</a>
            </td>
            <td>
                <b>
                    Fix rest API URL handling in `run` methods
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change creates an `Endpoint` object from the `GridConfig`'s
`endpoint` immediately as it is passed into the daemon's `run` methods
for Splinter and Sawtooth backends. This allows for the backend rest
API URL to be correctly formatted as it is returned by the
config object with a `splinter:` or `sawtooth:` prefix to allow the
daemon to start correctly. This fixes the issue where the `splinter:`
and `sawtooth:` prefixes are being passed in with the URL, returning
an error as this creates an invalid URL scheme.

Signed-off-by: Shannyn Telander <telander@bitwise.io>

To test: run `docker-compose -f examples/splinter/docker-compose.yaml up` and ensure that the logs start as normal 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-30 19:16:07 +0000 UTC
    </div>
</div>

