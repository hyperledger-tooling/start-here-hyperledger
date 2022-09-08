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
                PR <a href="https://github.com/hyperledger/firefly/pull/1050" class=".btn">#1050</a>
            </td>
            <td>
                <b>
                    Handle FFTM new style acks with batchNumber
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See https://github.com/hyperledger/firefly-transaction-manager/pull/36

> Leaving in draft mode until we have an FFTM+EVMConnect release, to include in the manifest
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-08 02:57:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1048" class=".btn">#1048</a>
            </td>
            <td>
                <b>
                    Consistently fall back to ff_system for legacy identity lookups
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Reverts #1035 
Fixes #1032
Fixes #1045 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-07 18:07:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1047" class=".btn">#1047</a>
            </td>
            <td>
                <b>
                    Properly enforce uniqueness of BatchPin blockchain events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Because listener_id is NULL for these events, we need separate indexes for when it is NULL and not NULL.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-07 14:19:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1046" class=".btn">#1046</a>
            </td>
            <td>
                <b>
                    update public chain docs
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
        Created At 2022-09-07 14:07:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1044" class=".btn">#1044</a>
            </td>
            <td>
                <b>
                    adding test cases for cache init errors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix coverage decrement introduced by central cache PR.

Signed-off-by: Chengxuan Xing <chengxuan.xing@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-06 21:28:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1043" class=".btn">#1043</a>
            </td>
            <td>
                <b>
                    Fix sequence query in auditevents
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Need to keep requesting new chunks of events even if the previous chunk
contained no matches.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-06 19:45:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1040" class=".btn">#1040</a>
            </td>
            <td>
                <b>
                    Update manifest for v1.1.0-rc.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Peter Broadhurst <peter.broadhurst@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-03 02:41:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1039" class=".btn">#1039</a>
            </td>
            <td>
                <b>
                    Updates to Home and Understanding FireFly sections
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updated description of what FireFly is on the "Home" page.

Reorganized Understanding FireFly section flow

No changes to any other sections.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-02 19:16:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1038" class=".btn">#1038</a>
            </td>
            <td>
                <b>
                    [address-resolver-route] POST /verifiers/resolve
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `POST /api/v1/verifiers/resolve`
Payload:

```json
{
  "type": "ethereum_address",
  "value": "hd-1-0-3"
}
```
Response

```json
{
  "type": "ethereum_address",
  "value": "0x7301ed0266c954309e62f76749d6c75a32c7c0b1"
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-02 12:49:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1037" class=".btn">#1037</a>
            </td>
            <td>
                <b>
                    Allow gateway init with DX and Shared Storage plugins + /data APIs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This allows use of the #1034 data for Gateway scenarios, such as publishing NFT metadata to IPFS.

Note that DX is used for local storage of the blob data only.

I've tried to carefully work through what is enabled:
- Removing the restriction of what plugins can be configured
- Determining which plugins/managers are enabled based on the plugins configured
- Allowing the broadcast manager to initialize without a batch manager, or multiparty
- Tweak the APIs so all the on-chain/off-chain messaging APIs are only multiparty
- Enable the data APIs only when the data manager is available
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-02 03:03:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1036" class=".btn">#1036</a>
            </td>
            <td>
                <b>
                    Prevent panic on ff_system namespace for synchronous token pool creation in V1.0 migrated env
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The following panic was occurring when using an ERC-20 connector, in an environment that had been migrated from V1.0, so had the `ff_system` namespace event listener running.

The panic failed the request to create the token pool with a `500`, but the token pool was created successfully.

The problem is specific to a `200 OK` return (rather than `202 Accepted`) return from the token connector on `/api/v1/createpool`, because there is no `blockchain` field (translated to `pool.Event` during processing) in the data from the connector on that path.

So this line would panic, dereferencing the `pool.Event.ProtocolID`:
https://github.com/hyperledger/firefly/blob/c5cc7ede18e6127277ebce4715baffb69d2ca513/internal/events/token_pool_created.go#L172

I've tidied up various logging along the way.

I also tidied up the path that was extracting `tokenData` in-line in the `handleTokenPoolCreate` calls, as in the `200 OK` in-line case the caller knows it. So this gets rid of an ugly log error like this, which was cruft:

```
[2022-09-01T19:03:12.399Z]  INFO TokenPool event data could not be parsed - continuing anyway (unexpected end of JSON input): {"decimals":18,"info":{"address":"0xc4c534921ccc96eb0342dffa9f0a0df21a3caf70","name":"f","schema":"ERC20WithData"},"poolLocator":"address=0xc4c534921ccc96eb0342dffa9f0a0df21a3caf70\u0026schema=ERC20WithData\u0026type=fungible","standard":"ERC20","symbol":"f","type":"fungible"} ns=default pid=123 role=aggregator
```

Original panic stack:

```
2022/09/01 19:03:04 http: panic serving 127.0.0.1:57740: runtime error: invalid memory address or nil pointer dereference
goroutine 749 [running]:
net/http.(*conn).serve.func1(0xc0007c1900)
	/usr/local/go/src/net/http/server.go:1804 +0x153
panic(0xf50420, 0x16c6b10)
	/usr/local/go/src/runtime/panic.go:971 +0x499
github.com/hyperledger/firefly/internal/events.(*eventManager).TokenPoolCreated.func1.1(0x11c5e98, 0xc0001104e0, 0xc000149860, 0x11c5e98)
	/firefly/internal/events/token_pool_created.go:172 +0x26f
github.com/hyperledger/firefly/internal/database/sqlcommon.(*SQLCommon).RunAsGroup(0xc0000ec820, 0x11c5e98, 0xc0001104e0, 0xc000088f30, 0x0, 0x0)
	/firefly/internal/database/sqlcommon/sqlcommon.go:159 +0x128
github.com/hyperledger/firefly/internal/events.(*eventManager).TokenPoolCreated.func1(0x1, 0xe, 0x0, 0xc000941e00)
	/firefly/internal/events/token_pool_created.go:145 +0xbc
github.com/hyperledger/firefly-common/pkg/retry.(*Retry).Do(0xc0000e8088, 0x11c5e98, 0xc000149860, 0x1082e05, 0x1e, 0xc000638df8, 0x0, 0x0)
	/go/pkg/mod/github.com/hyperledger/firefly-common@v1.1.1/pkg/retry/retry.go:56 +0xad
github.com/hyperledger/firefly/internal/events.(*eventManager).TokenPoolCreated(0xc0000e8000, 0x11d1580, 0xc00025df10, 0xc0007aac80, 0x0, 0x0)
	/firefly/internal/events/token_pool_created.go:144 +0xfa
github.com/hyperledger/firefly/internal/tokens/fftokens.(*callbacks).TokenPoolCreated(0xc00025df30, 0x11c5e98, 0xc00008ee10, 0xc0007aac80, 0xc000032d80, 0x0)
	/firefly/internal/tokens/fftokens/fftokens.go:71 +0xcd
github.com/hyperledger/firefly/internal/tokens/fftokens.(*FFTokens).handleTokenPoolCreate(0xc00025df10, 0x11c5e98, 0xc00008ee10, 0xc000032c90, 0xc000012260, 0x0)
	/firefly/internal/tokens/fftokens/fftokens.go:354 +0x50e
github.com/hyperledger/firefly/internal/tokens/fftokens.(*FFTokens).CreateTokenPool(0xc00025df10, 0x11c5e98, 0xc00008ee10, 0xc000318240, 0x2c, 0xc0003c8b60, 0x24, 0xc000318240, 0x2c)
	/firefly/internal/tokens/fftokens/fftokens.go:600 +0x745
github.com/hyperledger/firefly/internal/assets.(*assetManager).RunOperation(0xc0005ee420, 0x11c5e98, 0xc00008ee10, 0xc000181c20, 0xc000639270, 0x1, 0x1, 0xc00040ec40)
	/firefly/internal/assets/operations.go:109 +0x47b
github.com/hyperledger/firefly/internal/operations.(*operationsManager).RunOperation(0xc0000ed310, 0x11c5e98, 0xc00008ee10, 0xc000181c20, 0x0, 0x0, 0x0, 0x0, 0x0, 0x0)
	/firefly/internal/operations/manager.go:120 +0x334
github.com/hyperledger/firefly/internal/assets.(*assetManager).createTokenPoolInternal(0xc0005ee420, 0x11c5e98, 0xc00008ee10, 0xc0003c8b60, 0x0, 0x0, 0xc0004520c0, 0x2a)
	/firefly/internal/assets/token_pool.go:96 +0x362
github.com/hyperledger/firefly/internal/assets.(*assetManager).CreateTokenPool(0xc0005ee420, 0x11c5e98, 0xc00008ee10, 0xc0003c8b60, 0x1778e00, 0x50, 0xfe5f80, 0x1)
	/firefly/internal/assets/token_pool.go:56 +0x308
github.com/hyperledger/firefly/internal/apiserver.glob..func248(0xc0000ed5e0, 0xc0000ed630, 0xc00008ee10, 0xc00008f290, 0x0, 0x0)
	/firefly/internal/apiserver/route_post_token_pool.go:44 +0x111
github.com/hyperledger/firefly/internal/apiserver.(*apiServer).routeHandler.func1(0xc0000ed5e0, 0xc0000ed5e0, 0xc00013e240, 0xc00008f1a0, 0xc00008f200)
	/firefly/internal/apiserver/server.go:294 +0x3bd
github.com/hyperledger/firefly-common/pkg/ffapi.(*HandlerFactory).RouteHandler.func1(0x11c22d0, 0xc000a67200, 0xc0000b7800, 0x0, 0x0, 0x0)
	/go/pkg/mod/github.com/hyperledger/firefly-common@v1.1.1/pkg/ffapi/handler.go:162 +0x6a6
github.com/hyperledger/firefly-common/pkg/ffapi.(*HandlerFactory).APIWrapper.func1(0x11c22d0, 0xc000a67200, 0xc0000b7700)
	/go/pkg/mod/github.com/hyperledger/firefly-common@v1.1.1/pkg/ffapi/handler.go:262 +0x377
net/http.HandlerFunc.ServeHTTP(0xc000257c80, 0x11c22d0, 0xc000a67200, 0xc0000b7700)
	/usr/local/go/src/net/http/server.go:2049 +0x44
gitlab.com/hfuss/mux-prometheus/pkg/middleware.(*Instrumentation).Middleware.func1(0x11c2690, 0xc0003c8a80, 0xc0000b7700)
	/go/pkg/mod/gitlab.com/hfuss/mux-prometheus@v0.0.4/pkg/middleware/middleware.go:69 +0xec
net/http.HandlerFunc.ServeHTTP(0xc000a671e0, 0x11c2690, 0xc0003c8a80, 0xc0000b7700)
	/usr/local/go/src/net/http/server.go:2049 +0x44
github.com/gorilla/mux.(*Router).ServeHTTP(0xc0000ee900, 0x11c2690, 0xc0003c8a80, 0xc0000b7500)
	/go/pkg/mod/github.com/gorilla/mux@v1.8.0/mux.go:210 +0xd3
github.com/rs/cors.(*Cors).Handler.func1(0x11c2690, 0xc0003c8a80, 0xc0000b7500)
	/go/pkg/mod/github.com/rs/cors@v1.8.2/cors.go:231 +0x1bb
net/http.HandlerFunc.ServeHTTP(0xc00069b960, 0x11c2690, 0xc0003c8a80, 0xc0000b7500)
	/usr/local/go/src/net/http/server.go:2049 +0x44
net/http.serverHandler.ServeHTTP(0xc0008fb340, 0x11c2690, 0xc0003c8a80, 0xc0000b7500)
	/usr/local/go/src/net/http/server.go:2867 +0xa3
net/http.(*conn).serve(0xc0007c1900, 0x11c5e98, 0xc00012c2c0)
	/usr/local/go/src/net/http/server.go:1932 +0x8cd
created by net/http.(*Server).Serve
	/usr/local/go/src/net/http/server.go:2993 +0x39b
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-01 22:07:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1035" class=".btn">#1035</a>
            </td>
            <td>
                <b>
                    remove legacy namespace query for organizations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                closes #1032 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-01 17:15:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1034" class=".btn">#1034</a>
            </td>
            <td>
                <b>
                    Routes to directly publish blob/JSON data to shared storage (IFPS etc.)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A small extension to external API routes, that let you initiate uploads through your public storage plugin directly.

Unlike with the full on-chain/off-chain orchestration capabilities, no modification is made to the data, and no batching happens.

So this is the feature you would use for example to publish the metadata+binary of an NFT.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-01 17:05:42 +0000 UTC
    </div>
</div>

