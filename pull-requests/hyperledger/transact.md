---
layout: default
title: transact
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/transact
---

# transact <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/transact){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/127" class=".btn">#127</a>
            </td>
            <td>
                <b>
                    Command family smart contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates the command family and adds a sabre compatible command smart contract.

The make_command_transaction method is moved behind a separate experimental feature to allow for the command smart contract to be compiled into wasm.

The command family transaction handler is updated to use namespaces and a method is added to generate the sha512 hash of "command".

The necessary information is added to the docker files to allow for the command smart contract scar file to be build and archived in Jenkins.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-30 00:24:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/126" class=".btn">#126</a>
            </td>
            <td>
                <b>
                    Command family cli subcommands
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds subcommands to the transact cli to interact with the command family smart contract. This is behind the experimental feature "command".
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-30 00:22:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/123" class=".btn">#123</a>
            </td>
            <td>
                <b>
                    Update dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates various dependencies, cleaning up the output of 'cargo outdated -R'.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-28 23:05:58 +0000 UTC
    </div>
</div>

