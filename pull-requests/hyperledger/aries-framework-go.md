---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2859" class=".btn">#2859</a>
            </td>
            <td>
                <b>
                    chore: refactor CreateDestination interop behaviour behind flag
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-07 15:06:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2857" class=".btn">#2857</a>
            </td>
            <td>
                <b>
                    fix: Implemented iterator interface in pkg/mock/storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-06 14:01:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2856" class=".btn">#2856</a>
            </td>
            <td>
                <b>
                    feat: support packer selection based on destination MediaType
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change sets the media type priority based on the destination according to Aries RFCs 19, 44 and 587.
It sets the JWE message's CTY header based on the received media type.
It also updates the default authcrypt packing sender key type to be AES256CBCHS512.

closes #1112 (packer is selected based on mediaTypeProfile)
closes #272 (key type is managed by the kms)
closes #749 (diffrent keys are supported by the packers, except LegacyPacker that supports ED25519 keys only)
closes #2858 (SendToDID now can be used without a DID connection, as it was before)

Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-06 04:24:12 +0000 UTC
    </div>
</div>

