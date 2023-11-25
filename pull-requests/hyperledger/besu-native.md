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
                PR <a href="https://github.com/hyperledger/besu-native/pull/127" class=".btn">#127</a>
            </td>
            <td>
                <b>
                    add update commitment to ipa_multipoint JNI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Changing out ipa_multipoint API to these functions:

- pedersenHash: same as before (not changed)
- commit: expects up to 256 LE 32byte Fr values, returns Commitment serialized to Fp.
- groupToField: expects Commitment serialized to Fp, returns Fr
- updateCommitment: expects Commitment, diff value, and index, returns Commitment serialized to Fp

Everything expects LE bytes, and returns LE bytes. There is a lot of overhead with reversing bytes, for that I think we can simply fork banderwagon lib and make some changes on specialized "besu" branch.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-24 12:29:43 +0000 UTC
    </div>
</div>

