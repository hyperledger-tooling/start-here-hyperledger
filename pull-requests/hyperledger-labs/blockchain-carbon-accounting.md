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
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/297" class=".btn">#297</a>
            </td>
            <td>
                <b>
                    fix(chaincode): fix linting as per ESLint configuration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixed the linting as per the ESLint configuration added in by #295. The output of running `npm run lint` is given below.
![image](https://user-images.githubusercontent.com/51477130/136084508-d907676d-de79-4acd-81e1-d7f9c1f608df.png)
No errors are thrown after running the lint script.

Fixes #296.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-05 18:49:18 +0000 UTC
    </div>
</div>

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

