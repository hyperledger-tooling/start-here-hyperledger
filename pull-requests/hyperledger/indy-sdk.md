---
layout: default
title: indy-sdk
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-sdk
---

# indy-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2477" class=".btn">#2477</a>
            </td>
            <td>
                <b>
                    Remove the blocking input in the CD pipeline.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Remove the blocking input before the Cargo publish step.
- This is causing too many build resources issues to leave in place.
- Removing without adding the check and retry logic to see if and how much of an issue this still is.
- Related issue references:
  - https://github.com/hyperledger/indy-sdk/issues/2309
  - https://github.com/hyperledger/indy-sdk/issues/2395

Signed-off-by: Wade Barnes <wade@neoterictech.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-03 16:04:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2475" class=".btn">#2475</a>
            </td>
            <td>
                <b>
                    Update the version of Rust used in the workflows.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Wade Barnes <wade@neoterictech.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 18:36:09 +0000 UTC
    </div>
</div>

