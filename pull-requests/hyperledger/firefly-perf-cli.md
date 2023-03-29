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
                PR <a href="https://github.com/hyperledger/firefly-perf-cli/pull/52" class=".btn">#52</a>
            </td>
            <td>
                <b>
                    Post test balance check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change adds:
 - An optional check of the recipient token balance at the end of the test (plus a metric to track it over time)
 - Multiple actions per worker loop (so you can scale the number of parallel requests separately to scaling the workers)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-24 15:46:17 +0000 UTC
    </div>
</div>

