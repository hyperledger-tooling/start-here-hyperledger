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
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/202" class=".btn">#202</a>
            </td>
            <td>
                <b>
                    Skip creation of IPFS and DX when multiparty is disabled
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This will reduce the number of docker containers needed to run when multiparty mode has been disabled. Previously, IPFS and DX were there just sitting idle.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-16 15:00:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/201" class=".btn">#201</a>
            </td>
            <td>
                <b>
                    Make goreleaser honor pre-release tags
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-15 16:17:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/200" class=".btn">#200</a>
            </td>
            <td>
                <b>
                    Fix deletion of pre-v1.1 stacks, and cleanup redundant FFTM option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Fixed remote-rpc node provider
* Fixed removing stacks created with previous CLI version
* Removed fftm related code

Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-15 14:33:29 +0000 UTC
    </div>
</div>

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

