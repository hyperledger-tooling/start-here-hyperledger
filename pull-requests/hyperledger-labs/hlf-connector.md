---
layout: default
title: hlf-connector
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/hlf-connector
---

# hlf-connector <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/hlf-connector){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/hlf-connector/pull/70" class=".btn">#70</a>
            </td>
            <td>
                <b>
                    Increment version after release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">auto-version-increment</span>
            </td>
            <td>
                Automated changes by [create-pull-request](https://github.com/peter-evans/create-pull-request) GitHub action
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-10 13:09:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/hlf-connector/pull/69" class=".btn">#69</a>
            </td>
            <td>
                <b>
                    Fix broken Event-Publisher flow caused by java version upgrade
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR contains the changes to revert Java version upgrade which is potentially blocking the Chaincode Event publisher flow. 
Upgrade from 8 to 11 will be performed after verifying that no other dependencies of HLF connector has a strict dependency on version 8 or is incompatible with version 11.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-10 12:48:28 +0000 UTC
    </div>
</div>

