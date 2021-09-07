---
layout: default
title: go-perun
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/go-perun
---

# go-perun <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/go-perun){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/175" class=".btn">#175</a>
            </td>
            <td>
                <b>
                     Modify Adjudicator.Subscribe to take channel.ID instead of channel.Params
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Previously, Adjudicator.Subscribe was taking channel.Params, while it
  was using only the ID contained in the params.

- So, modified the API to take only the required parameter.

Resolves #173.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-01 18:28:26 +0000 UTC
    </div>
</div>

