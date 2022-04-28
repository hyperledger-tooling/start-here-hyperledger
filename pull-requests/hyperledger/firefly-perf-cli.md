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
                PR <a href="https://github.com/hyperledger/firefly-perf-cli/pull/34" class=".btn">#34</a>
            </td>
            <td>
                <b>
                    Extra podLabels for NetworkPolicies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: hfuss <haydenfuss@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-26 15:46:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-perf-cli/pull/33" class=".btn">#33</a>
            </td>
            <td>
                <b>
                    Multiple Workers per Test Case
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Updates README and `prep.sh` to work with the new test configuration format that allows defining multiple instances and multiple test cases per instance with a varying number of workers per test case
* Removes `monitoring/k8s.json` since its going to be tracked via https://github.com/hyperledger/firefly-helm-charts/pull/43 going forward
* Refactors config structs to better reflect the test concepts of: performance test, runner, instance, test case, and worker.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 15:33:18 +0000 UTC
    </div>
</div>

