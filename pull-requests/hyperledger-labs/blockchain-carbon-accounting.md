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
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/387" class=".btn">#387</a>
            </td>
            <td>
                <b>
                    Updates to CarbonTraker NFT contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit introduces major changes to the CarbonTracker contract
It also updates carbon-tracker.md describing how the CarbonTracker contract works in more detail
This includes mathmatical forumlae for how carbon intensities and emissions are calculated across tracker NFTs
and a diagram with a basic fuel supply chain example

Signed-off-by: brioux <Bertrand.rioux@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-13 10:43:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/384" class=".btn">#384</a>
            </td>
            <td>
                <b>
                    Initial UI for carbon tracker 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Assigning roles is not working yet but you can issue tokens and see them.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-11 00:56:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/382" class=".btn">#382</a>
            </td>
            <td>
                <b>
                    feat(scripts): Add script for packaging and installing chaincode locally
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added a script that executes the Fabric chaincode lifecycle locally instead of using the chaincode from an external container, so that changes in the chaincode may be tested out quickly. Now the chaincode is installed directly on the peer itself, and the created dev-peer containers may be used for easily debugging chaincode.

Closes #376. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-10 09:08:24 +0000 UTC
    </div>
</div>

