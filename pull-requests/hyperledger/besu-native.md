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
                PR <a href="https://github.com/hyperledger/besu-native/pull/135" class=".btn">#135</a>
            </td>
            <td>
                <b>
                    prepare for 0.8.4-SNAPSHOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                bump version and changelog
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-05 01:37:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-native/pull/134" class=".btn">#134</a>
            </td>
            <td>
                <b>
                    release version 0.8.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                release verson 0.8.3 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-05 00:45:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-native/pull/133" class=".btn">#133</a>
            </td>
            <td>
                <b>
                    WIP: Expose verkle prove call
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                WIP exposing prove call.

https://github.com/hyperledger/besu-native/pull/133/files#diff-6c182f542873a0b4e1718eec91be7decc4f4ff80602e2da0c11b9e68e93c55beR196

I would rather first wait for https://github.com/hyperledger/besu-native/pull/127 and test the trie with this crypto API and computing a root commitment before merging the proving/verifying calls, but as requested here's the draft. cc @thomas-quadratic @matkt 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-04 20:48:14 +0000 UTC
    </div>
</div>

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

