---
layout: default
title: firefly-perf-cli
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-perf-cli
---

# firefly-perf-cli <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-perf-cli){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-perf-cli/pull/29" class=".btn">#29</a>
            </td>
            <td>
                <b>
                    Add heartbeating to FF perf CLI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We saw a case where FireFly got an `EOF` on the WebSocket from the perf CLI:

```
[2022-03-29T17:48:00.375Z] ERROR node_0: Read failed: websocket: close 1006 (abnormal closure): unexpected EOF websocket=8a267d00-60bb-479f-b5d0-870718776047
```

... but there were no corresponding errors on the perf CLI side. I found that heartbeats were not configured.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-29 18:17:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-perf-cli/pull/28" class=".btn">#28</a>
            </td>
            <td>
                <b>
                    Message time fixes and delinquent message actions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a couple of fixes for tracking the time of messages and also adds a command line flag to exit the test runner if it detects delinquent messages. 

**The default behavior is to exit the test.** If you wish to simply log the delinquent messages and continue testing, use the `--delinquent log` flag.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-25 20:17:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-perf-cli/pull/27" class=".btn">#27</a>
            </td>
            <td>
                <b>
                    firefly-perfnode and ffperf Chart
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Used for install FireFly nodes onto K8s for performance testing and then running distributed instances of `ffperf` against them

Related to #26 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-24 12:54:47 +0000 UTC
    </div>
</div>

