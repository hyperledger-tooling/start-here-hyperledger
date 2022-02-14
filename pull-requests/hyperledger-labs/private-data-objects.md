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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/359" class=".btn">#359</a>
            </td>
            <td>
                <b>
                    Remove usage of outdated built-in CDI components
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR removes all CDI-related components from the first CDI prototype built directly into PDO, including the embedded compilation report in contracts as well as the policy engine previously built into the eservice.

Note: This PR entirely disables the wawaka-aot build and tests
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 00:52:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/358" class=".btn">#358</a>
            </td>
            <td>
                <b>
                    Remove the redundant WASM_MEM config from github workflows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The common config sets the default memory configuration
so we don't need to set it from here.

Signed-off-by: Mic Bowman <mic.bowman@intel.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-07 19:36:00 +0000 UTC
    </div>
</div>

