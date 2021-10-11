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
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/304" class=".btn">#304</a>
            </td>
            <td>
                <b>
                    Add lint checks to CI pipeline
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                PR #297 fixed the linting in the `chaincode/typescript` and `typescript_app` directories as per the ESLint and Prettier configuration. This PR will run the linting checks for both of these directories in separate jobs as part of the existing CI pipeline on GitHub actions, so that code style and formatting is enforced with every PR.

Fixes #221 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-11 08:40:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/303" class=".btn">#303</a>
            </td>
            <td>
                <b>
                    utility bills do not cover a year so this is more typical
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Si Chen <sichen@opensourcetrategies.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 17:36:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/299" class=".btn">#299</a>
            </td>
            <td>
                <b>
                    small documentation fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Si Chen <sichen@opensourcetrategies.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 17:08:43 +0000 UTC
    </div>
</div>

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
                    Support for FabricSigningCredentialType.WsX509
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

