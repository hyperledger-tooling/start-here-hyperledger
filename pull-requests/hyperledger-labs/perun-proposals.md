---
layout: default
title: perun-proposals
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/perun-proposals
---

# perun-proposals <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/perun-proposals){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-proposals/pull/9" class=".btn">#9</a>
            </td>
            <td>
                <b>
                    Update API Spec to use ERC20 token as currencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                 - An API is added to register new currencies. Because there are many
  ERC20 tokens, user should be able to register new ones.
    
 - Contract address are returned as map in node configuration. Since new
   currencies can be dynamically added, the list of asset holder
   contracts registered with the node will also be updated dynamically (one
   asset holder contract for each ERC20 token).
    
 - Add a payment data format and use it in the send payments API.

Relates to hyperledger-labs/perun-node#192.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-02 12:02:08 +0000 UTC
    </div>
</div>

