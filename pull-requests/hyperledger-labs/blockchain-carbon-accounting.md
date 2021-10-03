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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/287" class=".btn">#287</a>
            </td>
            <td>
                <b>
                    signing transaction with key stored in vault server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Added support for signing of fabric tx with vault transit key
- Restructured the typescript_app folder to support writing of unit test along with end-to-end test.
- unit test for blockchain-gateway logic.
- added test coverage.
- moved from tslint to eslint

Steps for running the test can be found inside `README.me` file of the folder.

1. `./start.sh`
2. start hardhat eth node : `cd net-emissions-token-network && npx hardhat node`
3. insert some mock data for testing : `npm run test:setup`
4. Run test with coverage : `npm run coverage`

work remaining for #268   
- use eslint in `blockchain-carbon-accounting/utility-emissions-channel/typescript_app/`

@sichen1234 @udosson 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-27 17:22:04 +0000 UTC
    </div>
</div>

