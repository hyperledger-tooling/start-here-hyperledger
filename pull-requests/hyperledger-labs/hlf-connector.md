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
                PR <a href="https://github.com/hyperledger-labs/hlf-connector/pull/98" class=".btn">#98</a>
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
        Created At 2023-06-23 04:38:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/hlf-connector/pull/97" class=".btn">#97</a>
            </td>
            <td>
                <b>
                    Use Framework provided html escape utility over third party libraries
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This changeset contains few minor refactorings like fixing code comments and using Framework provided HTML escape utility instead of using a third party library.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-23 04:27:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/hlf-connector/pull/96" class=".btn">#96</a>
            </td>
            <td>
                <b>
                    Fix duplicate Chaincode-Events from being pushed to subscription topic.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The `registerChaincodeEventListener()` on the Channel object provided by the Fabric Java SDK comes with a disclaimer of generating duplicate and out-of-order Events.

This PR contains the changeset to use `addContractListener()` on `Contract` object for registering Event listeners, which gurantees unique and ordered Events.

https://hyperledger.github.io/fabric-gateway-java/release-2.2/org/hyperledger/fabric/gateway/Contract.html
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-22 16:31:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/hlf-connector/pull/95" class=".btn">#95</a>
            </td>
            <td>
                <b>
                    Add XSS protection in Header config and minor refactorings
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
        Created At 2023-06-20 13:03:08 +0000 UTC
    </div>
</div>

