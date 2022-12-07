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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2037" class=".btn">#2037</a>
            </td>
            <td>
                <b>
                    Json-ld doc fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-02 17:05:21 +0000 UTC
    </div>
</div>

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

