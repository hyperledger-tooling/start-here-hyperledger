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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/348" class=".btn">#348</a>
            </td>
            <td>
                <b>
                    More functions to simplify wawaka contract development
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                Two new classes of functions for the Wawaka common library:
 - Secrets -- simplify (and standardize) generating messages that can be shared between contracts; a message is encrypted with the contracts encryption key.
- Attestation -- wrappers for the sgx report verification and processing functions
    
Add library of common wawaka contract methods.
    
There are several methods that are common to many contracts. This update provides a base implementation for those methods in order to simplify contract development.

Add common contracts methods for attestations.  Provides a wrapper for managing attested contract endpoints. Contract object provides an attestation package that is verified registering the encryption & verification keys for the contract. Useful for building contracts that share secrets.

Update attestation test to use the new helpers. Replace the code in the attestation test with calls packaged in the attestation common contract code. Complete the implementation of the send/recv secret. Complete testing of the new methods.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-11 19:02:00 +0000 UTC
    </div>
</div>

