---
layout: default
title: indy-node-monitor
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-node-monitor
---

# indy-node-monitor <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-node-monitor){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-node-monitor/pull/64" class=".btn">#64</a>
            </td>
            <td>
                <b>
                    Changed the variable order for detailed view.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Changed the order of variables for the detailed view so you can select Network first and Nodes based upon what network is selected.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-18 20:35:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-node-monitor/pull/63" class=".btn">#63</a>
            </td>
            <td>
                <b>
                    Fix for decoding hex seed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Using `openssl rand -hex 32` to generate a monitoring DID seed results in a 64 character string, which causes an error when used. This adds a check for a 64 character string and decodes it as hex.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-17 17:29:03 +0000 UTC
    </div>
</div>

