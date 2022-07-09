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

