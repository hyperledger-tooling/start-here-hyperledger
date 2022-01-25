---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/444" class=".btn">#444</a>
            </td>
            <td>
                <b>
                    Restore Transaction reference on TokenTransfer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Although transfers initiated outside of FireFly will NOT have a Transaction, it's
still useful to track Transactions for those transfers initiated by FireFly. This
is needed for tracking of async transfer requests, filtering transfers, etc.

Partially reverts 0e654d2a7b9960e3d2a4946c788f80e5052e056e
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-24 23:17:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/443" class=".btn">#443</a>
            </td>
            <td>
                <b>
                    Rename /contracts/events to /blockchainevents
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also move the query helpers from Contract Manager to Orchestrator, as this
has become a generic construct that spans more than one manager/plugin.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-24 22:52:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/441" class=".btn">#441</a>
            </td>
            <td>
                <b>
                    Create a Transaction and Operation for contract invoke requests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves #393
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-24 19:14:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/439" class=".btn">#439</a>
            </td>
            <td>
                <b>
                    v0.11.x backport: Ready state changes require a bump to the message to re-sequence it
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport_v0.11.x</span>
            </td>
            <td>
                Backport of #438 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-23 21:33:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/438" class=".btn">#438</a>
            </td>
            <td>
                <b>
                    Ready state changes require a bump to the message to re-sequence it
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-candidate</span><span class="chip">backport-complete</span>
            </td>
            <td>
                Fixes the core symptom reported in #421 

> Note that this does not implement the full change to batches described in the discussion on that issue.
> However, when that change happens, this fix will still be applicable.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-23 17:41:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/436" class=".btn">#436</a>
            </td>
            <td>
                <b>
                    Add AddressResolver to Ethereum for key-to-address mapping
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a REST-pluggable interface to the ethereum Blockchain plugin, that allows it to resolve non-Address strings (such as hierarchical HD wallet addresses) into ethereum addresses.

This supports a common configuration for signing as follows:

```
┌------------┐            ┌------------┐                ┌------------┐                ┌------------┐
|            |            |            |                |            |                |            |
|            |            |            |                |            |                |            |
|  FireFly   | -- REST -> | EthConnect | -- JSON/RPC -> |   Signer   | -- JSON/RPC -> |    Node    |
|            |            |            |   (unsigned)   |            |    (signed)    |            |
|            |            |            |                |            |                |            |
└-----┬------┘            └------------┘                └-----┬------┘                └------------┘
      |                                                       |
      └---------- Resolve non-address signing key ID ---------┘
```

Note that much of the FireFly relies on one-time resolution of the signing key, into a string
that is stored in database objects for later signing.

So once the interface has been used to resolve the key the target microservice **must**
reliably retain knowledge of the resolved address such that it can be used to perform
the actual transaction signing.

> The original input string is discarded by FireFly after resolution
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-23 02:01:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/435" class=".btn">#435</a>
            </td>
            <td>
                <b>
                    Fail transaction when token transfer operation fails
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #434
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-21 21:29:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/432" class=".btn">#432</a>
            </td>
            <td>
                <b>
                    v0.11.x backport: Fixing Websocket Connections when Prometheus Metrics Enabled + containerd update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport_v0.11.x</span>
            </td>
            <td>
                See #371

Also contains #414 `go.mod` update
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-21 03:36:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/431" class=".btn">#431</a>
            </td>
            <td>
                <b>
                    v0.11.x backport: Fix token account listing on Postgres
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport_v0.11.x</span>
            </td>
            <td>
                See #422 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-21 03:25:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/430" class=".btn">#430</a>
            </td>
            <td>
                <b>
                    v0.11.x backport: Add ping/pong heartbeating to WSClient, and fix concurrent map on config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport_v0.11.x</span>
            </td>
            <td>
                See https://github.com/hyperledger/firefly/pull/420
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-21 03:16:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/429" class=".btn">#429</a>
            </td>
            <td>
                <b>
                    v0.11.x backport: Fix querying transfers by tx or type, batches by tx
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport_v0.11.x</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-20 23:55:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/424" class=".btn">#424</a>
            </td>
            <td>
                <b>
                    Fix intermittent Fabric E2E test failure
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves https://github.com/hyperledger/firefly/issues/423
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-20 13:43:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/422" class=".btn">#422</a>
            </td>
            <td>
                <b>
                    Fix token account listing on Postgres
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-candidate</span><span class="chip">backport-complete</span>
            </td>
            <td>
                Postgres has much stricter constraints on DISTINCT/GROUP BY queries - specifically,
the fields used in ORDER BY must also be part of SELECT, and therefore may need
an aggregate function applied in order to give deterministic results.

Implement ordering by "seq" or "updated", which seem like the most useful.

Resolves #416
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-20 04:12:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/420" class=".btn">#420</a>
            </td>
            <td>
                <b>
                    Add ping/pong heartbeating to WSClient, and fix concurrent map on config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-candidate</span><span class="chip">backport-complete</span>
            </td>
            <td>
                Primary fix in this PR, is to add a heartbeat to the `WSClient` connections, to allow quicker detection of a case where the websocket between FireFly Core and a connector (EthConnect, FabConnect, DX) fails silently.

The default is 30 seconds between sending `ping` packets, with a 30 second timeout.

The feature can be disabled by setting the `heartbeatInterval` to zero on a given websocket client configuration.

Example log output showing operation of the heartbeating:

```
$ docker-compose logs -f firefly_core_0 | grep WS
firefly_core_0_1  | [2022-01-20T03:18:14.047Z]  INFO WS ws://ethconnect_0:8080/ws connected pid=1
firefly_core_0_1  | [2022-01-20T03:18:14.092Z]  INFO WS ws://dataexchange_0:3000 connected pid=1
firefly_core_0_1  | [2022-01-20T03:18:14.101Z]  INFO WS ws://tokens_0:3000/api/ws connected pid=1
firefly_core_0_1  | [2022-01-20T03:18:44.014Z] DEBUG WS ws://ethconnect_0:8080/ws heartbeat timer popped (ping) after 30000.57ms pid=1
firefly_core_0_1  | [2022-01-20T03:18:44.015Z] DEBUG WS ws://ethconnect_0:8080/ws heartbeat completed (pong) after 0.51ms pid=1
firefly_core_0_1  | [2022-01-20T03:18:44.059Z] DEBUG WS ws://dataexchange_0:3000 heartbeat timer popped (ping) after 30000.65ms pid=1
firefly_core_0_1  | [2022-01-20T03:18:44.062Z] DEBUG WS ws://dataexchange_0:3000 heartbeat completed (pong) after 2.76ms pid=1
firefly_core_0_1  | [2022-01-20T03:18:44.068Z] DEBUG WS ws://tokens_0:3000/api/ws heartbeat timer popped (ping) after 30001.13ms pid=1
firefly_core_0_1  | [2022-01-20T03:18:44.070Z] DEBUG WS ws://tokens_0:3000/api/ws heartbeat completed (pong) after 1.25ms pid=1
firefly_core_0_1  | [2022-01-20T03:19:13.982Z] DEBUG WS ws://ethconnect_0:8080/ws heartbeat timer popped (ping) after 30001.21ms pid=1
firefly_core_0_1  | [2022-01-20T03:19:13.983Z] DEBUG WS ws://ethconnect_0:8080/ws heartbeat completed (pong) after 0.92ms pid=1
firefly_core_0_1  | [2022-01-20T03:19:14.029Z] DEBUG WS ws://dataexchange_0:3000 heartbeat timer popped (ping) after 30001.20ms pid=1
firefly_core_0_1  | [2022-01-20T03:19:14.031Z] DEBUG WS ws://dataexchange_0:3000 heartbeat completed (pong) after 1.04ms pid=1
firefly_core_0_1  | [2022-01-20T03:19:14.037Z] DEBUG WS ws://tokens_0:3000/api/ws heartbeat timer popped (ping) after 30001.35ms pid=1
firefly_core_0_1  | [2022-01-20T03:19:14.039Z] DEBUG WS ws://tokens_0:3000/api/ws heartbeat completed (pong) after 1.23ms pid=1
firefly_core_0_1  | [2022-01-20T03:19:43.948Z] DEBUG WS ws://ethconnect_0:8080/ws heartbeat timer popped (ping) after 29999.30ms pid=1
firefly_core_0_1  | [2022-01-20T03:19:43.949Z] DEBUG WS ws://ethconnect_0:8080/ws heartbeat completed (pong) after 0.65ms pid=1
firefly_core_0_1  | [2022-01-20T03:19:43.998Z] DEBUG WS ws://dataexchange_0:3000 heartbeat timer popped (ping) after 30001.06ms pid=1
firefly_core_0_1  | [2022-01-20T03:19:44.001Z] DEBUG WS ws://dataexchange_0:3000 heartbeat completed (pong) after 1.99ms pid=1
firefly_core_0_1  | [2022-01-20T03:19:44.006Z] DEBUG WS ws://tokens_0:3000/api/ws heartbeat timer popped (ping) after 30001.08ms pid=1
firefly_core_0_1  | [2022-01-20T03:19:44.007Z] DEBUG WS ws://tokens_0:3000/api/ws heartbeat completed (pong) after 0.72ms pid=1
firefly_core_0_1  | [2022-01-20T03:20:13.916Z] DEBUG WS ws://ethconnect_0:8080/ws heartbeat timer popped (ping) after 30000.55ms pid=1
firefly_core_0_1  | [2022-01-20T03:20:13.917Z] DEBUG WS ws://ethconnect_0:8080/ws heartbeat completed (pong) after 0.63ms pid=1
firefly_core_0_1  | [2022-01-20T03:20:13.967Z] DEBUG WS ws://dataexchange_0:3000 heartbeat timer popped (ping) after 29999.39ms pid=1
firefly_core_0_1  | [2022-01-20T03:20:13.970Z] DEBUG WS ws://dataexchange_0:3000 heartbeat completed (pong) after 0.83ms pid=1
firefly_core_0_1  | [2022-01-20T03:20:13.974Z] DEBUG WS ws://tokens_0:3000/api/ws heartbeat timer popped (ping) after 30001.31ms pid=1
firefly_core_0_1  | [2022-01-20T03:20:13.975Z] DEBUG WS ws://tokens_0:3000/api/ws heartbeat completed (pong) after 0.79ms pid=1
firefly_core_0_1  | [2022-01-20T03:20:43.884Z] DEBUG WS ws://ethconnect_0:8080/ws heartbeat timer popped (ping) after 30001.25ms pid=1
firefly_core_0_1  | [2022-01-20T03:20:43.886Z] DEBUG WS ws://ethconnect_0:8080/ws heartbeat completed (pong) after 1.18ms pid=1
firefly_core_0_1  | [2022-01-20T03:20:43.936Z] DEBUG WS ws://dataexchange_0:3000 heartbeat timer popped (ping) after 30000.20ms pid=1
firefly_core_0_1  | [2022-01-20T03:20:43.936Z] DEBUG WS ws://dataexchange_0:3000 heartbeat completed (pong) after 0.48ms pid=1
firefly_core_0_1  | [2022-01-20T03:20:43.942Z] DEBUG WS ws://tokens_0:3000/api/ws heartbeat timer popped (ping) after 30000.69ms pid=1
firefly_core_0_1  | [2022-01-20T03:20:43.943Z] DEBUG WS ws://tokens_0:3000/api/ws heartbeat completed (pong) after 0.65ms pid=1
```

Also added a fix for this intermittent UT failure, which could hit real environments - by changing the locking in `config` to cover all cases of get/set concurrency:
```
goroutine 71 [running]:
runtime.throw(0x4ca0b0f, 0x21)
        /usr/local/Cellar/go/1.16.4/libexec/src/runtime/panic.go:1117 +0x72 fp=0xc0006bf9c8 sp=0xc0006bf998 pc=0x403b3b2
runtime.mapaccess2_faststr(0x4b64e00, 0xc0003df200, 0xc000680b10, 0x4, 0x53977c0, 0xc0003df100)
        /usr/local/Cellar/go/1.16.4/libexec/src/runtime/map_faststr.go:116 +0x4a5 fp=0xc0006bfa38 sp=0xc0006bf9c8 pc=0x4017625
github.com/spf13/viper.(*Viper).searchMap(0xc0000a61a0, 0xc0003df200, 0xc00068b340, 0x1, 0x2, 0x53977c0, 0x0)
        /Users/peterbroadhurst/dev/go/pkg/mod/github.com/spf13/viper@v1.10.1/viper.go:613 +0x5f fp=0xc0006bfa80 sp=0xc0006bfa38 pc=0x454ba5f
github.com/spf13/viper.(*Viper).isPathShadowedInDeepMap(0xc0000a61a0, 0xc00068b340, 0x2, 0x2, 0xc0003df200, 0x0, 0x0)
        /Users/peterbroadhurst/dev/go/pkg/mod/github.com/spf13/viper@v1.10.1/viper.go:749 +0x7f fp=0xc0006bfad0 sp=0xc0006bfa80 pc=0x454c3df
github.com/spf13/viper.(*Viper).find(0xc0000a61a0, 0xc000680b10, 0xe, 0x1, 0xc0006bfc40, 0x2)
        /Users/peterbroadhurst/dev/go/pkg/mod/github.com/spf13/viper@v1.10.1/viper.go:1267 +0xafd fp=0xc0006bfbe0 sp=0xc0006bfad0 pc=0x454e23d
github.com/spf13/viper.(*Viper).Get(0xc0000a61a0, 0xc000680b00, 0xe, 0x203000, 0x53958d0)
        /Users/peterbroadhurst/dev/go/pkg/mod/github.com/spf13/viper@v1.10.1/viper.go:843 +0x85 fp=0xc0006bfc78 sp=0xc0006bfbe0 pc=0x454c825
github.com/spf13/viper.(*Viper).GetString(0xc0000a61a0, 0xc000680b00, 0xe, 0xc000680b00, 0xe)
        /Users/peterbroadhurst/dev/go/pkg/mod/github.com/spf13/viper@v1.10.1/viper.go:910 +0x3f fp=0xc0006bfcb8 sp=0xc0006bfc78 pc=0x454d01f
github.com/spf13/viper.GetString(...)
        /Users/peterbroadhurst/dev/go/pkg/mod/github.com/spf13/viper@v1.10.1/viper.go:907
github.com/hyperledger/firefly/internal/config.(*configPrefix).GetString(0xc0001371f0, 0x4c86f9f, 0x9, 0x4c1a240, 0x30)
        /Users/peterbroadhurst/dev/photic/firefly/internal/config/config.go:552 +0x65 fp=0xc0006bfcf0 sp=0xc0006bfcb8 pc=0x455b3c5
github.com/hyperledger/firefly/internal/apiserver.(*apiServer).getPublicURL(0xc000032d80, 0x4de2e98, 0xc0001371f0, 0x0, 0x0, 0x5395780, 0x0)
        /Users/peterbroadhurst/dev/photic/firefly/internal/apiserver/server.go:417 +0x5e fp=0xc0006bfda8 sp=0xc0006bfcf0 pc=0x48b8bbe
github.com/hyperledger/firefly/internal/apiserver.(*apiServer).createMuxRouter(0xc000032d80, 0x4dd4f50, 0xc000032d40, 0x4de7ab0, 0xc00013a3c0, 0x0)
        /Users/peterbroadhurst/dev/photic/firefly/internal/apiserver/server.go:493 +0x158 fp=0xc0006bfe98 sp=0xc0006bfda8 pc=0x48b91d8
github.com/hyperledger/firefly/internal/apiserver.(*apiServer).Serve(0xc000032d80, 0x4dd4f50, 0xc000032d40, 0x4de7ab0, 0xc00013a3c0, 0x0, 0x1)
        /Users/peterbroadhurst/dev/photic/firefly/internal/apiserver/server.go:107 +0x35d fp=0xc0006bff18 sp=0xc0006bfe98 pc=0x48b6c7d
github.com/hyperledger/firefly/cmd.startFirefly(0x4dd4f50, 0xc000032d40, 0xc0004099d0, 0x4de7ab0, 0xc00013a3c0, 0x4dc0d00, 0xc000032d80, 0xc000046720)
        /Users/peterbroadhurst/dev/photic/firefly/cmd/firefly.go:163 +0x176 fp=0xc0006bffa0 sp=0xc0006bff18 pc=0x4964116
runtime.goexit()
        /usr/local/Cellar/go/1.16.4/libexec/src/runtime/asm_amd64.s:1371 +0x1 fp=0xc0006bffa8 sp=0xc0006bffa0 pc=0x4075181
created by github.com/hyperledger/firefly/cmd.run
        /Users/peterbroadhurst/dev/photic/firefly/cmd/firefly.go:118 +0x49e

goroutine 72 [runnable]:
github.com/spf13/viper.deepSearch(0xc0003dff50, 0xc0000331c0, 0x3, 0x4, 0x0)
				/Users/peterbroadhurst/dev/go/pkg/mod/github.com/spf13/viper@v1.10.1/util.go:189 +0x19c
github.com/spf13/viper.(*Viper).SetDefault(0xc0000a61a0, 0x4c9bd0c, 0x1d, 0x4b1b7e0, 0x4dab720)
				/Users/peterbroadhurst/dev/go/pkg/mod/github.com/spf13/viper@v1.10.1/viper.go:1437 +0x19d
github.com/spf13/viper.SetDefault(...)
				/Users/peterbroadhurst/dev/go/pkg/mod/github.com/spf13/viper@v1.10.1/viper.go:1428
github.com/hyperledger/firefly/internal/config.Reset()
				/Users/peterbroadhurst/dev/photic/firefly/internal/config/config.go:351 +0x1434
github.com/hyperledger/firefly/cmd.run(0x0, 0x0)
				/Users/peterbroadhurst/dev/photic/firefly/cmd/firefly.go:93 +0x47
github.com/hyperledger/firefly/cmd.glob..func1(0x5354fa0, 0x5395c48, 0x0, 0x0, 0x0, 0x0)
				/Users/peterbroadhurst/dev/photic/firefly/cmd/firefly.go:48 +0x32
github.com/spf13/cobra.(*Command).execute(0x5354fa0, 0x5395c48, 0x0, 0x0, 0x5354fa0, 0x5395c48)
				/Users/peterbroadhurst/dev/go/pkg/mod/github.com/spf13/cobra@v1.3.0/command.go:856 +0x472
github.com/spf13/cobra.(*Command).ExecuteC(0x5354fa0, 0x4dc3120, 0xc00013a601, 0xc000409c90)
				/Users/peterbroadhurst/dev/go/pkg/mod/github.com/spf13/cobra@v1.3.0/command.go:974 +0x375
github.com/spf13/cobra.(*Command).Execute(...)
				/Users/peterbroadhurst/dev/go/pkg/mod/github.com/spf13/cobra@v1.3.0/command.go:902
github.com/hyperledger/firefly/cmd.Execute(0x4c9086f, 0x13)
				/Users/peterbroadhurst/dev/photic/firefly/cmd/firefly.go:87 +0x45
github.com/hyperledger/firefly/cmd.TestExecOkRestartThenExit(0xc000103b00)
				/Users/peterbroadhurst/dev/photic/firefly/cmd/firefly_test.go:119 +0x3b0
testing.tRunner(0xc000103b00, 0x4cde8f0)
				/usr/local/Cellar/go/1.16.4/libexec/src/testing/testing.go:1193 +0xef
created by testing.(*T).Run
				/usr/local/Cellar/go/1.16.4/libexec/src/testing/testing.go:1238 +0x2b3
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-20 03:03:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/419" class=".btn">#419</a>
            </td>
            <td>
                <b>
                    JSON Schema validation for FFIs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR introduces JSON Schema into FFIs for describing `FFIParam`s. `FFIParam`s now have a `Schema` field that encompasses the previously used `Type` and `Details` fields.

The JSON Schema library used allows for extensions with custom compilers and validators to be added. So FireFly's JSON Schema for FFIs is a slightly more restrictive version of JSON Schema draft 2020-12 with the following requirements:

- The `type` field is always required
- The list of valid types are:
  - `string`
  - `integer`
  - `boolean`
  - `array`
  - `object`

The `type` field is now only used for telling FireFly the _input_ format of a field when a request is made to FireFly's API to invoke a smart contract.

For more specialized fields such as bytes, the input format would be `string` and an additional `contentEncoding` property can be added to the schema to indicate how to treat the contents of that string.

Additionally, blockchain plugins can expose a JSON Schema extension interface specific to that particular blockchain implementation. For example, the Ethereum plugin adds additional requirements (with another meta schema):

- `details` field is always required as an object
- `details` must contain a property called `type` that will always be a string
  - The compiler for the Ethereum JSON Schema extension also checks to make sure that the input type and the Ethereum type are a valid pairing
- An `indexed` boolean property is optional

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-20 02:07:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/417" class=".btn">#417</a>
            </td>
            <td>
                <b>
                    PostgreSQL updates following merging of onchain-logic branch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes for #415 

The PostgreSQL driver in Go passes `Scan` a `string` rather than a `[]byte` when reading data from the database, now that we are using `TEXT` columns. However, our custom `Scan()` implementations for these types assumed `[]byte` was being returned (in various spellings of that assumption).

To support environments created before the moved away from `BYTEA` we cannot take the old `Scan()` support for `[]byte`. So we need all the objects to support either.

Through incremental e2e test-fix cycles I found the following needed updates:
1. SQL Migration copy/paste bug from SQLite to PSQL
2. `fftypes.JSONObject`
3. `fftypes.JSONObjectArray`
4. `fftypes.Batch`
5. `fftypes.FFISerializedEvent`
6. `fftypes.FFIParams`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 16:06:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/414" class=".btn">#414</a>
            </td>
            <td>
                <b>
                    Update containerd
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-candidate</span><span class="chip">backport-complete</span>
            </td>
            <td>
                See https://github.com/advisories/GHSA-mvff-h3cj-wj9c
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 13:35:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/413" class=".btn">#413</a>
            </td>
            <td>
                <b>
                    [erc20-payload] pass name and symbol to CreateTokenPool()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The [ERC20 token connector](https://github.com/hyperledger/firefly-tokens-erc20) for Firefly requires that `name` and `symbol` be passed to the ERC20 token factory. This PR allows for firefly to pass these fields down to the token connector.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 08:11:53 +0000 UTC
    </div>
</div>

