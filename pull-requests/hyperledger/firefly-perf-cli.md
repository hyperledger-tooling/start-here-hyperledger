---
layout: default
title: firefly-perf-cli
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-perf-cli
---

# firefly-perf-cli <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-perf-cli){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-perf-cli/pull/49" class=".btn">#49</a>
            </td>
            <td>
                <b>
                    Add options to allow node(s) to be configured without a local FireFly stack
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This closes https://github.com/hyperledger/firefly-perf-cli/issues/48 adding features that make it easier to run the performance CLI against an arbitrary FireFly endpoint.

It also adds various configuration options to give more tuning options in the `instances.yaml` file:

- Name of the FireFly namespace to submit API calls to: `fireflyNamespace`
- Option to add a prefix to all API calls in case the FireFly endpoint has a gateway in front of it: `apiPrefix`
- Maximum time each action should take to avoid hard coded 60s limits: `maxTimePerAction`
- Option for token mint workers to skip waiting for the mint to be confirmed before doing the next mint: `skipMintConfirmations`
- The name of the token connector to use when creating a token pool: `poolConnectorName`
- Configure whether the token pool contract supports data: `supportsData`
- Configure whether the token pool contract supports URIs: `supportsURI`
- Choose the recipient of token mints: `mintRecipient`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-09 14:17:13 +0000 UTC
    </div>
</div>

