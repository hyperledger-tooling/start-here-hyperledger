---
layout: default
title: blockchain-carbon-accounting
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-carbon-accounting
---

# blockchain-carbon-accounting <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-carbon-accounting){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/295" class=".btn">#295</a>
            </td>
            <td>
                <b>
                    enh(chaincode): Migrate from TSLint to ESLint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Migrated the [chaincode/typescript](https://github.com/hyperledger-labs/blockchain-carbon-accounting/tree/main/utility-emissions-channel/chaincode/typescript) directory from TSLint to ESLint. Added the same ESLint and Prettier configuration as for the [typescript_app](https://github.com/hyperledger-labs/blockchain-carbon-accounting/tree/main/utility-emissions-channel/typescript_app) directory. Also added in the `lint` and `lint:fix` scripts.

Fixes #268. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-05 11:28:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/293" class=".btn">#293</a>
            </td>
            <td>
                <b>
                    Web socket identities
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR integrates web-socket secure identities into the utility-emissions-channel app
It uses the ws-wallet package to generate key pairs on an external clients device and identity packages to connect it to the fabric application (using cactus-plugin-ledger-connector-fabric).
The src for both packages are included in the secure-identities directory
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-05 05:24:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/290" class=".btn">#290</a>
            </td>
            <td>
                <b>
                    lock Fabric records while Cactus transaction with Ethereum is in place
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - DataLock chaincode for locking fabric data, present on `utilityemissions` chaincode
- `recordAuditedEmissionsToken` endpoint of `typescript_app` uses, it to lock emissions record while minting of token is taking place on Ethereum network.

close #204 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-02 17:56:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/289" class=".btn">#289</a>
            </td>
            <td>
                <b>
                    Mentorship cactus integration
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
        Created At 2021-10-02 14:27:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/288" class=".btn">#288</a>
            </td>
            <td>
                <b>
                    small ui fix to voluntary carbon offsets directory
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
        Created At 2021-09-28 17:43:32 +0000 UTC
    </div>
</div>

