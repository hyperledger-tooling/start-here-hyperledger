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
                PR <a href="https://github.com/hyperledger/besu-native/pull/105" class=".btn">#105</a>
            </td>
            <td>
                <b>
                    Simple implementation of mimc, light-tested
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Add an implementation of MiMC on the bn254 scalar field in rust.

/// MIMC7 is a hash function suited for BN256's scalar field.
///
/// It has modulus
/// p = 21888242871839275222246405745257275088548364400416034343698204186575808495617
///
/// The MIMC paper (https://eprint.iacr.org/2016/492.pdf) states that monomial x^d is a permutation
/// in Fp if gcd(d,p) == 1
///
/// Exponent for MIMC7 is 5, which satisfies the above condition.
/// MIMC can't be implemented generically as different
/// prime fields will require different MIMC implementations.
///
/// ```code
/// pseudo code:
fn mimc5_permutation(constants, x, k):
    h := x;
    for i = 0..constants.len() {
        h := h + k + constants[i]
        h := h^5;
    }
    h = h + k;
    return h;

## Interface

```rust
pub fn mimc_hash<T : AsRef<[u8]>>(bytes: T) -> Vec<u8>;
```
The implementation targets full consistency with the present implementation:



## Consistency testing with gnark's implementation

gnark and the present implementation are tested to give the same result for the strings.

* `0x0000000000000000000000000000000000000000000000000000000000000000`
* `0x0000000000000000000000000000000000000000000000000000000000000001`
* `0x0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000100000000000000000000000000000000000000000000000000000000000000020000000000000000000000000000000000000000000000000000000000000003000000000000000000000000000000000000000000000000000000000000000400000000000000000000000000000000000000000000000000000000000000050000000000000000000000000000000000000000000000000000000000000006000000000000000000000000000000000000000000000000000000000000000700000000000000000000000000000000000000000000000000000000000000080000000000000000000000000000000000000000000000000000000000000009000000000000000000000000000000000000000000000000000000000000000a000000000000000000000000000000000000000000000000000000000000000b000000000000000000000000000000000000000000000000000000000000000c000000000000000000000000000000000000000000000000000000000000000d000000000000000000000000000000000000000000000000000000000000000e000000000000000000000000000000000000000000000000000000000000000f`

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-28 14:35:07 +0000 UTC
    </div>
</div>

