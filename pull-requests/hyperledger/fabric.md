---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4426" class=".btn">#4426</a>
            </td>
            <td>
                <b>
                    Update bootstrap script for v3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update old bootstrap.sh script to match the newer install-fabric.sh script.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-05 13:29:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4424" class=".btn">#4424</a>
            </td>
            <td>
                <b>
                    Fix install-fabric.sh to pull baseos for v3.x
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Bug fix

#### Description

Fixed install-fabric.sh to pull baseos images for v3.x as well as v2.x.

#### Additional details

#### Related issues

https://github.com/hyperledger/fabric/issues/4423
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-05 01:16:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4422" class=".btn">#4422</a>
            </td>
            <td>
                <b>
                    up consensus library
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
        Created At 2023-09-03 21:44:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4421" class=".btn">#4421</a>
            </td>
            <td>
                <b>
                    Add v3.* tags as a trigger to release job
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add v3.* tags as a trigger to release job.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-01 11:28:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4419" class=".btn">#4419</a>
            </td>
            <td>
                <b>
                    Release notes v3.0.0-preview
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release notes for v3.0.0-preview release.

Also delete old v2.5.x release notes that are now maintained in release-2.5 branch.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-01 02:08:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4418" class=".btn">#4418</a>
            </td>
            <td>
                <b>
                    Whats New doc for v3.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add What's New doc for v3.0.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-31 20:08:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4416" class=".btn">#4416</a>
            </td>
            <td>
                <b>
                    Change evaluation method in gateway.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Since RAFT node is able to run with capability turned on, changed the gateway code to evaluate consensus type rather than evaluating channel capabilities.

#### Type of change
- Bug fix

#### Description
Since RAFT node is able to run with capability turned on, changed the gateway code to evaluate consensus type rather than evaluating channel capabilities.
Following that changed the [https://github.com/hyperledger/fabric/blob/main/internal/pkg/gateway/submit.go#L53](url) file to check the consensus type.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-31 11:40:45 +0000 UTC
    </div>
</div>

