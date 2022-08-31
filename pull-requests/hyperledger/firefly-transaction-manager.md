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
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/32" class=".btn">#32</a>
            </td>
            <td>
                <b>
                    Pass options.signer for EthCompat mode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                EVMConnect will separate out the option `options.signer: true` from the `options.methods: []` list of methods to match, so you can just request `signer`. Also so that even if no methods match we still set the signer.

This means a tweak to the EthCompat mode
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-29 21:07:59 +0000 UTC
    </div>
</div>

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

