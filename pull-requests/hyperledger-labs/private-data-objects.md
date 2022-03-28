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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/366" class=".btn">#366</a>
            </td>
            <td>
                <b>
                    Upgrade crypto lib to support secp256k1 and secp384r1 at runtime 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR makes the following contributions:
1. it generalizes the PDO crypto lib signing scheme to support the secp256k1 and secp384r1 ECDSA curves at runtime. A curve can be selected directly through the constructor objects, or it is recognized when a key is deserialized. The mechanism can be extended.
2. it adds tests to test the crypto lib with each curve -- in addition to the original default tests which use secp256k1
3. it consolidates common parts of the public and private key objects in an abstract class.
4. it fixes the max signature size issue -- the value was fixed to the secp256k1 max sig size constant -- by removing the constants and making the calculation dependent on the keys (or better, curves) actually used.
5. it adds tests for testing the python wrapper with the two curves.

Usage changes:
- the default usage/API does not change, and secp256k1 is used
- there is new constructor in the sig-keys, which accepts the curve type as input. For the private key, this is useful to generate curve-specific keys. For the public key, this is useful for the `SerializeXYToHex`/`DeserializeXYToHex` functions.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-27 20:17:35 +0000 UTC
    </div>
</div>

