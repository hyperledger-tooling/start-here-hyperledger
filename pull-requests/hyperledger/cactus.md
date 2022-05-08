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
                PR <a href="https://github.com/hyperledger/cactus/pull/2007" class=".btn">#2007</a>
            </td>
            <td>
                <b>
                    fix(security): mitigate Cross-Site Scripting attack (XSS)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Unsanitized input from ```req.params``` flows into ```res.send```, where it is used to render an HTML page returned to the user. This may result in a Cross-Site Scripting attack (XSS)
Signed-off-by: Bhaskar <dev@bhaskar.email>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-06 13:49:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2005" class=".btn">#2005</a>
            </td>
            <td>
                <b>
                    build(lerna): evaluate lerna-lite migration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1890

Signed-off-by: johnhomantaring <john.h.o.mantaring@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-05 19:02:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1999" class=".btn">#1999</a>
            </td>
            <td>
                <b>
                    feat(odap-plugin): backup gateway implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Addition of backup gateways allowed field
* New test where a backup gateway is allowed to replace one that crashed

Signed-off-by: André Augusto <andre.augusto@tecnico.ulisboa.pt>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-02 11:35:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1997" class=".btn">#1997</a>
            </td>
            <td>
                <b>
                    feat(connector-polkadot): polkadot connector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Polkadot</span>
            </td>
            <td>
                This PR adds a long-term effort to adding preliminary support to Substrate-based chains. Most work wonderfully done by @CatarinaPedreira



"The Polkadot Connector provides functionality that enables any permissioned blockchain (as long as it is supported by Hyperledger Cactus) to connect to the Polkadot network and perform monetary transactions to the latter. Besides this, the connector provides methods for these blockchains to deploy and interact with smart contracts in the network.

Our connector in Hyperledger Cactus uses three different API’s to communicate with the Polkadot network: ”@polkadot/api” (which has the base API functionality), ”@polkadot/api-contracts” (which contains the API specific for smart contract interaction) and ”@polkadot/types” (which encompasses specific
Polkadot types)."

Features:
-transact on the network
-read smart contracts
-deploy smart contracts
-read from smart contracts
-endpoints for the features

Future work/limitations
- The integration tests are commented/skipped because we need to add the source code of the smart contracts (metadata, etc) to the repository, such that they can be executed.
- Some of the features could be more extensible/flexible, but again, this is the first version of the connector
- Some endpoints are not fully implemented

Thanks to @petermetz for helping develop the test ledger.

Co-authored-by: CatarinaPedreira <catarina.pedreira@tecnico.ulisboa.pt>
Signed-off-by: Rafael Belchior <rafael.belchior@tecnico.ulisboa.pt>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-02 00:31:12 +0000 UTC
    </div>
</div>

