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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1854" class=".btn">#1854</a>
            </td>
            <td>
                <b>
                    python-3.7 update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # UNDER RAPID DEVELOPMENT!
This draft PR updates ACA-PY to use python-3.7 along with dependency updates. 
For questions during development please reach out to @burdettadam or @dbluhm.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-05 18:14:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1853" class=".btn">#1853</a>
            </td>
            <td>
                <b>
                    fix: return if return route but no response
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Small fix to return an http inbound session if the return route decorator is present but the processing of the message did not elicit a response. Ended up being a quite straightforward fix. Current behaviour is to keep the socket open and hang indefinitely.

I would like some input on this PR as it changes behaviour and makes e.g. long polling impossible. However I do think there's ways to work around that. As @smithbk pointed out in #1372 we could reserve the `noop` message from the pickup protocol for this. 

Currently clients have to guess whether ACA-Py succesfully received the message as it won't return a 200 response. This mens that e.g. in AFJ we terminate the request after 15 seconds and just assume it went well if return routing was enabled.

We could of course disable return routing in the client (I'll make an additional PR to AFJ), but I think it's good to also fix the behaviour in ACA-Py.

The behaviour as implemented in this PR is also what's implemented in AFJ. We process the message, and if the processing didn't elicit a response we terminate the socket for HTTP. For websockets we keep it alive as it's more expected to have long lived sessions.

With current behaviour how it is implemented in AFJ's client side I was able to reduce the setup process (create connection with mediator, request mediation) from 17 to 1.7 seconds. Of course this is because AFJ has a set timeout of 15 seconds, but I suspect other implementations will have similar behaviour.

Fixes #1372 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-04 20:33:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1851" class=".btn">#1851</a>
            </td>
            <td>
                <b>
                    Enable manually triggering keylist updates during connection
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is a significant refactor of routing for both Mediation and Multi-tenancy, impacting Connections, Out-of-band, and DID Exchange managers, with the goal of eliminating a race condition possible when using mediation. Additionally, this PR also simplifies routing setup significantly for both mediation and multi-tenancy.

### Mediation Race Condition during Connection Formation

During connection formation, the current implementation of mediation support triggers a keylist update message to be sent just prior to sending the connection request or response (or a DID Exchange request or response) **without** waiting for confirmation from the mediator that the keylist update was received and processed successfully. This can result in a scenario where the connection request or response is received and responded to before the mediator has processed the keylist update. Typically, the keylist update process is quick and, especially when using the default HTTP transport mechanisms, the chances of things getting out of order are very slim. However, when introducing outbound queuing or another transport, this race condition has proven to be frequent.

#### Mediation Client as Invitee
![image](https://user-images.githubusercontent.com/22032832/176949299-2eef91a5-c4b6-47b6-994a-8d627637e696.png)

#### Mediation Client as Inviter
![image](https://user-images.githubusercontent.com/22032832/176950192-3f385598-5430-4085-9ec8-35ffdc3363e6.png)

### Solution
To prevent this race condition, this PR adds the `/mediation/update-keylist/{conn-id}` Admin endpoint that is called after `receive-invitation` or `receive-request` and before `accept-invitation` or `accept-request`. This endpoint creates connection keys and sends those keys in a keylist update to the specified mediator. When combined with the changes in #1769, the controller can then wait for the keylist update response received webhook, match the thread_id to the id of the keylist update returned from `/mediation/update-keylist/{conn-id}`, and then proceed with the next step in the connection.

![image](https://user-images.githubusercontent.com/22032832/176953386-630b8a1d-b9a6-45ca-b4d9-e2957ccbb6eb.png)

![image](https://user-images.githubusercontent.com/22032832/176953427-1a4cdf60-72e5-4f2e-8e2f-a96840238c47.png)


This should look familiar; this is more or less how the old `establish-inbound` endpoint worked. However, a key difference and the next major addition of this PR is the new `RouteManager` abstract base class. Two concretions are included in this PR: one for standard Coordinate Mediation v1 route management and one for Multi-tenancy + Mediation, which handles base wallet route creation and routing through a base wallet mediator and/or a sub wallet mediator.

Using the `RouteManager` to abstract away routing details, the Connection, OOB, and DIDExchange managers have each been significantly simplified (IMHO :slightly_smiling_face:).

Some additional notes:
- This is a backwards compatible change. If `/mediation/update-keylist/{conn-id}` is not used, forming connections through a mediator should behave exactly as before.
- This PR also corrects a slight misbehavior where both the base wallet's and sub wallet's mediator were informed of new connection keys being formed, even though the base wallet mediator was the only mediator in that chain that would have seen those keys.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-01 18:55:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1849" class=".btn">#1849</a>
            </td>
            <td>
                <b>
                    0.7.4 Release Changelog and version update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-30 17:12:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1847" class=".btn">#1847</a>
            </td>
            <td>
                <b>
                    Fix handling of non-revocable credential when timestamp is specified (askar/credx)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Test output with the error (mixing revocable and non-revocable credentials in one proof): https://github.com/hyperledger/aries-cloudagent-python/pull/1761#issuecomment-1165468687

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-29 22:44:10 +0000 UTC
    </div>
</div>

