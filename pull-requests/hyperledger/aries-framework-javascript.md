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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/715" class=".btn">#715</a>
            </td>
            <td>
                <b>
                    fix: close session early if no return route
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a `close` method to all transport session so it can be closed from within the agent. This allows us to close the session early if the message doesn't have return routing enabled. Specifically this resolves the following issue raised:

> Hi Timo, I'm debugging our DIDCOMM protocol engine, and it seems that AFJ doesn't respond immediately after it has received the payload by HTTP POST. Our protocol state-machine keeps waiting for the response, but instead of that, AFJ sends a new HTTP POST request. Naturally, we could handle that, but could you please confirm that this is the case? Does your HTTP handlers block, i.e. process the payload and send the new request before responding?

Although it's not necesarily a wrong doing in AFJ, there is no need to keep the session open for longer than needed. Draft as this is dependant on some changes in this PR: https://github.com/hyperledger/aries-framework-javascript/pull/712
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-21 15:46:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/714" class=".btn">#714</a>
            </td>
            <td>
                <b>
                    feat: support handling messages with different minor version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds support for processing messages with a different minor version.

Some notes about the changes:
- The static `type` property on the message classes are now `ParsedMessageType` containing info about the message type. I've done this to make the info readily available and not have to parse it every time we need this info (would need to be done for every message for each message received). This is how declaring the type now looks. `praseMessageType` is an utitliy method that makes it easier to created the `ParsedMessageType` object.
```ts
class CustomProtocolMessage extends AgentMessage {
  @IsValidMessageType(CustomProtocolMessage.type)
  public readonly type = CustomProtocolMessage.type.messageTypeUri
  public static readonly type = parseMessageType('https://didcomm.org/fake-protocol/1.5/message')
}
```
- Had to refactor the decorators a bit as it was incorrectly typed which was now causing errors with typescript
- Added an e2e test where we send a message with a lower minor version to another agent with a higher minor version, and also a test where we send a message with a higher minor version to another agent with a lower minor version.
- Added transformations from string values `1` and `0` to `n__1` and `n__0`. See here for the relevant discussion: https://github.com/hyperledger/aries-framework-javascript/pull/690#discussion_r850942240. Other approaches very welcome.

~~This PR doesn't include handling the error case where we receive a message with a higher minor version. I'll like to address that in a separate PR (should be straightforward, we just have to change the reason in the problem report), but this at least unblocks us now.~~ -> Higher versions are now allowed, still need to send the problem report though in a future pr
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 10:49:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/712" class=".btn">#712</a>
            </td>
            <td>
                <b>
                    fix: allow agent without inbound endpoint to connect when using multi-use invitation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Quite an edge case, but when an agent without an inbound endpoint (e.g. mobile wallet connecting to mediator) would respond to a multi-use connection invitation (quite common with mediators) the session would be stored for the multi-use invitation connection. But during the processing of the request a new connection will be created, which means the session won't be reused afterwards because it's tied to the multi-use invitation connection. 

Normally this isn't that big a deal, as the next time a message is sent using the new connection the session can be reused, but for agent without an inbound transport this made it impossible to connect to AFJ. 

This PR adds the sessionId to the inbound message, and later attaches it to the outbound message. This is only used when directly responding to an incoming message. Wasn't sure if attaching the sessionId is the best here, but couldn't think of other straightforward approaches. We basically want to attach it to the inbound message, so we can just respond to the inbound session (instead of finding a session by the connection id, which is still used for a lot of other use cases)

Also changed the subject transport a bit to not require an inbound transport anymore when no inbound endpoint is configured (better reflects real-world setup)

Fixes #483 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-15 21:57:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/711" class=".btn">#711</a>
            </td>
            <td>
                <b>
                    feat: pickup v2 protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Implemented [pickup v2 protocol ](https://github.com/hyperledger/aries-rfcs/tree/main/features/0685-pickup-v2#delivery-request) along with unit testing for the implemented methods leaving room for future testing within the Mediation Recipient Module. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-15 21:57:09 +0000 UTC
    </div>
</div>

