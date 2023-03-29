---
layout: default
title: sawtooth-core
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/sawtooth-core
---

# sawtooth-core <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/sawtooth-core){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-core/pull/2447" class=".btn">#2447</a>
            </td>
            <td>
                <b>
                    Fix of medium vulnerabilities - Weak Cryptography
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### What was wrong?

When software generates predictable values in a context requiring unpredictability, it may be possible for an attacker to guess the next value that will be generated, and use this guess to impersonate another user or access sensitive information.

### How was it fixed?

I just changed the PRNG lib from random to secrets (OWASP recommendation).

### CWEs:
- [CWE-338](https://cwe.mitre.org/data/definitions/338): Use of Cryptographically Weak Pseudo-Random Number Generator (PRNG);
- [CWE-330](https://cwe.mitre.org/data/definitions/330): Use of Insufficiently Random Values;
- [CWE-326](https://cwe.mitre.org/data/definitions/326): Inadequate Encryption Strength;
- [CWE-1241](https://cwe.mitre.org/data/definitions/1241): Use of Predictable Algorithm in Random Number Generator.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-24 18:36:45 +0000 UTC
    </div>
</div>

