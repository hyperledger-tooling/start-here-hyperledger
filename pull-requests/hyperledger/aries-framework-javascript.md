---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/995" class=".btn">#995</a>
            </td>
            <td>
                <b>
                    refactor(demo): Faber creates invitation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It's better if Faber creates an invitation than Alice does because we can test mobile agents with Faber more easily.
- Now, Faber creates an invitation and Alice receives it.
- I didn't change the code but just exchanged connection-related code between Alice and Faber.
- The second commit(1e6af7a) is a minor bug fix.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-29 08:37:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/994" class=".btn">#994</a>
            </td>
            <td>
                <b>
                    feat: connection type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added a connection type enum to the connection record so that you can filter the connections based on type. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-26 18:03:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/991" class=".btn">#991</a>
            </td>
            <td>
                <b>
                    feat: Discover Features V2 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Initial, non-breaking API implementation of Discover Features V2 with a `FeatureRegistry` where arbitrary features can be registered and queried by modules. 

Signed-off-by: Ariel Gentile <gentilester@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-25 04:39:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/990" class=".btn">#990</a>
            </td>
            <td>
                <b>
                    fix: expose oob domain
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-24 07:00:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/989" class=".btn">#989</a>
            </td>
            <td>
                <b>
                    feat(routing): manual mediator pickup lifecycle management
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Small update on Mediation Recipient module to allow stopping message pickup loop, and then restarting it anytime by calling `initiateMessagePickup()` manually.

An optional parameter has been added to **initiateMessagePickup** method in order to let start the agent with a `None` messagePickupStrategy (so it will not attempt to connect to mediator at the beginning) and be able to start the pickup afterwards (using any strategy we want).

So it can be used in the following way:

1) Start agent normally (with whatever Mediation Strategy you already have). It will initiate Pickup loop (V1, V2 or Implicit)
2) Call stopMessagePickup() to pause this process (e.g. when agent is offline)
3) Call initiateMessagePickup() to restart the process (e.g. agent goes online)

In case that default pickup strategy is set to None, of course, initiateMessagePickup should be called after 1 using parameters defaultMediator and the desired strategy (and the same in 3)

And I'm not completely sure, but it might also help with some failures in test suites when shutting down agents.

Resolves #753 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-23 18:26:50 +0000 UTC
    </div>
</div>

