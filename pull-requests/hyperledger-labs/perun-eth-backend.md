---
layout: default
title: perun-eth-backend
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/perun-eth-backend
---

# perun-eth-backend <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/perun-eth-backend){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-eth-backend/pull/44" class=".btn">#44</a>
            </td>
            <td>
                <b>
                    Restore compatibility between go-perun post-0.10.6 and eth-backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Two changes have been implemented in go-perun that break the eth-backend. This PR restores the compatibility by adapting to the changes made in go-perun:

- Removal of the ```Secondary``` field in ```channel.AdjudicatorReq``` [here](https://github.com/hyperledger-labs/go-perun/commit/be6e07257c123309c98fbbea4b86440275be2797).
- Creation of an AppID type to generalize App identifiers instead of using Ethereum addresses [here](https://github.com/hyperledger-labs/go-perun/commit/c23f66bcb91dd71ff6c24acb37adb2928bfee96a)

Note that this PR aims to close issue [#38 ](https://github.com/hyperledger-labs/perun-eth-backend/issues/38).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-12 13:16:10 +0000 UTC
    </div>
</div>

