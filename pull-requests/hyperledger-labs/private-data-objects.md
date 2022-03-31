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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/367" class=".btn">#367</a>
            </td>
            <td>
                <b>
                    Blockstore and configuration updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                PR includes two commits. 

The first makes the configuration globally accessible. A PDO client builds the configuration from files & command line switches and then pushes it into the global configuration. Services like the block store, file lookup, and replication manager can use it. Several strange defaults have been replaced with references to the global configuration.

The second commit moves the block store manager out of the storage service so that it can be used more generally. Specifically, the file system-based cache used by the client has been replaced with a cache based on the block store manager. This should simplify the process of managing the cache *as a cache*. Replaced several constants (that were overriding configuration file settings) with calls to the configuration manager. Generalized the block store to block store synchronization to make it easier to move blocks between various servers (may want to look at simplifying the replication service with this). The local block store cache will also simplify development of the client-side kv store management.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-31 16:52:12 +0000 UTC
    </div>
</div>

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
6. it makes the default curve programmable at compile time

Usage changes:
- the default usage/API does not change, and secp256k1 is used
- there is new constructor in the sig-keys, which accepts the curve type as input. For the private key, this is useful to generate curve-specific keys. For the public key, this is useful for the `SerializeXYToHex`/`DeserializeXYToHex` functions.

Test results using secp384r1 as the default curve:
- the sawtooth-based test fails as expected, because the transaction processors tries to verify the contract registration signature using secp256k1
- the CCF-based test succeeds, as both CCF and PDO can recognize the curve from the PEM encoded key and verify signatures accordingly.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-27 20:17:35 +0000 UTC
    </div>
</div>

