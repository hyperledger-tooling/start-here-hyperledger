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
                PR <a href="https://github.com/hyperledger/firefly-perf-cli/pull/36" class=".btn">#36</a>
            </td>
            <td>
                <b>
                    [override-typo] fixing typo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Echelberger <eberger727@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-03 15:24:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-perf-cli/pull/35" class=".btn">#35</a>
            </td>
            <td>
                <b>
                    Fix prep.sh for docker-compose.yml and update getLogs.sh for 1 historical
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Fix `prep.sh` now that `docker-compose.yml` has moved back out of `init` to the base dir
- Update `getLogs.sh` to:
    - Get one historical log file for each container, as well as the base log
    - Only get the last 100k lines from `ffperf.log`
- Update `prep.sh` with the long-run defaults we have been using
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-03 12:38:03 +0000 UTC
    </div>
</div>

