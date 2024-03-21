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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/480" class=".btn">#480</a>
            </td>
            <td>
                <b>
                    Make SGX registration a bit more robust
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Handle missing SGX verification status CONFIGURATION_AND_SW_HARDENING_NEEDED
* Honor PDO_LOG_LEVEL in registration script

Note this is tested on top if (2024-03-15) version of PR #477, so for now still "inherits" also Bruno's commit from that PR.  Once PR#477 is closed i will rebase this one and  "undraft" it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-15 18:00:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/478" class=".btn">#478</a>
            </td>
            <td>
                <b>
                    Provide PDO_SOURCE_ROOT default for docker to allow zero-config build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Minor change to allow docker builds out-of-the-box without any configuration/environment variable definition.  This default for PDO_SOURCE_ROOT also hides an error for undefined `PDO_SOURCE_ROOT` which is _very_ unintuitive to figure out if you haven't run into this issue beforehand.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-15 01:42:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/477" class=".btn">#477</a>
            </td>
            <td>
                <b>
                    Fixes for making PDO work in SGX HW-mode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR continues the work in #463 to enable tests in SGX HW-mode, and makes the following contributions.

1. this PR adds targets to the docker makefile to enable sgx builds and tests.
2. the enclave code signing key is passed from the host to the docker container (if one exists)
3. it adds the necessary volumes and devices for sgx tests in docker compose
4. it assigns a location for sgx collateral in a container (different from the xfer folder)
5. at runtime, it copies the sgx collateral from the xfer folder to the location assigned within the container _before_ services are configured (because configuration requires the sgx collateral)



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-14 19:58:59 +0000 UTC
    </div>
</div>

