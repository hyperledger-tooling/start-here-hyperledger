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
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/69" class=".btn">#69</a>
            </td>
            <td>
                <b>
                    Create stack and config optimized for running a FireFly core outside of docker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR makes it easy(er) to run one or more FireFly core processes outside of docker. This is especially useful when making code changes to FireFly itself and wanting to step through the code in a debugger.

You can now use the `-e <int>` flag to specify the number of core processes that you would like to manage outside of docker. The default (if `-e` is not set) is `0`, meaning that unless `-e` is set, all FireFly core processes will run inside docker.

When starting a stack with external processes, the CLI will wait for FireFly to run before running contract deployment and member registration. This means that the developer doesn't have to worry about complex registration even when they are debugging FireFly locally. This should greatly speed up local development going foward.

> **NOTE**: Right now it is a requirement that _at least one_ FireFly core run inside docker, because the CLI needs to pull the compiled smart contracts out of a container to install them

Resolves https://github.com/hyperledger-labs/firefly-cli/issues/39
Resolves https://github.com/hyperledger-labs/firefly-cli/issues/2

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-30 14:05:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/67" class=".btn">#67</a>
            </td>
            <td>
                <b>
                    Replace ganache with geth
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR removes `ganache-cli` and replaces it with a proper `geth` node. Ganache has some interesting (not quite correct behavior) that was causing https://github.com/hyperledger-labs/firefly/issues/115 on local CLI environments, due to ethconnect not being able to tell the difference between an empty event list, or a non existent list. This fixes that strange behavior, and is even closer to what running FireFly would be like in a real production environment, with no additional containers.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-28 19:01:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/66" class=".btn">#66</a>
            </td>
            <td>
                <b>
                    Do not deploy Payment contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is no longer used. It will be superceded by the new work on Tokens
when available.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-28 16:14:04 +0000 UTC
    </div>
</div>

