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
                PR <a href="https://github.com/hyperledger/fabric/pull/3503" class=".btn">#3503</a>
            </td>
            <td>
                <b>
                    Update secured asset transfer tutorial
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates to align with latest sample:
- Set state-based endorsement to asset owner only
- Document that additional endorsers could be set to make the sample more secure, e.g. using a trusted third party
- Set environment variable for ASSET_ID and reference in commands to make it easy to copy/paste sample commands

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-29 11:32:17 +0000 UTC
    </div>
</div>

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

