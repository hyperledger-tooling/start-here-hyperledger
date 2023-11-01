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
                PR <a href="https://github.com/hyperledger/besu/pull/6085" class=".btn">#6085</a>
            </td>
            <td>
                <b>
                    create trielog state for tracing
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

## Fixed Issue(s)

fixes #6050 
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-25 08:53:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6083" class=".btn">#6083</a>
            </td>
            <td>
                <b>
                    Add transaction selector based on min priority fee parameter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Add transaction selector based on min priority fee parameter

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-25 07:35:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6082" class=".btn">#6082</a>
            </td>
            <td>
                <b>
                    Add option to clique to skip creating empty blocks
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
Add an option to clique to not create empty blocks. To skip creating empty blocks the config `createemptyblocks` can be false in the clique configuration of the genesis file. By default, Clique will create empty blocks. This is the current behaviour in Clique.

This is useful for large private networks that are using Clique. As empty blocks increase the amount of storage is needed.

note: That all validators must have the same setting for ``createemptyblocks`.

Changes
* Clique miner has been changed to not create empty blocks when `createemptyblocks` is disabled
* Header validation for Clique checks that there are no empty blocks when `createemptyblocks` is disabled

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-25 06:50:57 +0000 UTC
    </div>
</div>

