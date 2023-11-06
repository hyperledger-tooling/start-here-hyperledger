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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1132" class=".btn">#1132</a>
            </td>
            <td>
                <b>
                    Fix test-network chaincode-as-a-service deployment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves a regression introduced in e73bb717db47185a8ccd1b701503b369cd2a73e1.

Previous change defaulted to "auto" as the sequence number but omitted the call to generate the correct sequence number for the "auto" value. This resulted in "auto" being used as the sequence number, which is an error since an integer is required.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-05 13:14:26 +0000 UTC
    </div>
</div>

