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
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/344" class=".btn">#344</a>
            </td>
            <td>
                <b>
                    Add REST request endpoint for ws-wallet connection to ws-identity server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                    ws-wallet open [keyname] [endpoint]
    open connection for keyname to ws-identity server
    provide a websock session endpoint of the fabric app that will use this connection
    i.e., the session can only be used by the IP address of the app that requests it
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-04 16:38:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/339" class=".btn">#339</a>
            </td>
            <td>
                <b>
                    feat (test): Add MD5 checksum test for emission records
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Every time a new emission is recorded, its MD5 digest is computed and stored on the ledger. Then, when the emission is retrieved again, the MD5 digest is re-computed and is checked against the value stored in the ledger. This PR exercises this functionality as a test, by deleting the emission document and then adding a dummy document in its place. This should cause the MD5 digest to be changed, and hence the test should fail.

Closes #188.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 13:04:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/338" class=".btn">#338</a>
            </td>
            <td>
                <b>
                    feat(CI): Add linting and tests for datalock chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds linting and chaincode tests to the existing CI pipeline for the [datalock chaincode](https://github.com/hyperledger-labs/blockchain-carbon-accounting/tree/main/utility-emissions-channel/chaincode/datalock). It uses the same scripts as specified in the Makefile. I have used [this action](https://github.com/marketplace/actions/run-golangci-lint) to setup the golangcli-lint tool.

Closes #306.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-02 19:58:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/337" class=".btn">#337</a>
            </td>
            <td>
                <b>
                    Revision to secure-identity doc edits by opentaps main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Some fixes to the secure-identities docs.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-02 10:54:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/336" class=".btn">#336</a>
            </td>
            <td>
                <b>
                    update documentation for ws-socket and vault security
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                @brioux @Zzocker Can you please review these changes to the documentation based on our call on Monday?

I'm still not too clear where the ws-identity and ws-identity-client are vs each other. Does ws-wallet talk to ws-identity, which then talks through ws-identity-client to Fabric?

A client application that uses web socket identity then somehow incorporate ws-wallet in its UI?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-29 00:15:00 +0000 UTC
    </div>
</div>

