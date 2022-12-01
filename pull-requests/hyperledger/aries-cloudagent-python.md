---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2034" class=".btn">#2034</a>
            </td>
            <td>
                <b>
                    Allow multi-use public invites and public invites with metadata
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adjusts the functionality of invitations created with Public DIDs.
Specifically, it does the following:
- allows for multi-use invitations to be created with a Public DID
- allows for an agent to create an invitation with metadata when using a Public DID
- adds a new flag governing behavior of an agent with a Public DID: `--requests-through-public-did`
    - This flag handles a slightly odd edge case. Prior to this PR, if Alice has `--public-invites` and `--auto-accept`, Bob could make an unsolicited connection request against Alice’s Public DId, which is to say, Bob is not responding to an explicit invitation that Alice has created. In that scenario, Alice would automatically accept that request. 
    - This flag separates that behavior from the `—public-invites` flag. `--public-invites` still allows for invitations to be created with a Public DID, but unless `--requests-through-public-did` is set, those unsolicited connection requests will be ignored.

Thanks to @dbluhm for additional conceptual design and help debugging :) 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-30 18:48:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2033" class=".btn">#2033</a>
            </td>
            <td>
                <b>
                    feat: Proof Negotiation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Łukasz Przytuła <lprzytula@gmail.com>

Allow proof negotiation by providing an updated proof request to `/present-proof/records/{pres_ex_id}/send-request` endpoint (if no proof request will be passed in body, it will be created according to the presentation proposal)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-29 23:08:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2031" class=".btn">#2031</a>
            </td>
            <td>
                <b>
                    fix: Correct typo in model -- required spelled incorrectly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

Signed-off-by: Stephen Curran <swcurran@cloudcompass.ca>

Signed-off-by: Stephen Curran <swcurran@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-25 22:44:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2030" class=".btn">#2030</a>
            </td>
            <td>
                <b>
                    Special handling for the write ledger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

Issue https://github.com/hyperledger/aries-cloudagent-python/issues/2002

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-25 18:19:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2026" class=".btn">#2026</a>
            </td>
            <td>
                <b>
                    Dock updates for json demo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

Addresses issue https://github.com/hyperledger/aries-cloudagent-python/issues/2014

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-24 21:17:54 +0000 UTC
    </div>
</div>

