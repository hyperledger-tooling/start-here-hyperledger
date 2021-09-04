---
layout: default
title: firefly-tokens-erc1155
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly-tokens-erc1155
---

# firefly-tokens-erc1155 <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly-tokens-erc1155){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-tokens-erc1155/pull/20" class=".btn">#20</a>
            </td>
            <td>
                <b>
                    Add curl to docker image for healthchecks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `curl` is necessary to have in the Docker image so that the container can run its own health checks. Custom health checks are required so that the FireFly Core does not start up until after the tokens connector is already listening for WebSocket connections.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-01 23:54:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-tokens-erc1155/pull/19" class=".btn">#19</a>
            </td>
            <td>
                <b>
                    Add arbitrary "data" input to all POST APIs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The /pool API will also be migrated from taking separate parameters
for namespace/name/clientId and will instead require clients to pack
relevant info into "data".
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-01 20:17:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-tokens-erc1155/pull/18" class=".btn">#18</a>
            </td>
            <td>
                <b>
                    Allow overriding request ID
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
        Created At 2021-08-31 14:44:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-tokens-erc1155/pull/17" class=".btn">#17</a>
            </td>
            <td>
                <b>
                    Remove "author" field from token-pool event
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Can be merged after https://github.com/hyperledger-labs/firefly/pull/177
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-30 20:16:35 +0000 UTC
    </div>
</div>

