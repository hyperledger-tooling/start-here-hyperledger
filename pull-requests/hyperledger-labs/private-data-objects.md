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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/482" class=".btn">#482</a>
            </td>
            <td>
                <b>
                    Fix several bugs in the service data routines for verification
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                Small changes to fix several problems with the way last_verified_time is handled in the service data store. Improves variable naming and ensures that the value of last_verified_time is pushed through. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-26 14:32:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/481" class=".btn">#481</a>
            </td>
            <td>
                <b>
                    Transition service groups to a persistent data store (comparable to the service endpoints store)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">client</span>
            </td>
            <td>
                Service group files loaded on demand has been one of the more painful complexities for running contracts. This commit introduces a persistent database comparable to the database used to store service   endpoints. The new groups database is stored at the location specified in the ['Service', 'GroupDatabaseFile'] configuration entry.
    
The service groups commands were all updated to accommodate the new style. These are SIGNIFICANT changes. To ensure that correctness has not been compromised, a new test was added for storage groups.
    
Finally, the persistent database required updating several other tests.  This change is, for the moment, a "functionally correct" change to the tests (meaning that all tests now use the correct service groups commands) but there is significant room for cleaning up the process.

Note that this will require changes to the test scripts for PDO contracts (and the notebooks that set up the service groups). The correct approach would be (for tests) to invoke the site-configuration.psh script in place of the create-service-groups script. And a future jupyter notebook will create an interface for managing the database more explicitly.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-21 16:17:42 +0000 UTC
    </div>
</div>

