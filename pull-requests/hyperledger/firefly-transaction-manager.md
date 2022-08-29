---
layout: default
title: firefly-transaction-manager
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-transaction-manager
---

# firefly-transaction-manager <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-transaction-manager){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/31" class=".btn">#31</a>
            </td>
            <td>
                <b>
                    Move completion log from "error" to "info"
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
        Created At 2022-08-29 17:49:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/29" class=".btn">#29</a>
            </td>
            <td>
                <b>
                    Integrating sprig into gasOracle.Template
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                http://masterminds.github.io/sprig/ is a common supplemental library for Go templating that has handy functions for ints and floats.

For oracle templates where we need to convert from gwei to wei, and /or convert from float to int, these utility functions can be very useful. This also provides us with a good starting point of examples in the event we ever need to write our own Go template functions such as converting from hex to bigints, etc.

Thanks @peterbroadhurst for doing the hard part of getting everything in place.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-26 04:15:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/28" class=".btn">#28</a>
            </td>
            <td>
                <b>
                    Fix hang broadcasting to broken connection
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Policy loop blocked...

```
goroutine 46 [chan send, 19 minutes]:
github.com/hyperledger/firefly-transaction-manager/internal/ws.(*webSocketServer).SendReply(0x1159540?, {0xa51b80?, 0xc001592140?})
	/go/pkg/mod/github.com/hyperledger/firefly-transaction-manager@v0.9.8/internal/ws/wsserver.go:163 +0x36
github.com/hyperledger/firefly-transaction-manager/pkg/fftm.(*manager).sendWSReply(0xc000369180, 0xc0015e8ea0)
	/go/pkg/mod/github.com/hyperledger/firefly-transaction-manager@v0.9.8/pkg/fftm/policyloop.go:293 +0x195
github.com/hyperledger/firefly-transaction-manager/pkg/fftm.(*manager).execPolicy(0xc000369180, {0xd803b8, 0xc0001d0210}, 0xc001d4be40, 0x0)
	/go/pkg/mod/github.com/hyperledger/firefly-transaction-manager@v0.9.8/pkg/fftm/policyloop.go:271 +0x7bf
github.com/hyperledger/firefly-transaction-manager/pkg/fftm.(*manager).policyLoopCycle(0xc000369180, {0xd803b8, 0xc0001d0210}, 0x1)
	/go/pkg/mod/github.com/hyperledger/firefly-transaction-manager@v0.9.8/pkg/fftm/policyloop.go:123 +0xf5
github.com/hyperledger/firefly-transaction-manager/pkg/fftm.(*manager).policyLoop(0xc000369180)
	/go/pkg/mod/github.com/hyperledger/firefly-transaction-manager@v0.9.8/pkg/fftm/policyloop.go:45 +0x1c6
created by github.com/hyperledger/firefly-transaction-manager/pkg/fftm.(*manager).Start
	/go/pkg/mod/github.com/hyperledger/firefly-transaction-manager@v0.9.8/pkg/fftm/manager.go:191 +0x26a
```

... by broadcast channel ...

```
goroutine 20 [chan send, 19 minutes]:
github.com/hyperledger/firefly-transaction-manager/internal/ws.(*webSocketServer).broadcastToConnections(...)
	/go/pkg/mod/github.com/hyperledger/firefly-transaction-manager@v0.9.8/internal/ws/wsserver.go:227
github.com/hyperledger/firefly-transaction-manager/internal/ws.(*webSocketServer).processReplies(0xc000129260)
	/go/pkg/mod/github.com/hyperledger/firefly-transaction-manager@v0.9.8/internal/ws/wsserver.go:221 +0x25e
created by github.com/hyperledger/firefly-transaction-manager/internal/ws.NewWebSocketServer
	/go/pkg/mod/github.com/hyperledger/firefly-transaction-manager@v0.9.8/internal/ws/wsserver.go:83 +0x216
```

I assert this is due to attempting to dispatch to a closed websocket connection.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-25 01:07:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/27" class=".btn">#27</a>
            </td>
            <td>
                <b>
                    add debug endpoint
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
        Created At 2022-08-24 18:34:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/26" class=".btn">#26</a>
            </td>
            <td>
                <b>
                    Remove the websocket.topic for simplicity and to avoid undefined behavior
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The original intention during EVMConnect was to remove this field, because the behavior around it in EthConnect was confusing.
- It had to be unique to each Event Stream
- We didn't enforce it to be unique
- If it wasn't unique, the behavior was undefined

However, we thought that compatibility/migration in FireFly Core and the ERC-20/ERC-721 and ERC-1155 token connectors would be a pain. So we put it back in...

We've since worked through all that in the tokens thanks to @awrichar in the following PRs, so this PR pulls it back out again:
- FireFly Core Ethereum Connector: ???
- ERC-1155: https://github.com/hyperledger/firefly-tokens-erc1155/pull/94
- ERC-20/ERC-721: https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/83

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-23 19:59:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/25" class=".btn">#25</a>
            </td>
            <td>
                <b>
                    Add delete functionality with policy engine involvement
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See https://github.com/hyperledger/firefly-transaction-manager/issues/24#issuecomment-1222821262

- New `DELETE` `/transactions/{transactionId}` API
- Adds new `DeleteRequested` field to the `ManagedTX` structure
- Changes `updated` boolean return on policy engine `Execute()` to an enum:
   - `UpdateYes` - same as current `true`
   - `UpdateNo` - same as current `false`
   - `UpdateDelete` - the transaction will be deleted from the persistence, with one last event emitted
- Invokes the policy engine once in-line with the API request
  - Returns `200` if that results in immediate removal
  - Returns `202` if the removal is not immediate, but the policy engine does not return an error
  - Returns an error if that run of the policy engine fails
- The policy engine executes this request sequentially with it's other processing
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-22 21:40:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/23" class=".btn">#23</a>
            </td>
            <td>
                <b>
                    Add checkpoint/catchup information from FFCAPI to listener GET API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves #22

- Calls the existing `EventListenerHWM` endpoint in the FFCAPI and mixes that into the API response for the listener
- Adds a `catchup` flag to that API, that allows an FFCAPI implementation to mark a stream as in catchup mode
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-22 18:31:39 +0000 UTC
    </div>
</div>

