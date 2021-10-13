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
                PR <a href="https://github.com/hyperledger/fabric-sdk-go/pull/195" class=".btn">#195</a>
            </td>
            <td>
                <b>
                    fix: allow negative threshold for MinBlockHeight
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Negative values are used to disable the threshold and currently appear in [unit tests](https://github.com/hyperledger/fabric-sdk-go/blob/3e3a3c6aeec9622cf988d571c911c873a0e1c07a/pkg/fab/events/client/peerresolver/minblockheight/minblockheight_test.go#L34) and in [preferorg's tests](https://github.com/hyperledger/fabric-sdk-go/blob/main/pkg/fab/events/client/peerresolver/preferorg/preferorg_test.go#L63).
We currently have a real use case for this.

My understanding is that there is no reason not to allow negative values, but I'd be glad to discuss this further.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-13 09:43:11 +0000 UTC
    </div>
</div>

