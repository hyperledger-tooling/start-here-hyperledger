---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1195" class=".btn">#1195</a>
            </td>
            <td>
                <b>
                    test-network envVar.sh script improvement
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change shell script to use single equals.

In my shell environment single bracket with double equals did not work. It caused failure when running the chaincode-external tutorial README.

It looks like for maximum portability, it is best to use single bracket with single equals.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-12 02:42:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1194" class=".btn">#1194</a>
            </td>
            <td>
                <b>
                    Fix docs and scripts for asset-transfer-basic as an external service
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
#### Type of change

- Bug fix
- Documentation update

#### Description

This PR fixes docs and scripts for asset-transfer-basic as an external service.

The path to the configuration file that the peer container in the test-network references seems to have changed. So we need to update the path in the procedures.

As discussed in the following mailing list exchange, starting with Fabric v2.5, so we need to change the scripts (detect, build, release, run) to start with #!/bin/bash instead of #!/bin/sh.
https://lists.hyperledger.org/g/fabric/topic/104464487

#### Related issues

Resolves #1137
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-11 04:20:01 +0000 UTC
    </div>
</div>

