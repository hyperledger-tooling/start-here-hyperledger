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
                PR <a href="https://github.com/hyperledger/fabric-sdk-go/pull/225" class=".btn">#225</a>
            </td>
            <td>
                <b>
                    Recreate event service if WithNoCache() opt used
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds WithNoCache() func opt to the event client constructor to force reinitialization of event client instead of using an event client from cache. 

Now if two event clients will be created with the same EventService if the same context.ChannelProvider (`New(channelProvider context.ChannelProvider, opts ...ClientOption)`) was passed. As a result, the passed functional options are ignored. 

Example of undocumented behaviour:

```
eventClient1, err := event.New(chPrvdr, event.WithBlockEvents(), event.WithSeekType(seek.FromBlock), event.WithBlockNum(0))
...
eventClient2, err := event.New(chPrvdr, event.WithBlockEvents(), event.WithSeekType(seek.FromBlock), event.WithBlockNum(10))
```

eventClient2 will listen not from 10 block, but from 0. Expected behavior: the client will listen from the 10 block.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-04 09:48:39 +0000 UTC
    </div>
</div>

