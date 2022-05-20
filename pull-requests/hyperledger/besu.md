---
layout: default
title: besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3834" class=".btn">#3834</a>
            </td>
            <td>
                <b>
                    3619 unify rpc ports
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

- Introduces new JsonRPCService that handles both http and websockets
- Removes websocket specific configs
- renames WebSocketRequestHandler to WebSocketMessageHandler to be more in line with websocket semantics.

## Fixed Issue(s)

fixes #3619 

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-13 16:07:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3832" class=".btn">#3832</a>
            </td>
            <td>
                <b>
                    Reduce EVM library dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Reduce the runtime dependencies of the EVM module by moving a
class used by a single class out of util to the owned module (QosTimer)
and them removing un-used dependencies from EVM and dependant modules.

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-13 02:33:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3831" class=".btn">#3831</a>
            </td>
            <td>
                <b>
                    Added Metrics for number of open RPC connections[#3781]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dev experience</span>
            </td>
            <td>
                Added Metrics for number of open RPC connections - besu_rpc_active_http_connection_count, besu_rpc_active_ws_connection_count

Signed-off-by: Sharad Gulati sharad.develop@gmail.com

## Fixed Issue(s)
fixes #3781 

## Documentation

- [ x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
Documentation might need to be updated due to additional metrics

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-13 01:55:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3830" class=".btn">#3830</a>
            </td>
            <td>
                <b>
                    quorum ATs can run on medium executor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Change quorum ATs (nightly) from XL to medium executor. 

The job ran successfully on medium executor https://app.circleci.com/pipelines/github/hyperledger/besu/14864/workflows/e1c2b5d0-44b1-45aa-a5c6-f46eeca7f4bc/jobs/85796

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-13 01:41:24 +0000 UTC
    </div>
</div>

