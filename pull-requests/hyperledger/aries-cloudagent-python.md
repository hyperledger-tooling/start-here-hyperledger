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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2494" class=".btn">#2494</a>
            </td>
            <td>
                <b>
                    WIP: DID Rotate Protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is an early implementation of the DID Rotate protocol (currently a PR to Aries RFCs: https://github.com/hyperledger/aries-rfcs/pull/794). This was an exercise to feel out any potential issues with the protocol as defined.

This is not yet a complete implementation. Notably missing right now is a way to actually trigger a DID rotation through an Admin API call. I also need to finish wiring up the handlers to the manager. And who could forget about tests. :slightly_smiling_face: 

Overall, the protocol is solid. I'll report my thoughts on the protocol on the PR to the Aries RFCs.

An ACA-Py specific concern I discovered in this process that probably deserves some discussion: invalidating the connection target cache when the DID Rotation is committed. As currently structured, we never really expect the connection targets for a connection to change after the protocol establishing it concludes. DID Rotation shakes that expectation up.

Right now, in my changes, I've added a `clear_connection_targets_cache` helper method to partially address this. It's partial because it will only work for ACA-Py when run as a single instance with the default in memory cache or if you're using Indicio's redis cache plugin for whole cluster shared caching.

I think it would be better for ACA-Py to use a value including both DIDs of the connection in the cache key as a more complete solution. The problem with this and why I've not done it on a first pass is that there would need to be some restructuring of how we use the `Responder` classes so that the `send` methods expect a whole `ConnRecord` and not just a `connection_id` (or individually a `their_did` and `my_did`, I suppose) so we can extract the DIDs from it. 9 times out of 10, I would say that connection record is already available to the caller of the `send` method and my hypothesis is that in the remaining 1 time out of 10, it will not dramatically impact performance of critical operations (it is not common for us to know the connection_id and not also have a connection record -- maybe only a few places in the Admin API might be like this).

I'll do some more investigation on these points. Might be good to talk implications at the next ACA-PUG call.

cc @swcurran @TelegramSam
FYI @Jsyro this has ties back to updating the DIDs associated with connections that we've talked about recently.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-15 02:21:56 +0000 UTC
    </div>
</div>

