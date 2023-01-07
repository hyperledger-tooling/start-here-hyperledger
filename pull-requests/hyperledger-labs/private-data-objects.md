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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/390" class=".btn">#390</a>
            </td>
            <td>
                <b>
                    Various updates to make multi-user contracts work
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                This PR includes a number of fixes that make it easier for users on different clients to share access to contracts. 

First, it introduces the configuration of a persistent storage service that is identified in the extra data (this is a hint, not a guarantee) in the contract file. The persistent storage service is a service where the current state of the contract is likely to exist (and persistent indefinitely).

Second, to allow storage services that are not associated with an eservice (e.g. to make a persistent storage service that has a policy for maintaining state that is not the same as the short term caches generally used by the storage services attached to an eservice), make the replication manager work with storage services NOT eservices. 

Third, since we long ago removed the need for uploading contract code on every transaction (since the code is stored in the contract state), the code is removed from the contract save file. This makes the save files a LOT smaller (especially with wawaka code) and reasonable to package in an email & send to someone. The contract code hash is included to verify that the code used matches the code expected. 

Finally, the PDO documentation is lacking. This PR will not fix that. However, some additional documentation was added to help interpret the process for building wawaka contracts. This is a start, not the end.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-06 19:21:58 +0000 UTC
    </div>
</div>

