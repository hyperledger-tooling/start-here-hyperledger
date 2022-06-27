---
layout: default
title: fabric-ca
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-ca
---

# fabric-ca <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-ca){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/306" class=".btn">#306</a>
            </td>
            <td>
                <b>
                    Correct handling of CA VerifyOptions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The verify options strucutre is global property - but the verify struture in the case
of re-enroll is set back by 30 seconds.

If this is the global structure - then that is not good.

Duplicating the structure.  Many ways to solve this problem; but this the current approach is cleaner.

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-27 13:08:41 +0000 UTC
    </div>
</div>

