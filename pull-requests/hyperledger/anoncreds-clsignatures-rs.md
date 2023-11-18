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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-clsignatures-rs/pull/31" class=".btn">#31</a>
            </td>
            <td>
                <b>
                    Add checks to quadratic residue sampling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                To sample a quadratic residue mod n uniformly at random, one technique is to sample an integer between 1 and n-1, check that it is invertible, and square it, e.g. see [here](https://www.inf.ufpr.br/murilo/public/IndexingPaper.pdf).

The added code ensures the randomly-sampled element that gets squared is invertible (which also implies it is non-zero, so no need to check it is non-zero separately).

In normal usage of this function for AnonCreds, n = p \* q where p and q are large primes, so the probability that an element is not invertible is only 1 - (p-1)\*(q-1) / (p\*q) = 1/p + 1/q - 1/(p\*q), which means the expectation on the number of iterations of the while loop is very close to 1.

(Now with DCO!)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-15 18:36:41 +0000 UTC
    </div>
</div>

