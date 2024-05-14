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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/490" class=".btn">#490</a>
            </td>
            <td>
                <b>
                    Improvements to SGX attestation verification
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds checks to the attestation verification procedures, as discussed in #195 .
The additions/modifications are as follows:

- it makes the sgx debug flag dependent on the PDO_DEBUG_BUILD environment variable. In the cmake file for building the enclave, it use CMAKE_BUILD_TYPE (debug/release) to ensure the the NDEBUG variable is set appropriately. In the swig wrapper, it defines the EDEBUG variable (as defined and used in the SGX SDK) to ensure that the the SDK sets the SGX_DEBUG_FLAG correctly when creating the enclave.

- it adds a script to generate the xml configuration file for the enclave. This is necessary to set the DisableDebug field appropriately. The xml file is generated in the build folder since it is a build artifact.

- it updates the enclave registration policy and the transaction processor. The policy now contains the sgx_debug_flag. So now we totally have 3 modes of operation: sim mode (no policy checks), hw mode with enclave debug disabled, hw mode with enclave debug enabled. The TP will enforce the flag check accordingly when it receives enclave registrations. Additionally, it will also check that the enclave runs in 64-bit mode.

- it updates the pservice with additional attestation checks before provisioning an enclave. To do this, it extends the metadata header built by the eservice to provide info about the enclave to the pservice. Originally, it contained only mrenclave; now it contains the enclave attributes and relative mask. The pservice always checks the 64-bit flag. Also, it checks the debug flag in the attributes  _only if_ this is set in the mask -- if set in the mask, it must be enforced. (Note: the mask is derived from how the [SDK manages the DisableDebug field](https://github.com/intel/linux-sgx/blob/80a6625c497056c43e78d993e414ca99a9efed5c/sdk/sign_tool/SignTool/manage_metadata.cpp#L294) in the configuration file; if 1, it forces the debug flag to 0; if 0, it considers the debug flag irrelevant, and the untrusted host which runs the enclave can set it arbitrarily; in this last case, the debug flag is still verifiable through the attestation, and its value may differ compared to the one appearing in the signed enclave metadata).



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-13 20:22:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/489" class=".btn">#489</a>
            </td>
            <td>
                <b>
                    Move to standard tools for in-memory contract object cache
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Transition from very simple cache for contract objects to a more standard cache implementation from cachetools. The transition enables both more functionality (explicit client control of when the cache is flushed) and better behavior (automatic flushing of older contract objects).

Several other clean ups of imports and other unused variables.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-08 22:24:41 +0000 UTC
    </div>
</div>

