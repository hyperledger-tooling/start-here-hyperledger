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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/494" class=".btn">#494</a>
            </td>
            <td>
                <b>
                    Update memory configurations and simplify specification 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Several changes to make memory allocation cleaner:
    
1) enable build-time configuration of the memory configuration for the eservice enclave (the pservice enclave does not have dynamic memory requirements so they remain fixed).
    
2) a single variable now controls the allocation for enclave and interpreter memory; PDO_MEMORY_CONFIG may be set to SMALL, MEDIUM, or LARGE. this replaces the old WASM_MEM_CONFIG which was used for interpreter memory configuration. The SMALL configuration sets up the enclave and the interpreter for 4MB, MEDIUM is for 8MB and LARGE is for 16MB.
 
3) remove the stack and heap configuration from the contract build scripts; this appears to be unnecessary though further testing is warranted.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-14 21:03:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/493" class=".btn">#493</a>
            </td>
            <td>
                <b>
                    small docker fixes to fix loglevel switch in tools
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                cleaning up a couple small bugs with docker tools
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-12 16:06:54 +0000 UTC
    </div>
</div>

