---
layout: default
title: indy-node
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-node
---

# indy-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-node/pull/1794" class=".btn">#1794</a>
            </td>
            <td>
                <b>
                    Fix dependency scheme
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - A fix for the dependency scheme related to indy-plenum.  Fixes the issue where the python package version installed using the deb package is different than the published python package.

- The issue was due to how the dependency options of `fpm` were being used.  The deb package build was using the python dependencies to define the deb package dependencies.  Since the deb and python package version numbers use slightly different formats for non-release (`dev` and `rc`) versions, the versions of the python dependencies (notably indy-plenum) were being set to match the deb version format in order to correctly define the deb dependencies.  This strategy has the unfortunate side affect of causing dependency issues with the python packages down the road.

Signed-off-by: Wade Barnes <wade@neoterictech.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-19 13:09:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-node/pull/1793" class=".btn">#1793</a>
            </td>
            <td>
                <b>
                    fixed correct checkout version & tags fetch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Following fix made here; https://github.com/sovrin-foundation/sovrin/pull/315

Signed-off-by: Wade Barnes <wade@neoterictech.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-13 19:14:06 +0000 UTC
    </div>
</div>

