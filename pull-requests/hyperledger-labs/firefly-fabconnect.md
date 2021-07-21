---
layout: default
title: firefly-fabconnect
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly-fabconnect
---

# firefly-fabconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly-fabconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-fabconnect/pull/13" class=".btn">#13</a>
            </td>
            <td>
                <b>
                    Added Makefile, linter and fixed linting errors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jim Zhang <jim.zhang@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-20 18:31:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-fabconnect/pull/12" class=".btn">#12</a>
            </td>
            <td>
                <b>
                    Foundation implementation and framework (missing submanager, idmanager and tests)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `internal/conf`: configuration objects for all packages
`internal/errors`: error messages and templates
`internal/fabric`: RPC client and objects that interact with the Fabric nodes via `fabric-sdk-go`
`internal/kafka`: Kafka client via `samara`
`internal/kvstore`: abstract interface for LevelDB based key-value store
`internal/messages`: interfaces and methods for all messages submitted to fabconnect
`internal/rest`: REST server and router
`internal/rest/async`: async request handler and receipt store
`initernal/rest/sync`: sync request handler
`internal/rest/receipt`: receipt store incl. 3 implementations (mongo, leveldb, memory)
`internal/tx`: transaction processor and object
`internal/ws`: websocket server
`cmd`: command definition for launching the REST server

Components that are still missing and to be implemented in a followup PR:
- signing identity management: `internal/identiey`
- event stream management: `internal/eventstream`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-19 17:46:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-fabconnect/pull/8" class=".btn">#8</a>
            </td>
            <td>
                <b>
                    Updated README license chapter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adding chapter License to README.md in a consistent format with other hyperledger-labs projects.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-15 15:55:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-fabconnect/pull/7" class=".btn">#7</a>
            </td>
            <td>
                <b>
                    Add CODEOWNERS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-15 15:23:54 +0000 UTC
    </div>
</div>

