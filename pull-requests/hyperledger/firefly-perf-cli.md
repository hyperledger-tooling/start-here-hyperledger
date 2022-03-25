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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-perf-cli/pull/26" class=".btn">#26</a>
            </td>
            <td>
                <b>
                    New run Command with Graceful Shutdown and HTTP Server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Provides a YAML or JSON "DSL" for defining multiple test "instances". A test instance consists of a _single_ test type, test options, length, and number of workers.

The idea is that we can now run multiple instances of `ffperf` either with `nohup` or multiple containers / pods. Each instance just then takes in a different `--instance-name` or `--instance-index` to determine what it runs.

Can run in either test or daemon mode. HTTP server runs in the background to serve future Prometheus metrics.

Includes Dockerfile for building as a Docker image.

Tested locally and via https://github.com/hyperledger/firefly-perf-cli/pull/27.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 18:32:58 +0000 UTC
    </div>
</div>

