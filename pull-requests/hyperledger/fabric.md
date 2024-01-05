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
                PR <a href="https://github.com/hyperledger/fabric/pull/4590" class=".btn">#4590</a>
            </td>
            <td>
                <b>
                    fix error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #4589

Analysed recent errors in gatway integration tests. There is one error everywhere (I hope it is the last one). 
The problem is that after restarting orderer2 peer did not manage to reconnect to it because of backoff timeout.
I studied the logs and made it so that we don't send Submit until the peer connects to orderer2.

For a test this is ok, but maybe in real work it will not work. Then I suggest someone to modify the file `github.com/hyperledger/fabric/internal/pkg/gateway/registry.go` . When selecting connections orderers should check the connection status and reconnect violently if necessary.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-04 21:42:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4588" class=".btn">#4588</a>
            </td>
            <td>
                <b>
                    Validate the request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The patchset adds validation to the request before using it.

Change-Id: Ic6a7a65d6da289d84fe82c3f6e048e396b1f1a0e

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

The patchset adds validation to the request before using it.

This can help protect from malformed request.


#### Additional details

N/A

#### Related issues

N/A

#### Release Note

N/A

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-03 22:04:07 +0000 UTC
    </div>
</div>

