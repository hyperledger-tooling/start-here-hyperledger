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
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/306" class=".btn">#306</a>
            </td>
            <td>
                <b>
                    :boom: Channel.Update/ForceUpdate: updater no longer returns error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #155 

Instead of changing the API drastically, improve documentation.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-25 16:51:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/305" class=".btn">#305</a>
            </td>
            <td>
                <b>
                    💥 Rename wire message types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Consistently use the pattern `<message-name>Msg` for all message types.

- Export the unexported message types, so that newer wire serialization adapters can define functions for serializing/de-serializing these messages.

Closes #302


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-24 12:02:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/304" class=".btn">#304</a>
            </td>
            <td>
                <b>
                    303 check assets
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #303 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-21 12:43:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/300" class=".btn">#300</a>
            </td>
            <td>
                <b>
                    Fix virtual channel proposal id generation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Previously, the proposal ID for a virtual channel was generated using
  the ProposalID method defined on BaseChannelProposal.

- Hence, not all parameters of the virtual channel proposal were used.

- Fix it by defining a ProposalID method on the virtual channel.

- Also, remove the ProposalID method on the BaseChannelProposal, as it
  is not needed.

Fixes #299.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 07:42:30 +0000 UTC
    </div>
</div>

