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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1465" class=".btn">#1465</a>
            </td>
            <td>
                <b>
                    Fix error removing proof req entries by timestamp
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

Addresses issue https://github.com/hyperledger/aries-cloudagent-python/issues/1455

(WIP not completed yet)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-30 00:12:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1464" class=".btn">#1464</a>
            </td>
            <td>
                <b>
                    Implement Revocation Notification v1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements revocation notifications following the RFC: https://github.com/hyperledger/aries-rfcs/blob/main/features/0183-revocation-notification/README.md

Currently, `~please_ack` support is not implemented and there is no way to propagate a comment from issuer to recipient. Hopefully this serves as a good starting point to collect feedback.

I've done some testing using the [revocation demo](https://github.com/Indicio-tech/acapy-revocation-demo) I put together a while ago and everything worked as expected but I plan to implement some tests (at a minimum unit tests, perhaps integration test with some direction from @ianco) before we merge this one.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-29 20:57:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1463" class=".btn">#1463</a>
            </td>
            <td>
                <b>
                    Allow base wallet to connect to a mediator after startup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Connecting the base wallet to a mediator is supported through command line arguments but not the Admin API. In our experience, it is often simpler to establish the base wallet's mediator after startup through the Admin API. That being said, there could be consequences to this change that I'm not seeing yet so hoping @ianco and @TimoGlastra could give their thoughts on this change.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-29 13:01:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1461" class=".btn">#1461</a>
            </td>
            <td>
                <b>
                    Auto connect from author to endoposer on startup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

If the appropriate startup arguments are provided, auto-initiate the connection between the author and endorser on agent startup
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-28 21:13:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1459" class=".btn">#1459</a>
            </td>
            <td>
                <b>
                    Startup and shutdown events (prep for endorser updates)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

Added startup and shutdown event notifications

@TimoGlastra  this adds startup/shutdown notifications (as discussed on RocketChat I think?), let me know if this is what you were thinking.  This is for the base wallet but assume we need something similar for sub-wallets?

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-27 22:38:21 +0000 UTC
    </div>
</div>

