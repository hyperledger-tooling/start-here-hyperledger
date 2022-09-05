---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2155" class=".btn">#2155</a>
            </td>
            <td>
                <b>
                    build(openapi): upgrade openapi-generator version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Commit to be reviewed
------------------------------------

build(openapi): upgrade openapi-generator version   


    Primary Changes
    ---------------
    1. Updated openapitools.json file   
    
    Secondary Changes
    ----------------
    1. Some of the generated kotlin files are updated with the new code

Signed-off-by: jagpreetsinghsasan <jagpreet.singh.sasan@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-05 06:29:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2154" class=".btn">#2154</a>
            </td>
            <td>
                <b>
                    feat(cbdc-bridging-app): refactor ODAP plugin implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * From now there is one PluginOdapGateway that must be extended by any implementation of a gateway
* This commit intends to decouple the gateway implementation from any ledger
* There is still a Gateway implementation for Fabric and Besu
* The asset being transferred is now in the scope of the request and not the gateway, which makes possible the transfer of multiple assets without having to create new gateways

closes #2132 

Signed-off-by: André Augusto <andre.augusto@tecnico.ulisboa.pt>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-01 16:06:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2153" class=".btn">#2153</a>
            </td>
            <td>
                <b>
                    feat(connector-iroha2): add support for Iroha V2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                - Add new Iroha V2 cactus connector.
- Two OpenAPI endpoints are implemented: `transact` and `query`. Both endpoints support
  critical subset of instructions and queries supported by the upstream javascript iroha sdk.
- One SocketIO endpoint can be used to monitor new blocks from the ledger.
- New connector can be used through a verifier-client interface.
- All added functions are tested in functional test suites and documented.
- Added execution of Iroha2 tests to the CI.

Additional notes:
- Connector doesn't work well with cactus module system, the issue has been reported and described
  in README. PR is not merge-ready until this is fixed (the CI should fail now).
- Iroha V2 javascript packages are not available on official npm yet, had to include `.npmrc` with
  private npm address. I'm not sure if there's ETA of delivering these through NPM, so it might be
  necessary to commit it after all.

Closes #2138
Depends on #2140

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-31 14:59:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2152" class=".btn">#2152</a>
            </td>
            <td>
                <b>
                    fix(cactus-example-electricity-trade): enable tsconfig strict flag an…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …d fix all the warnings

Fixed all warnings when strict flag is enabled

Closes: #2144

Signed-off-by: Tomasz Awramski <tomasz.awramski@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 09:29:13 +0000 UTC
    </div>
</div>

