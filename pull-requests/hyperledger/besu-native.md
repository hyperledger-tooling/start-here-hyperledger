---
layout: default
title: besu-native
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu-native
---

# besu-native <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu-native){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-native/pull/132" class=".btn">#132</a>
            </td>
            <td>
                <b>
                    Add support for MiMC on BLS12-377's scalar field
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Description

The current PR adds supports for the MiMC hash function, but on the BLS12-377 scalar's field (not to be confused with BLS12-381). The implementation is - as for its BN254 counterpart - imported from gnark's. The PR keeps support for the BN254's implementation which is used by Shomei as of now. The implementation 

In more details:

- Renames `computeMiMC` to `computeMiMC254` to make the naming more specific. This can be reverted if deemed useful during the review as this introduces a breaking change.
- Extends the LibGnark class to also provide `computeMiMCBls12377`
- Adds test-cases on the Java side to check the hashes are consistent with what we get on go. The test-vectors used for the testing are the same as the one used for the Bn254 counterpart.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-03 23:25:49 +0000 UTC
    </div>
</div>

