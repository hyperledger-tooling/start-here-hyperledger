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
                PR <a href="https://github.com/hyperledger/caliper/pull/1176" class=".btn">#1176</a>
            </td>
            <td>
                <b>
                    Fix generator integration test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Downgrade to v3 Yeoman generator in dependencies
* Downgrade to v3 Yeoman generator in integration test

Note: Yeoman v4 requires Node.js v14 LTS, bump back versions once Node version is also bumped.

Signed-off-by: Attila Klenik <a.klenik@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-16 10:26:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1175" class=".btn">#1175</a>
            </td>
            <td>
                <b>
                    Fix Ethereum integration test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Anchor Ethereum client docker image version
* Fix geth CLI flags according to the set release

Signed-off-by: Attila Klenik <a.klenik@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-15 22:14:40 +0000 UTC
    </div>
</div>

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

