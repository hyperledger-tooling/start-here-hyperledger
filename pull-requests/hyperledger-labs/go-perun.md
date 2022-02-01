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
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/309" class=".btn">#309</a>
            </td>
            <td>
                <b>
                    eth/channel: Fix tx receipt pulling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #308 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-31 16:15:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/307" class=".btn">#307</a>
            </td>
            <td>
                <b>
                    :boom: Update the mechanism for propsal ID generation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As described in #301, use the proposer nonce share as the proposal ID.

Also,

- Update the tests for proposal ID generation by removing the assertions that
  check if the proposal ID changes when the channel parameters change.

- Make the ProposalID a field of BaseChannel proposal, as it does not depend on
  the type of channel proposal and remove the proposal ID method from
  `ChannelProposal` interface.

Closes #301.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 14:26:57 +0000 UTC
    </div>
</div>

