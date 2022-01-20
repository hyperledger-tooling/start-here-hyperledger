---
layout: default
title: transact
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/transact
---

# transact <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/transact){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/307" class=".btn">#307</a>
            </td>
            <td>
                <b>
                    Update workload to report remaining time in logs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If a duration is set for a workload the `request_logger` should report how much time remains in the format hh:mm:ss

Example output for a workload with duration of 10 minutes:
```
Starting Command-Workload-0 with target rate 1/s and duration 10m
Command-Workload-0: Jan-14-2022 17:06:53.209, Sent: 5, Queue Full 0, Batches/s 0.999, time remaining 0:9:54
Command-Workload-0: Jan-14-2022 17:06:58.213, Sent: 5, Queue Full 0, Batches/s 0.999, time remaining 0:9:49
Command-Workload-0: Jan-14-2022 17:07:03.217, Sent: 5, Queue Full 0, Batches/s 0.999, time remaining 0:9:44
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-14 17:12:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/306" class=".btn">#306</a>
            </td>
            <td>
                <b>
                    Fix lint introduced in the 1.58 release of Rust
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
        Created At 2022-01-14 15:27:49 +0000 UTC
    </div>
</div>

