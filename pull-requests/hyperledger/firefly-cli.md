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
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/250" class=".btn">#250</a>
            </td>
            <td>
                <b>
                    Fix Goreleaser Job
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves https://github.com/hyperledger/firefly-cli/issues/249

Also updates the goreleaser action to v4
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 20:51:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/248" class=".btn">#248</a>
            </td>
            <td>
                <b>
                    Add an option '--remote-node-deploy' to treat remote nodes like local nodes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Specifically, this option allows the `ff init` command to be run with `-n remote-rpc` without specifying `--contract-address`, something which was previously not supported.

By default the CLI will behave the same as previous versions. However, setting the new `--remote-node-deploy=true` option will perform both the deployment of the FireFly contract, and the identity/org registration. Effectively this option is a way of saying "the remote node is a free-gas chain", but I thought it might be possible to use for non-free-gas chains such as Polygon, if you had a way of ensuring your signing key had enough gas to pay for the deployment. Hence calling the new option `--remote-node-deploy`, not `--remote-node-free-gas` or similar.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 12:20:52 +0000 UTC
    </div>
</div>

