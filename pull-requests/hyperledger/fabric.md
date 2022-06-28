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
                PR <a href="https://github.com/hyperledger/fabric/pull/3502" class=".btn">#3502</a>
            </td>
            <td>
                <b>
                    Add OpenTelemetry interceptors to capture traces from gRPC communications
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See #2954 - was closed for inactivity while #2997 was pending.

#### Type of change
- New feature

#### Description

Adds OpenTelemetry tracing by adding interceptors on all gRPC communications.

#### Related issues
This is tied to https://github.com/hyperledger/fabric-rfcs/blob/main/text/0000-opentelemetry-tracing.md

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 21:31:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3500" class=".btn">#3500</a>
            </td>
            <td>
                <b>
                    Check if inner consensus message is missing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                An orderer to orderer consensus message that contains an empty inner message crashes the node because it attempts to figure out its type and the mere action of determining the type of a nil pointer, causes a panic.

This commit ensures the inner message is not nil.

Change-Id: I06b466e6ff6d43f2b9804dd21185241716356050
Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-21 15:53:34 +0000 UTC
    </div>
</div>

