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
                PR <a href="https://github.com/hyperledger/firefly/pull/279" class=".btn">#279</a>
            </td>
            <td>
                <b>
                    Add EventTypeTransferOpFailed for token transfer operations that fail
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This basically works, but I'd like to vet the behavior since there are some slight inconsistencies.

When you submit a transfer request, you'll (now) ultimately receive one of two events in response:
* `EventTypeTransferConfirmed` if transfer is confirmed -> references the transfer's `LocalID` so you can look up the transfer
* `EventTypeTransferOpFailed` if transfer fails -> references the operation's `ID` so you can look up the failed operation (there is no transfer object created in this case)

Even though this means the events are a bit asymmetric, I can't come up with a more sensible way to do it.

However, when submitting a transfer with `confirm=true`, the sync-async bridge tracks a _single_ ID which will ultimately resolve in success or failure. I've chosen the transfer's `LocalID`, but that means there's an additional step in the case of `EventTypeTransferOpFailed`, for sync-async to map the operation `ID` to the transfer `LocalID`. This also meant extracting some helpers to `txcommon` (for lack of a better place to put them).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-21 01:06:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/278" class=".btn">#278</a>
            </td>
            <td>
                <b>
                    tokens-by-id getTokenPoolByNameOrID() and getTokenTransfersByID()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                To support the new [Tokens Page in the UI](https://github.com/hyperledger/firefly-ui/issues/65), an endpoint to get token pools by name or ID and to get token transfers by ID is needed.

```GET /namespaces/<namespace>/tokens/pools/{nameOrID}``` returns all token pools with specified name or ID
```GET /namespaces/<namespace>/tokens/transfers/{transferID}``` returns token transfer with specified ID
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-21 01:03:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/277" class=".btn">#277</a>
            </td>
            <td>
                <b>
                    introduce FFTime.Time()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                 - Converts FFTime -> Time
 - some misc. changes my linter pointed out
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 20:25:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/276" class=".btn">#276</a>
            </td>
            <td>
                <b>
                    Add extra columns to token tables for UI support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Extra columns desired in support of https://github.com/hyperledger/firefly-ui/issues/65
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 18:06:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/275" class=".btn">#275</a>
            </td>
            <td>
                <b>
                    New GET routes for tokens
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Reviewed separately on a branch:
* https://github.com/kaleido-io/firefly/pull/33
* https://github.com/kaleido-io/firefly/pull/34
* https://github.com/kaleido-io/firefly/pull/35
* https://github.com/kaleido-io/firefly/pull/36

Squashed together here for upstreaming.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 16:53:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/274" class=".btn">#274</a>
            </td>
            <td>
                <b>
                    Additional E2E coverage for tokens
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Ensure that testing covers fungible/non-fungible, sync/async, and with/without
message data.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 16:32:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/273" class=".btn">#273</a>
            </td>
            <td>
                <b>
                    Group token database calls into RunAsGroup wherever possible
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
        Created At 2021-10-20 16:30:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/270" class=".btn">#270</a>
            </td>
            <td>
                <b>
                    Allow nested RunAsGroup calls
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If a transaction is already started, it is reused.

This allows code to be reused in a fashion where it may need to start a transaction, or may be called from
within an already-started transaction (useful for operations that span multiple packages, such as the
ongoing work on token transfers with associated messages).

It does introduce a new constraint for database implementations (noted in the database plugin definition).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 14:47:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/268" class=".btn">#268</a>
            </td>
            <td>
                <b>
                    Split asset manager into multiple files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                No code changes - just splitting up files.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 14:18:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/267" class=".btn">#267</a>
            </td>
            <td>
                <b>
                    Adjust version for firefly-tokens-erc1155
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Moving to a pre-release versioning pattern to avoid incrementing version numbers
too frequently.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 14:16:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/266" class=".btn">#266</a>
            </td>
            <td>
                <b>
                    Use firefly_e2e instead of firefly-e2e for container names
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fits with other FireFly naming conventions and makes highlighting in terminal
a bit easier.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-19 18:22:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/264" class=".btn">#264</a>
            </td>
            <td>
                <b>
                    Do not use tokenIndex in E2E test for fungible tokens
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Pulls in the behavior from https://github.com/hyperledger/firefly-tokens-erc1155/pull/35 and adjusts E2E test to match.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-19 17:27:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/262" class=".btn">#262</a>
            </td>
            <td>
                <b>
                    Do not allow UUIDs to be used as names
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
        Created At 2021-10-18 19:03:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/261" class=".btn">#261</a>
            </td>
            <td>
                <b>
                    Added more tests to the Fabric plugin for 100% coverage
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
        Created At 2021-10-18 15:51:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/260" class=".btn">#260</a>
            </td>
            <td>
                <b>
                    Move e2e to new routes, and add private/broadcast strong datatype tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                New E2E tests created as part of a recreate for #257, which turned out to be working as designed (due to a quirk of the JSON Schema syntax allowing additional properties by default).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-16 20:46:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/258" class=".btn">#258</a>
            </td>
            <td>
                <b>
                    Fix logic for transfer+message with waitConfirm=true
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Part of #218.

Includes a new MessageSender interface that is used by asset manager, broadcast manager, private messaging,
and sync-async bridge. This allows cleaner tracking of the progress of resolving and sending a message, and
injection of hooks at particular spots in the flow (which is needed here to dispatch the transfer and message in
a specific order).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-15 19:08:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/256" class=".btn">#256</a>
            </td>
            <td>
                <b>
                    Re-subscribe if the instance path changes 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                For newly created environments, this PR adds a 16 character unique suffix to the ethconnect subscription names it creates, using the instance path from the config at the time the sub is created. This means that if the contract instance changes in the future, we will re-subscribe to the new contract.

Note I also saw this issue  in a test run on my machine, and added a change to read this config once on HTTP server startup.

```
fatal error: concurrent map read and map write

goroutine 150 [running]:
runtime.throw(0x496ca08, 0x21)
        /usr/local/Cellar/go/1.16.4/libexec/src/runtime/panic.go:1117 +0x72 fp=0xc000121c48 sp=0xc000121c18 pc=0x403aa12
runtime.mapaccess2_faststr(0x488eba0, 0xc0005eb3b0, 0xc0000301f8, 0x3, 0x0, 0x0)
        /usr/local/Cellar/go/1.16.4/libexec/src/runtime/map_faststr.go:116 +0x4a5 fp=0xc000121cb8 sp=0xc000121c48 pc=0x4016fe5
github.com/spf13/viper.(*Viper).searchMap(0xc0002dad80, 0xc0005eb3b0, 0xc0003bc300, 0x2, 0x2, 0x0, 0x0)
        /Users/peterbroadhurst/dev/go/pkg/mod/github.com/spf13/viper@v1.8.1/viper.go:568 +0x5f fp=0xc000121d00 sp=0xc000121cb8 pc=0x445665f
github.com/spf13/viper.(*Viper).find(0xc0002dad80, 0xc0000301f8, 0x13, 0x1, 0xc000121e70, 0x2)
        /Users/peterbroadhurst/dev/go/pkg/mod/github.com/spf13/viper@v1.8.1/viper.go:1218 +0x40e fp=0xc000121e10 sp=0xc000121d00 pc=0x445842e
github.com/spf13/viper.(*Viper).Get(0xc0002dad80, 0x4960281, 0x13, 0x43e8965, 0x4e65370)
        /Users/peterbroadhurst/dev/go/pkg/mod/github.com/spf13/viper@v1.8.1/viper.go:798 +0x85 fp=0xc000121ea8 sp=0xc000121e10 pc=0x4457425
github.com/spf13/viper.(*Viper).GetString(0xc0002dad80, 0x4960281, 0x13, 0x4960281, 0x13)
        /Users/peterbroadhurst/dev/go/pkg/mod/github.com/spf13/viper@v1.8.1/viper.go:865 +0x3f fp=0xc000121ee8 sp=0xc000121ea8 pc=0x4457c3f
github.com/spf13/viper.GetString(...)
        /Users/peterbroadhurst/dev/go/pkg/mod/github.com/spf13/viper@v1.8.1/viper.go:862
github.com/hyperledger/firefly/internal/config.(*configPrefix).GetDuration(0x4e318f0, 0x4960281, 0x13, 0x2c)
        /Users/peterbroadhurst/dev/photic/firefly/internal/config/config.go:551 +0x69 fp=0xc000121f20 sp=0xc000121ee8 pc=0x445cdc9
github.com/hyperledger/firefly/internal/config.GetDuration(...)
        /Users/peterbroadhurst/dev/photic/firefly/internal/config/config.go:548
github.com/hyperledger/firefly/internal/apiserver.(*httpServer).serveHTTP.func1(0x4a4c2d8, 0xc000021ac0, 0xc0001c4fc0, 0xc00061c660)
        /Users/peterbroadhurst/dev/photic/firefly/internal/apiserver/http_server.go:175 +0x179 fp=0xc000121fc0 sp=0xc000121f20 pc=0x46c4279
runtime.goexit()
        /usr/local/Cellar/go/1.16.4/libexec/src/runtime/asm_amd64.s:1371 +0x1 fp=0xc000121fc8 sp=0xc000121fc0 pc=0x4073f21
created by github.com/hyperledger/firefly/internal/apiserver.(*httpServer).serveHTTP
        /Users/peterbroadhurst/dev/photic/firefly/internal/apiserver/http_server.go:171 +0x98
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-15 03:44:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/255" class=".btn">#255</a>
            </td>
            <td>
                <b>
                    Use a single mutex, as there is a single keys map
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #254 

The problem in the stack, is that we were creating separate mutexes for locking, but passing the same root map down in the config objects. So this cleans up the code to a single mutex, and makes it more clear there's a single root map.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-15 00:34:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/253" class=".btn">#253</a>
            </td>
            <td>
                <b>
                    Reduce I/O load of test runs by using memory DB
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Now we have SQLConfMaxConnections, the previous reasons we needed a real filesystem backing the SQL tests has been removed, and it seems to significantly slow down the test to have a full filesystem on I/O throttled build servers.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-14 21:48:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/251" class=".btn">#251</a>
            </td>
            <td>
                <b>
                    Update E2E script to use manifest file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Opening this as a draft PR for now. It will fail until we merge and tag/release https://github.com/hyperledger/firefly-cli/pull/112. This uses the new CLI flag when running E2E tests to ensure that the images tested, are the specific ones listed in the `manifest.json` for the FireFly Core commit being tested.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-14 14:43:51 +0000 UTC
    </div>
</div>

