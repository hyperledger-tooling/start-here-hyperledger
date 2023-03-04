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
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/67" class=".btn">#67</a>
            </td>
            <td>
                <b>
                    Nil check on confirmations for reset
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes this on reset of a listener:
```
[2023-03-03T00:19:19.383Z] ERROR evmconnect: RPC[000004742] <-- ERROR: FF22012: Backend RPC request failed: Post "http://geth:8545/": context canceled eventstream=0186a4be-434c-1a8c-f19a-b2bc725d3378
[2023-03-03T00:19:19.384Z]  WARN evmconnect: Error uninstalling filter '0xc0006e0390': FF22012: Backend RPC request failed: Post "http://geth:8545/": context canceled eventstream=0186a4be-434c-1a8c-f19a-b2bc725d3378
2023/03/03 00:19:19 http: panic serving 127.0.0.1:55092: runtime error: invalid memory address or nil pointer dereference
goroutine 26602 [running]:
net/http.(*conn).serve.func1()
	/usr/local/go/src/net/http/server.go:1825 +0xbf
panic({0xc05e80, 0x13b0ed0})
	/usr/local/go/src/runtime/panic.go:844 +0x258
github.com/hyperledger/firefly-transaction-manager/internal/events.(*eventStream).Stop(0xc0003c6500, {0xee7cf0, 0xc0008de660})
	/go/pkg/mod/github.com/hyperledger/firefly-transaction-manager@v1.2.3/internal/events/eventstream.go:563 +0x1a9
github.com/hyperledger/firefly-transaction-manager/internal/events.(*eventStream).AddOrUpdateListener(0xbfa9c0?, {0xee7cf0, 0xc0008de660}, 0xc000351ee0, 0xbc4a40?, 0x1)
	/go/pkg/mod/github.com/hyperledger/firefly-transaction-manager@v1.2.3/internal/events/eventstream.go:378 +0x135
github.com/hyperledger/firefly-transaction-manager/pkg/fftm.(*manager).createOrUpdateListener(0xc000148000, {0xee7cf0, 0xc0008de660}, 0xc0000ecb93?, 0xc00079af00, 0xc2?)
	/go/pkg/mod/github.com/hyperledger/firefly-transaction-manager@v1.2.3/pkg/fftm/stream_management.go:230 +0x183
github.com/hyperledger/firefly-transaction-manager/pkg/fftm.(*manager).updateExistingListener(0xbff460?, {0xee7cf0, 0xc0008de660}, {0xc0000ecb93?, 0x4000a165b8?}, {0xc0000ecbc2?, 0xc000050800?}, 0xc00079af00, 0x0?)
	/go/pkg/mod/github.com/hyperledger/firefly-transaction-manager@v1.2.3/pkg/fftm/stream_management.go:214 +0x8e
github.com/hyperledger/firefly-transaction-manager/pkg/fftm.glob..func23.3(0xc000807680)
	/go/pkg/mod/github.com/hyperledger/firefly-transaction-manager@v1.2.3/pkg/fftm/route_post_eventstream_listener_reset.go:42 +0xee
github.com/hyperledger/firefly-common/pkg/ffapi.(*HandlerFactory).RouteHandler.func1({0xee74f0, 0xc0002a0380}, 0xc0006fd500)
	/go/pkg/mod/github.com/hyperledger/firefly-common@v1.2.1/pkg/ffapi/handler.go:179 +0x64e
github.com/hyperledger/firefly-common/pkg/ffapi.(*HandlerFactory).APIWrapper.func1({0xee74f0?, 0xc0002a0380}, 0xc0006fd400)
	/go/pkg/mod/github.com/hyperledger/firefly-common@v1.2.1/pkg/ffapi/handler.go:285 +0x4a7
net/http.HandlerFunc.ServeHTTP(0xc0006fd300?, {0xee74f0?, 0xc0002a0380?}, 0x78000000004d0b60?)
	/usr/local/go/src/net/http/server.go:2084 +0x2f
github.com/gorilla/mux.(*Router).ServeHTTP(0xc000146000, {0xee74f0, 0xc0002a0380}, 0xc0006fd200)
	/go/pkg/mod/github.com/gorilla/mux@v1.8.0/mux.go:210 +0x1cf
github.com/rs/cors.(*Cors).Handler.func1({0xee74f0, 0xc0002a0380}, 0xc0006fd200)
	/go/pkg/mod/github.com/rs/cors@v1.8.2/cors.go:231 +0x1c4
net/http.HandlerFunc.ServeHTTP(0x0?, {0xee74f0?, 0xc0002a0380?}, 0x40ef45?)
	/usr/local/go/src/net/http/server.go:2084 +0x2f
net/http.serverHandler.ServeHTTP({0xee58b0?}, {0xee74f0, 0xc0002a0380}, 0xc0006fd200)
	/usr/local/go/src/net/http/server.go:2916 +0x43b
net/http.(*conn).serve(0xc00051c640, {0xee7cf0, 0xc0008de330})
	/usr/local/go/src/net/http/server.go:1966 +0x5d7
created by net/http.(*Server).Serve
	/usr/local/go/src/net/http/server.go:3071 +0x4db
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-03 00:44:14 +0000 UTC
    </div>
</div>

