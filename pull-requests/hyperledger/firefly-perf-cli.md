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
                PR <a href="https://github.com/hyperledger/firefly-perf-cli/pull/84" class=".btn">#84</a>
            </td>
            <td>
                <b>
                    Adding control for submission rate.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently in no wait submission mode, firefly-perf-cli submit test requests as fast as it possibly can. This can cause undesired load on the targeting system under test.

This PR introduces `maxSubmissionsPerSecond` setting in the configuration to add control for a more stable submission pattern.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-13 11:05:01 +0000 UTC
    </div>
</div>

