---
layout: default
title: weaver-dlt-interoperability
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/weaver-dlt-interoperability
---

# weaver-dlt-interoperability <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/weaver-dlt-interoperability){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/95" class=".btn">#95</a>
            </td>
            <td>
                <b>
                    Return Signatures along with payload from corda-interop-app
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Now `GetExternalStateByLinearId` returns a JSON String, with proof consisting of list of signatures along with payload.
2. Modified client app, to read the new return object from `GetExternalStateByLinearId`.

This feature addition was a requirement from Marcopolo demo.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-29 10:03:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/89" class=".btn">#89</a>
            </td>
            <td>
                <b>
                    interop-cc chaincode changes pertaining to locking mechanism reorganization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR addresses the below:
- Reorganize the interop-cc, base-class and base-class-contract pertaining to locking mechanism
- Add the code to support ECDLP lock along with HashLock
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-24 17:29:39 +0000 UTC
    </div>
</div>

