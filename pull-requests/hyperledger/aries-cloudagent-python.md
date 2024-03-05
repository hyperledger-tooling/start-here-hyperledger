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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2822" class=".btn">#2822</a>
            </td>
            <td>
                <b>
                    Anoncreds - support for anoncreds and askar wallets concurrently
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Very much still in refactoring and testing stage.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-05 00:10:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2821" class=".btn">#2821</a>
            </td>
            <td>
                <b>
                    Send revocation list instead of rev_list object - Anoncreds
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes anoncreds specific problem on initial rev_list. Was sending the rev_list object to the event handler instead of the actual list.

Added a log message to v1 handler for after the message has been sent.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-01 18:56:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2820" class=".btn">#2820</a>
            </td>
            <td>
                <b>
                    FIX: GHA update for doc publishing, fix doc file that was blanked
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Next try (if needed) will get into the regex...
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-29 22:15:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2819" class=".btn">#2819</a>
            </td>
            <td>
                <b>
                    Allow for crids in event payload to be integers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The revocation notification not sending ended up being a simple bug. The crids from the ledger response was a list of integers but the list comprehension statement was expecting strings as thats what it gets from the wallet. I solved this by converting the list to strings to allow the payload to send integers. Think this is slightly better then making sure everywhere that ever uses this event handler is sending strings. Also added a bit better logging.

One thing I noticed is that both v1 and v2 handlers are both handling the same event. The first handler (v1 is loaded first) deletes the record so the v2 won't send the message. Not sure if this is what we want or not. Also the v1 wasn't using the `revocation.notify` config. So that is a bug as well I think. I changed v1 to recognize that config now.

Ran into a lot of things with testing traction locally against new acapy changes.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-28 21:54:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2816" class=".btn">#2816</a>
            </td>
            <td>
                <b>
                    feat: did-rotate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Taken from #2494 (c/o @dbluhm)

This PR is an early implementation of the [RFC 0794 DID Rotate protocol](https://github.com/hyperledger/aries-rfcs/tree/main/features/0794-did-rotate). This was an exercise to feel out any potential issues with the protocol as defined.

This is not yet a complete implementation. Notably missing right now is a way to actually trigger a DID rotation through an Admin API call. I also need to finish wiring up the handlers to the manager. And who could forget about tests. 🙂

Overall, the protocol is solid. I'll report my thoughts on the protocol on the PR to the Aries RFCs.

An ACA-Py specific concern I discovered in this process that probably deserves some discussion: invalidating the connection target cache when the DID Rotation is committed. As currently structured, we never really expect the connection targets for a connection to change after the protocol establishing it concludes. DID Rotation shakes that expectation up.

Right now, in my changes, I've added a clear_connection_targets_cache helper method to partially address this. It's partial because it will only work for ACA-Py when run as a single instance with the default in memory cache or if you're using Indicio's redis cache plugin for whole cluster shared caching.

I think it would be better for ACA-Py to use a value including both DIDs of the connection in the cache key as a more complete solution. The problem with this and why I've not done it on a first pass is that there would need to be some restructuring of how we use the Responder classes so that the send methods expect a whole ConnRecord and not just a connection_id (or individually a their_did and my_did, I suppose) so we can extract the DIDs from it. 9 times out of 10, I would say that connection record is already available to the caller of the send method and my hypothesis is that in the remaining 1 time out of 10, it will not dramatically impact performance of critical operations (it is not common for us to know the connection_id and not also have a connection record -- maybe only a few places in the Admin API might be like this).

I'll do some more investigation on these points. Might be good to talk implications at the next ACA-PUG call.

cc @swcurran @TelegramSam
FYI @Jsyro this has ties back to updating the DIDs associated with connections that we've talked about recently.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-27 21:14:27 +0000 UTC
    </div>
</div>

