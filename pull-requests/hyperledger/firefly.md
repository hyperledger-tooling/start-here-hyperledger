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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1033" class=".btn">#1033</a>
            </td>
            <td>
                <b>
                    Update manifest for v1.1.0-rc.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Updates EthConnect, EVMConnect, and FireFly Signer
- Fixes the tests for EVMConnect:
   - They were actually running EthConnect (missing env var)
   - The archive logs weren't distinguished uniquely
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-31 21:50:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1031" class=".btn">#1031</a>
            </td>
            <td>
                <b>
                    update event docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                in a chain with #1028 

not currently published on my github pages due to hosting another doc changes. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-31 20:37:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1028" class=".btn">#1028</a>
            </td>
            <td>
                <b>
                    Add status information for subscriptions & contract listeners
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                 If the `fetchstatus` query param is supplied when querying `subscriptions` or `listeners` by ID, firefly will return additional status information, if it is available.

### Contract listeners:
FF environments connected to evm connectors will return listener checkpoint formation under the `status` key.

Example query: `http://localhost:5000/api/v1/namespaces/default/contracts/listeners/92e3bc0c-3c3f-455b-81d3-4124a0270b1d?fetchstatus`

Response:
```
{
    "id": "92e3bc0c-3c3f-455b-81d3-4124a0270b1d",
    "interface": {
        "id": "30775d45-61af-4f76-9d35-69b5d8ffbf42"
    },
    "namespace": "default",
    "name": "0182f410-a686-79ed-23a5-ac8c62acbf51",
    "backendId": "0182f410-a686-79ed-23a5-ac8c62acbf51",
    "location": {
        "address": "0x62d365e68fc55845ba904acef688feba7a598c9c"
    },
    "created": "2022-08-31T13:21:48.1687995Z",
    "event": {
        "name": "Changed",
        "description": "",
        "params": [
            {
                "name": "from",
                "schema": {
                    "type": "string",
                    "details": {
                        "type": "address",
                        "internalType": "address",
                        "indexed": true
                    }
                }
            },
            {
                "name": "value",
                "schema": {
                    "type": "integer",
                    "details": {
                        "type": "uint256",
                        "internalType": "uint256"
                    }
                }
            }
        ]
    },
    "signature": "Changed(address,uint256)",
    "topic": "bsc",
    "options": {
        "firstEvent": "oldest"
    },
    "status": {
        "checkpoint": {
            "block": 0,
            "transactionIndex": -1,
            "logIndex": -1
        }
    }
}
```

### Subscriptions
Subscriptions will provide offset information if available

Example Query: `http://localhost:5000/api/v1/namespaces/default/subscriptions/32cddc74-cc1a-4493-b376-45781e2d8d35?fetchstatus`

Response:
```
{
    "id": "32cddc74-cc1a-4493-b376-45781e2d8d35",
    "namespace": "default",
    "name": "simple-storage",
    "transport": "websockets",
    "filter": {
        "message": {},
        "transaction": {},
        "blockchainevent": {}
    },
    "options": {
        "firstEvent": "-1",
        "withData": false
    },
    "created": "2022-08-31T17:13:04.295134Z",
    "updated": null,
    "status": {
        "currentOffset": 31
    }
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-31 17:53:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1027" class=".btn">#1027</a>
            </td>
            <td>
                <b>
                    Use advisory lock instead of exclusive lock on events table
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Advisory locks are identified with a 64-bit integer, so I've put in place a
rudimentary mapping from namespace names to a (probably) unique int64.
This should ensure consistent ordering for the writes to the events table
within a particular namespace, without blocking reads or other namespaces.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-31 17:39:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1026" class=".btn">#1026</a>
            </td>
            <td>
                <b>
                    Allow null signer on transfers to account for non-archive indexing of historical transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1023 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-31 13:21:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1022" class=".btn">#1022</a>
            </td>
            <td>
                <b>
                    [identity-tutorial] identity tutorial
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Tutorial to guide user through creating a Custom Identity in FireFly.

References https://github.com/hyperledger/firefly/issues/621
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 19:10:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1021" class=".btn">#1021</a>
            </td>
            <td>
                <b>
                    Allow any plugin to terminate the system on a bad event
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Terminating the system is better than leaving it up in a crippled state.

Closes #957
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 18:52:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1019" class=".btn">#1019</a>
            </td>
            <td>
                <b>
                    Clean up event manager unit tests
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
        Created At 2022-08-30 17:25:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1018" class=".btn">#1018</a>
            </td>
            <td>
                <b>
                    add another account for fabric
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Anna Jackson <anna.jackson@kaleido.io>

Fixes #1011 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 09:17:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1017" class=".btn">#1017</a>
            </td>
            <td>
                <b>
                    adds `fetchreference` to /events/:id
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When provided, firefly will include the record that the `ref` field references in the response body.

closes #1016 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 02:33:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1015" class=".btn">#1015</a>
            </td>
            <td>
                <b>
                    Add firefly-signer to manifest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-29 19:21:38 +0000 UTC
    </div>
</div>

