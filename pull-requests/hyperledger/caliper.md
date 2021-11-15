---
layout: default
title: caliper
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/caliper
---

# caliper <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/caliper){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1174" class=".btn">#1174</a>
            </td>
            <td>
                <b>
                    Fix Besu integration test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Change opened RPC WS API names to upper case, lower case names resulted in error.
* Remove the custom docker build from the network, use the Besu image directly and set the required parameters on the container.
* Fix the Besu version to 21.10.1
* Add some docker container log dumps in case of CI test failure

Signed-off-by: Attila Klenik <a.klenik@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-15 15:00:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1172" class=".btn">#1172</a>
            </td>
            <td>
                <b>
                    Update branch name in Azure CI pipeline configuration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Probably the first step to get the CI pipeline working (before debugging integration tests or porting to GitHub Actions).

Signed-off-by: Attila Klenik <a.klenik@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-09 12:25:06 +0000 UTC
    </div>
</div>

