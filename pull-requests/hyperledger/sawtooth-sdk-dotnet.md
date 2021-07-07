---
layout: default
title: sawtooth-sdk-dotnet
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/sawtooth-sdk-dotnet
---

# sawtooth-sdk-dotnet <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/sawtooth-sdk-dotnet){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-sdk-dotnet/pull/15" class=".btn">#15</a>
            </td>
            <td>
                <b>
                    Fixed Signer to ensure 256 bit signatures
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prepend the truncated zero bytes to both halves of the ECDSA signature.

Previously, the R and S values of the signatures would be concatenated
as-is. This would result in malformed signatures if any of the generated
BigInteger values were less than the expected 32 bytes in length.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-30 17:33:44 +0000 UTC
    </div>
</div>

