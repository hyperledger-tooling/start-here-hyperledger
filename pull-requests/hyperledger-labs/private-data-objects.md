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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/456" class=".btn">#456</a>
            </td>
            <td>
                <b>
                    Basic support for numeric keys 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                New stuff:
* support for the numeric format for ecdsa keys (constructors)
* first start at a test harness for crypto tests, greatly expanded suite of tests for ecdsa keys

Clean up:
* "modernizing" the error handling in the ECDSA key classes
* canonicalizing all of the types for handling smart pointers with openssl
* consolidation of (a lot of) redundant code in the ecdsa key classes
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-23 00:33:46 +0000 UTC
    </div>
</div>

