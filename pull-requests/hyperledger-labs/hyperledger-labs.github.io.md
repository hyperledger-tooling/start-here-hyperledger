---
layout: default
title: hyperledger-labs.github.io
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/hyperledger-labs.github.io
---

# hyperledger-labs.github.io <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/hyperledger-labs.github.io){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/hyperledger-labs.github.io/pull/255" class=".btn">#255</a>
            </td>
            <td>
                <b>
                    One-Attestation-API Lab Proposal
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This lab proposes to create a single API to handle attestations.
Attestations are a crucial mechanism to establish trust in hardware-based trusted execution environments (TEEs).
Today, multiple attestation mechanisms are available (e.g., SGX-EPID, SGX-DCAP, TDX-DCAP).
This proposal aims to create a single abstraction for the generation and verification of hardware-based attestations.
The abstraction can benefit, and avoid redundant implementations in, multiple projects (e.g., Fabric Private Chaincode, Private Data Objects)
that use TEEs to enhance software integrity and confidentiality.

--

@mbrandenburger Please acknowledge sponsorship.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-11 18:50:59 +0000 UTC
    </div>
</div>

