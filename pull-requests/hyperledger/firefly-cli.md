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
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/165" class=".btn">#165</a>
            </td>
            <td>
                <b>
                    Unique topics for multiple connectors against same ethconnect
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Few changes here:

1. We already set the topic to be unique per node in the CLI, but we don't do the same for token connectors.
    - This means if you request use of multiple token connectors of the same type, or are using the CLI to aid deployment against a remote EthConnect (such as in Kaleido), you can't be sure to have unique topics.
2. Log the API call that failed, when logging errors
3. Allow a `--contract-address` to be specified at `init`, which bypasses the contract deploy step at `start`. This can be combined with `--core-config` to use a remotely hosted EthConnect with a separately deployed contract (for example Kaleido smart contract management)
4. Remove registration of a REST API for the FireFly smart contract across all EthConnect instances, in all cases. This is no longer required.
5. Do deployment of the FireFly contract in the same way that all other deployment is now done (without any use of the `/abis` REST API functionality in FireFly)
    - Partially addresses a `Deprecated` function usage in the code - ERC-1155 still has debt to address
    - Requires https://github.com/hyperledger/firefly/pull/624
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-23 18:35:24 +0000 UTC
    </div>
</div>

