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

