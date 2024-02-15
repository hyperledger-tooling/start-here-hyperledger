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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/468" class=".btn">#468</a>
            </td>
            <td>
                <b>
                    Simplify build and install for CCF
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Several changes to improve the performance (and remove dependencies) for CCF startup. Many of the changes are centered in the ccf Makefile to separate the creation of the ccf clients (like the ping test, ledger authority retrieval and policy scripts that might reasonably be executed from anywhere) from the environment needed for a ccf service node (the script to start a ccf network).

The big win from the separation is that we can remove dependency on the sandbox script & pre-install all of the python package dependencies independently from the execution of the ccf nodes. The result is that the ledger containers start in a couple seconds instead of several minutes.

Note that a future PR will package the ccf client scripts separately and install them with other PDO packages so they are available on all PDO installations.

@bvavala your review is requested because the second commit adds the code to copy the member keys into the
ledger key directory. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 23:13:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/467" class=".btn">#467</a>
            </td>
            <td>
                <b>
                    Changes to Fix Ledger APIs used to set Contract Enclave attestation policy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                This is an enabler PR to improve the current implementation of registration of contract enclave attestation policy with the ledger. 

The current `register_enclave_attestation_verification_policy` member API that is used to register attestation policy with ledger is replaced with two member  APIs: `set_contract_enclave_check_attestation_flag` and `set_contract_enclave_expected_sgx_measurements`. 

`set_contract_enclave_check_attestation_flag` is invoked as part of ledger start up, and simply specifies whether attestation check should be enabled or not for contract enclaves. The expectation is to disable the flag for SGX_SIM mode and enable the flag for HW mode. If the flag is enabled, the second API `set_contract_enclave_expected_sgx_measurements` must be subsquently invoked by the member to provide expected values for mrenclave, basename and ias_public_key. 

This PR does not specify when/how the second API gets invoked with HW mode. That will be addressed in a separate PR. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-13 06:08:20 +0000 UTC
    </div>
</div>

