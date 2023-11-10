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
                PR <a href="https://github.com/hyperledger/firefly-perf-cli/pull/72" class=".btn">#72</a>
            </td>
            <td>
                <b>
                    Adding latency metrics to the report and fixing actionsPerLoop
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - [x] Actions in a loop are not emitted in parallel. Based on description: `This can be helpful when you want to scale the number of actions done in parallel without having to scale the number of workers.` I believe it's intended that actions should be triggered in parallel.
> It's not clear when should one add more workers vs set more actions per loop to scale the number of requests. My thinking is that we could bind workers to a specific signing address in the future, so if one want multiple requests per signing address then they tune `actionsPerWorker` if they want more signing addresses to send requests, then they add more workers
- [x] Add latency metrics 
- [x] Support for generating an HTML report at the test run
- [x] Report latency metrics in the final report
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-08 10:04:24 +0000 UTC
    </div>
</div>

