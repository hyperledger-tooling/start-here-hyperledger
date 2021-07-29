---
layout: default
title: fabric-sdk-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-go
---

# fabric-sdk-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-go/pull/183" class=".btn">#183</a>
            </td>
            <td>
                <b>
                    feat(gateway): add WithBlockNum option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Rationale

I have a use case where each organization has an application that listens to chaincode events through the gateway and react accordingly.
All events should be processed, even when starting the application after the other organizations.

## Proposed changes

Currently the gateway only supports listening to *new* events, not existing ones, although the event client has such capability.
This PR introduces a new gateway option to let the user specify from which block to start listening to events.

## Design choices

`FromBlockSet` is a flag since `0` would be a valid block number, we need to determine if the user has explicitly set a starting block number.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-29 09:58:58 +0000 UTC
    </div>
</div>

