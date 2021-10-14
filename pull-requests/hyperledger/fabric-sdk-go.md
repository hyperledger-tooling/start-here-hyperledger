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

I attempted to retain the default behavior, but I don't see how to do so without massive impact.
We would need to be able to distinguish between the zero and the unset case, which is not currently possible with an `int` field in the policy. I quickly tried to switch to a `string` field but did not pursue this way as this would impact many other modules.
So I went to find a middle ground: default is only applied when the resolver mode is not explicitly set and value is less or equal than zero.
I'm not very happy with this since there are different behaviors depending on the resolver mode being set or not. On the other hand the lag threshold only have meaning when using the appropriate resolver, so I guess this is fine.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-13 09:43:11 +0000 UTC
    </div>
</div>

