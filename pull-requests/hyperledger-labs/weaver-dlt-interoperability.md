---
layout: default
title: weaver-dlt-interoperability
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/weaver-dlt-interoperability
---

# weaver-dlt-interoperability <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/weaver-dlt-interoperability){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/399" class=".btn">#399</a>
            </td>
            <td>
                <b>
                    fix(driver): monitor to always process events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Monitor should always process events if there is a single block not yet read.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-20 18:15:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/398" class=".btn">#398</a>
            </td>
            <td>
                <b>
                    feat(fabric-driver): Added monitor for missed events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Added Monitor in fabric driver for missed events.
2. Removed contract event listener, now block listener serves both block and contract events.
3. Two env variables to configure monitor:
```
MONITOR_ENABLE: Enable or disable monitor
MONITOR_SYNC_PERIOD: time period in seconds for monitor to sleep before running again
```
4. Fix Fabric testnet for Mac
5. Upgrade Fabric testnet to v2.5
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-19 19:50:06 +0000 UTC
    </div>
</div>

