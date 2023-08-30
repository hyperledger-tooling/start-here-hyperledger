---
layout: default
title: yui-relayer
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/yui-relayer
---

# yui-relayer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/yui-relayer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-relayer/pull/101" class=".btn">#101</a>
            </td>
            <td>
                <b>
                    Add check process for channel and connection finalization to handshake
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * set `finality_delay` value to 5
* `connection not finalized, retrying...` is debug log

```
sts/eth2eth/scripts/../demo/.urelayer tx connection ibc01
2023/08/30 11:49:13 - [ibc0]@{0}conn(connection-0)-{STATE_UNINITIALIZED_UNSPECIFIED} : [ibc1]@{0}conn(connection-0)-{STATE_UNINITIALIZED_UNSPECIFIED}
2023/08/30 11:49:19 connection not finalized, retrying...
2023/08/30 11:49:20 connection not finalized, retrying...
2023/08/30 11:49:21 connection not finalized, retrying...
2023/08/30 11:49:22 connection not finalized, retrying...
2023/08/30 11:49:23 - [ibc1]@{0}conn(connection-0)-{STATE_UNINITIALIZED_UNSPECIFIED} : [ibc0]@{240}conn(connection-0)-{STATE_INIT}
2023/08/30 11:49:29 connection not finalized, retrying...
2023/08/30 11:49:30 connection not finalized, retrying...
2023/08/30 11:49:31 connection not finalized, retrying...
2023/08/30 11:49:32 connection not finalized, retrying...
2023/08/30 11:49:33 - [ibc0]@{250}conn(connection-0)-{STATE_INIT} : [ibc1]@{250}conn(connection-0)-{STATE_TRYOPEN}
2023/08/30 11:49:39 connection not finalized, retrying...
2023/08/30 11:49:40 connection not finalized, retrying...
2023/08/30 11:49:41 connection not finalized, retrying...
2023/08/30 11:49:42 connection not finalized, retrying...
2023/08/30 11:49:43 - [ibc1]@{260}conn(connection-0)-{STATE_TRYOPEN} : [ibc0]@{260}conn(connection-0)-{STATE_OPEN}
2023/08/30 11:49:49 ★ Connection created: [ibc0]client{mock-client-0}conn{connection-0} -> [ibc1]client{mock-client-0}conn{connection-0}
+ /Users/dongri.jin/go/src/github.com/datachainlab/toki-relayer-longrun/tests/eth2eth/scripts/../../../relayer/build/relayer --home /Users/dongri.jin/go/src/github.com/datachainlab/toki-relayer-longrun/tests/eth2eth/scripts/../demo/.urelayer tx channel ibc01
2023/08/30 11:49:49 - [ibc0]@{0}chan(channel-0)-{STATE_UNINITIALIZED_UNSPECIFIED} : [ibc1]@{0}chan(channel-0)-{STATE_UNINITIALIZED_UNSPECIFIED}
2023/08/30 11:49:53 channel not finalized, retrying...
2023/08/30 11:49:53 channel not finalized, retrying...
2023/08/30 11:49:54 channel not finalized, retrying...
2023/08/30 11:49:55 channel not finalized, retrying...
2023/08/30 11:49:56 - [ibc1]@{0}chan(channel-0)-{STATE_UNINITIALIZED_UNSPECIFIED} : [ibc0]@{273}chan(channel-0)-{STATE_INIT}
2023/08/30 11:50:03 channel not finalized, retrying...
2023/08/30 11:50:03 channel not finalized, retrying...
2023/08/30 11:50:04 channel not finalized, retrying...
2023/08/30 11:50:05 channel not finalized, retrying...
2023/08/30 11:50:06 - [ibc0]@{283}chan(channel-0)-{STATE_INIT} : [ibc1]@{283}chan(channel-0)-{STATE_TRYOPEN}
2023/08/30 11:50:13 channel not finalized, retrying...
2023/08/30 11:50:13 channel not finalized, retrying...
2023/08/30 11:50:14 channel not finalized, retrying...
2023/08/30 11:50:15 channel not finalized, retrying...
2023/08/30 11:50:16 - [ibc1]@{293}chan(channel-0)-{STATE_TRYOPEN} : [ibc0]@{293}chan(channel-0)-{STATE_OPEN}
2023/08/30 11:50:23 ★ Channel created: [ibc0]chan{channel-0}port{transfer} -> [ibc1]chan{channel-0}port{transfer}
+ set +x
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-30 03:04:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-relayer/pull/100" class=".btn">#100</a>
            </td>
            <td>
                <b>
                    add `ChainInfo::Timestamp` and implement it for the tendermint chain module
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
        Created At 2023-08-24 08:10:49 +0000 UTC
    </div>
</div>

