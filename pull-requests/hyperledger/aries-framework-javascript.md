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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1639" class=".btn">#1639</a>
            </td>
            <td>
                <b>
                    OpenId4Vc Support
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
        Created At 2023-11-15 15:31:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1638" class=".btn">#1638</a>
            </td>
            <td>
                <b>
                    feat!: message pickup live mode support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As promised, some progress in supporting missing features from [RFC 0685](https://github.com/hyperledger/aries-rfcs/tree/main/features/0685-pickup-v2), most notably the "Live Mode", in such a way that might be compatible with a multi-instance architecture as discussed in #1625.

Conceptually, it consists mostly in changes in Mediator role, where we can choose our strategy when a Forward message is received:  
- We can simply queue it to the `MessagePickupRepository`, so it will be in charge of manually trigger a delivery of queued messages: this can be possible because `MessagePickupModule` now emits events when Live Sessions are opened and closed (so any consumer of an AFJ instance can subscribe to a central Message Pickup Repository and know if a newly queued message belongs to any of its connected clients), and `MessagePickupApi` exposes a method to deliver any queued message using V2 protocol.
- We can try to deliver it immediately using V2 protocol, previously adding it to the queue and . This is mostly useful in single instance AFJ scenarios, yet taking advantage of the protocol-level acknowledges Pickup V2 provides
- We can try to deliver the encrypted message immediately, without any protocol-level encapsulation. This is what AFJ does now, in a kind of 'implicit mode' (not recommended as it is more unreliable)

On `mediatee` side, there is a new `MediatorPickupStrategy` called `PickUpV2LiveMode` where, once it connects to Mediator WebSocket, it will set Live Delivery mode on (retrieving, as usual, any pending message). Current `PickUpV2` mode works in polling mode (sending a `status-request` message every `mediatorPollingInterval` milliseconds.

Some changes done so far:

- `MediatorModule` now has a config parameter to select its message forwarding strategy
- `MessagePickupApi` includes Live Mode session service that keeps track of all connected clients using V2 protocol in Live Mode and exposes a method to deliver any queued message to them. When new sessions are added or removed, it emits events
- `MessageRepository` was renamed to `MessagePickupRepository` (any better naming is more than welcome!) and methods were changed to allow removal of messages by their id and filter by connectionId/recipientKey
- `MessagePickupRepository` is now completely responsibility of `MessagePickupModule`: an in-memory default implementation will be instantiated if not specified in its config or defined externally before instantiating the Agent
- `TransportService` now emits events when sessions are created and removed. This was done mainly to be consumed by `MessagePickupSessionService`, but they can also be useful externally


There are lots of TODOS, especially about testing different settings. And also doubts like:

- Filtering by recipientKey doesn't sound that hard to implement, but Pickup V2 protocol is so open that it can allow a client to create a dedicated Live Mode session for a single recipient key
- It does not explicitly tells about that, but the protocol assumes that `delivery` message always come as a response to a `delivery-request`. Otherwise, how can I know what's the limit of messages I can batch on it (or if I should set recipient_key parameter)?

I'll for sure add more things in the incoming days but, if you have some time to bring your ideas and feedback on the approaches followed here, they will be really welcome!
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-15 02:29:29 +0000 UTC
    </div>
</div>

