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
                PR <a href="https://github.com/hyperledger/besu-native/pull/194" class=".btn">#194</a>
            </td>
            <td>
                <b>
                    Rel next 0.9.4 snapshot
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                bump next release version 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-17 17:33:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-native/pull/193" class=".btn">#193</a>
            </td>
            <td>
                <b>
                    release 0.9.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                release 0.9.3 
* remove long-deprecated altbn128 [#192](https://github.com/hyperledger/besu-native/pull/192)
* fix eip-196 point padding in gnark-crypto [#191](https://github.com/hyperledger/besu-native/pull/191)


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-17 17:32:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-native/pull/192" class=".btn">#192</a>
            </td>
            <td>
                <b>
                    remove long-deprecated altbn128 library
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The altbn128 library has been superseded by matterlabs for EIP-196 for years, and has been unused by besu since 2020

Now that matter-labs library is slated to be removed in favor of gnark-crypto and/or constantine implementations, it seems well overdue to remove this library from besu-native

* remove from gh workflows
* remove from build.sh
* remove from settings.gradle
* remove altbn128 directory altogether
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-16 19:53:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-native/pull/191" class=".btn">#191</a>
            </td>
            <td>
                <b>
                    Right pad incomplete point inputs for eip-196
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In the gnark-crypto implementation of eip-196, incomplete scalar inputs are already right padded with zero.  However,  points also require this treatment.

* in g1Add, right pad p0 and p1 points with zero if they are not the full 32 bytes
* in g1Mul, right pad p0 point if it is not 32 bytes and check to see if the resulting point is in the field before returning 0


from eip-196 [spec](https://eips.ethereum.org/EIPS/eip-196):
```
For both precompiled contracts, if the input is shorter than expected, it is assumed to be virtually padded with zeros at the end (i.e. compatible with the semantics of the CALLDATALOAD opcode). If the input is longer than expected, surplus bytes at the end are ignored.
```


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-16 19:21:17 +0000 UTC
    </div>
</div>

