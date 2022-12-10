---
layout: default
title: private-data-objects
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/private-data-objects
---

# private-data-objects <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/private-data-objects){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/386" class=".btn">#386</a>
            </td>
            <td>
                <b>
                    Change the python version regular expression for multi-digit versions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                This is preliminary support for clients running on ubuntu 22.04 where the python version is 3.10. Previously the regular expression used to get the version was limited to one digit minor versions. This should fix that limitation.

Note that shell scripts can use the check_python_version macro defined in the common.sh library.

Signed-off-by: Mic Bowman <mic.bowman@intel.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-06 00:51:56 +0000 UTC
    </div>
</div>

