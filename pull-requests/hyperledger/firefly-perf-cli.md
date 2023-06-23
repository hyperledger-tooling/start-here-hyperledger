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
                PR <a href="https://github.com/hyperledger/firefly-perf-cli/pull/67" class=".btn">#67</a>
            </td>
            <td>
                <b>
                    Refactor ramp period and TPS calculation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR changes the way the ramp period works. Rather than specifying an exact request rate (which didn't quite work correctly before) the only option now is `rampLength` which is specified as a `time.Duration`. The perf CLI will delay the startup of each worker to linearly increase load throughout the ramp length.

For example, if you specify `rampLength: 60s` and you use `workers: 60`, over the course of 60 seconds, one new worker per second will be started.

The ramp period is also excluded from the final TPS calculation at the end of the test run. TPS will be calculated and logged during the test, including during the ramp period. At the end of the ramp period, the TPS calculation will switch to only look at transactions that happened after the ramp period ended. This is because the rate should be gradually changing during the ramp, and what we really want to see is the long term sustained rate after the system has warmed up.

Lastly, this PR includes a new chaincode for Fabric custom contract testing. The new chaincode is part of this PR and should be compiled and deployed to your Fabric network before running the `custom_fabric_contract` scenario.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-19 19:44:41 +0000 UTC
    </div>
</div>

