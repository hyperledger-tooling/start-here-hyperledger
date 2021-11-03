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

