---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/905" class=".btn">#905</a>
            </td>
            <td>
                <b>
                    Fix java contract paperkey parameter in commercial paper example
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In Java contract of "commercial paper" example, the "paperkey" is not equivalent of "paperNumber" parameter only, but  it's a combination of "issuer" and "paperNumber" params.
this is already done for Js https://github.com/hyperledger/fabric-samples/blob/main/commercial-paper/organization/magnetocorp/contract/lib/papercontract.js#L104
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-14 12:43:05 +0000 UTC
    </div>
</div>

