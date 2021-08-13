---
layout: default
title: firefly-cli
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly-cli
---

# firefly-cli <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly-cli){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/81" class=".btn">#81</a>
            </td>
            <td>
                <b>
                    Minor enhancements to contract/REST calls
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These are the commits originally in #79 but not specifically related to tokens.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-13 15:08:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/79" class=".btn">#79</a>
            </td>
            <td>
                <b>
                    Deploy ERC1155 contract and tokens microservice
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Tokens Docker will need to be deployed before this can work, which implies a dependency on https://github.com/hyperledger-labs/firefly-tokens-erc1155/pull/3. **Edit:** this pre-req is now [done](https://github.com/hyperledger-labs/firefly-tokens-erc1155/pkgs/container/firefly-tokens-erc1155).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-12 12:45:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/78" class=".btn">#78</a>
            </td>
            <td>
                <b>
                    Add command line flag for customizing provider
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a start for support for several different blockchain providers. This just adds the command line interface options to specify which provider you want. `geth` is the only valid option currently. It's also written to the `stack.json` now so future versions of the CLI should be able to read `stack.json` files created with this code and be able to load that stack.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-11 20:16:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/77" class=".btn">#77</a>
            </td>
            <td>
                <b>
                    Add files for consistent repo structure
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
        Created At 2021-08-10 17:29:44 +0000 UTC
    </div>
</div>

