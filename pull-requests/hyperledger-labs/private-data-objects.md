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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/329" class=".btn">#329</a>
            </td>
            <td>
                <b>
                    Enable contract to contract attestation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                This is a very large modification. We could break it into smaller pieces though all the pieces must be in place before the functionality is effective. The following changes are included:

- several small functional changes to the Wawaka interpreter to simplify access to cryptographic and key/value routines
- some improvements to the way CCF submitter caches connections to enable multi-ledger access
- split the contract update and initialize operations (previously these were separated by a "verb" field, they are now separate code paths with some common functions), this includes changes in the enclave service, the python clients, and both the CCF and Sawtooth ledger components
- change the way the code hash is computed so that the nonce can be used to verify the actual source hash
- add verifiable signing and encryption keys that can be used to create verifiable and secure communication with the contract
- add a ledger command to the pdo-shell to retrieve the attestation of code and contract keys
- a test suite that demonstrates how contract-to-contract attestation can be implemented
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-25 13:47:35 +0000 UTC
    </div>
</div>

