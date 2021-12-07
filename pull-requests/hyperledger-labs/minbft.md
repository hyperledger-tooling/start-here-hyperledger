---
layout: default
title: minbft
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/minbft
---

# minbft <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/minbft){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/minbft/pull/219" class=".btn">#219</a>
            </td>
            <td>
                <b>
                    Simplified handling of certified messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                <!-- NOTE: Please check the contribution guideline before submitting -->

<!-- describe the purpose of the pull request, as well as its benefits
     and possible concerns related to the proposed changes -->
This pull request changes handling of messages certified with USIG. It requires replicas to send certified messages strictly sequentially in the assigned UI values. This applies both to replica's own messages and foreign messages embedded into replica's own messages. Moreover, only correct messages update the UI value tracked for each peer replica. These changes aim at simplifying reasoning about correctness of the implementation, especially when it comes to view change.

<!-- and reference any issues resolved by the pull request, e.g. #123 -->
Related to #217, #178.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-06 17:24:34 +0000 UTC
    </div>
</div>

