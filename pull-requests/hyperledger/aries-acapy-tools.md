---
layout: default
title: aries-acapy-tools
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-acapy-tools
---

# aries-acapy-tools <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-acapy-tools){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-tools/pull/13" class=".btn">#13</a>
            </td>
            <td>
                <b>
                    Renames repo to aries-acapy-tools
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Addresses issue #11
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-03 16:08:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-tools/pull/12" class=".btn">#12</a>
            </td>
            <td>
                <b>
                    fix: return tag_value if no value_key
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes what seems to have been a bug in the handling of plaintext tags.

@andrewwhitehead this line was one we happened to inherit :slightly_smiling_face: I believe these changes captured the intended function of this method but a double check from you would be appreciated, if you get a chance.

Plaintext tags are not well used (I don't think they're used at all in ACA-Py) which let this bug slip past our testing which operates exclusively on ACA-Py wallets.

@blu3beri this also relates to a `TODO` line I noticed in https://github.com/hyperledger/aries-askar/pull/104 where you asked what `tag[1]` represented. I wasn't sure which lead to the discovery of this bug :slightly_smiling_face: 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-02 14:25:19 +0000 UTC
    </div>
</div>

