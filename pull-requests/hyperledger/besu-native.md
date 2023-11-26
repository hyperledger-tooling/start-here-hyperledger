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
- commit: expects up to 256 BE 32byte Fr values, returns Commitment serialized to Fp.
- updateCommitment: expects Commitment, diff value, and index, returns Commitment serialized to Fp
- groupToField: expects Commitment serialized to Fp, returns Fr

Everything expects BE bytes, and returns BE bytes.


I still think Java is working on BE bytes by default. Please re-run `TestPedersenCommitment` and put a breakpoint. Example and screenshot:


![995CEEBE-40F4-4DAD-B511-8706FA202285](https://github.com/hyperledger/besu-native/assets/22306045/9047c503-3330-4b06-9f72-125ca3309531)

so [28, -127, 74 ....

is 1c,81,4a in hex




Only thing that is working on LE is "serialize" call from arkworks

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-24 12:29:43 +0000 UTC
    </div>
</div>

