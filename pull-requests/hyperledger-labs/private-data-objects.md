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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/382" class=".btn">#382</a>
            </td>
            <td>
                <b>
                    Enable DCAP quote generation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR enables DCAP quote generation in PDO, alongside EPID quotes.

The PR adds the following features:
*  a new `PDO_ATTESTATION_TYPE` variable to specify the type of attestation. Currently, it supports the following values: `simulated` in SIM mode; `epid-linkable` or `dcap` in HW mode.
* updated docker build to support DCAP quote generation in HW mode
  * updated support for dcap devices and a new file to specify the sgx attestation type (even in SIM mode)
  * a PCCS is required and the build assumes that an instance is up and running. The address can be configured through the `PCCS_HOSTPORT` variable.
* documentation for the dcap attestation and new variables
* support for DCAP quote generation, alongside EPID quote generation, inside the eservice. The attestation type is used to select the quoting enclave target and the right data structures to use. As before, a generic quote buffer is returned to the caller. For EPID, this is sent to IAS to grab the verification report. For DCAP, the proof data is currently dropped because: 1) support for DCAP quote verification must be implemented; 2) this allows to test the rest of PDO (CCF TP and pservice), albeit (with the rest compiled) for SIM mode.

Testing.
* This PR depends on #379 -- which enables HW mode only for the eservice, for testing purposes.
* This PR was tested through:
  * the usual github CI, in SIM mode;
  * locally in HW mode with EPID;
  * locally in HW mode with DCAP, using a local PCCS on the same platform.
    *  Troubleshooting proxy/PCCS issues in CI. Errors in proxy/pccs configuration typically result in `Error returned from the p_sgx_get_quote_config API. 0xe019`.
      * Make sure that the no-/proxy variables are set up correctly on the host (since these are later ported to the containers in the CI) and in the containers.
      * Also, make sure that the `/etc/sgx_default_qcnl.conf` on the host, or in the container, is set up correctly with a reachable PCCS.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-24 22:35:32 +0000 UTC
    </div>
</div>

