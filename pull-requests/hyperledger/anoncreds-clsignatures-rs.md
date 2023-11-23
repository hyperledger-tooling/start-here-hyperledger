---
layout: default
title: anoncreds-clsignatures-rs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/anoncreds-clsignatures-rs
---

# anoncreds-clsignatures-rs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/anoncreds-clsignatures-rs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-clsignatures-rs/pull/33" class=".btn">#33</a>
            </td>
            <td>
                <b>
                    Conditional serialization for crypto primitives (string or bytes)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Make conditional serialization for crypto primitives:
*  For JOSN serialization, crypto primitives such BugNumber's, Points, etc. are represented as string.
*  For message pack or cbor these crypto primitives represented as bytes.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-22 06:55:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-clsignatures-rs/pull/32" class=".btn">#32</a>
            </td>
            <td>
                <b>
                    Add check to generation of s in issuer public key
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The implementation uses the method described in p24 of [this CL paper](https://eprint.iacr.org/2010/496.pdf#page=24) when generating the issuer public key, which involves sampling a random quadratic residue S and from that computing random powers to generate additional residues.  However, as stipulated in the paper, this method only works if S is a generator of the group of invertible quadratic residues mod n. This can be checked by verifying that it has order equal to the product of the Sophie-Germain primes p' and q' used to construct the safe RSA modulus n, but this check is not done  in the implementation.

Since p' and q' are coprime and are primes, every invertible quadratic residue has order 1, p', q' or p'\*q'.  It therefore suffices to check that S is not 1, that S^p' is not 1 mod n, and S^q' is not 1 mod n.

Added this check in a separate PR from my other one but both need to be integrated - hope it makes sense!
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-17 11:57:47 +0000 UTC
    </div>
</div>

