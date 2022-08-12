---
layout: default
title: firefly-cli
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-cli
---

# firefly-cli <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-cli){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/199" class=".btn">#199</a>
            </td>
            <td>
                <b>
                    Add support for evmconnect
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds support for evmconnect and chosing between it and ethconnect (still the default) with the new ` -c, --blockchain-connector` flag.

It also moves logging related items to a context which is passed throughout the CLI code, and it creates a new interface for blockchain connectors.

Right now a BlockchainProvider creates the blockchain connector instance, but I feel like it should probably be the other way around in the future. That's a refactor for another day, as it is quite a disruptive code change, with no tangible benefit to the end user (only code maintainability).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-10 14:07:44 +0000 UTC
    </div>
</div>

