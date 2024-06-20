---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1529" class=".btn">#1529</a>
            </td>
            <td>
                <b>
                    fix: do not start multiple blockchain plugin on retry of namespace start
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes https://github.com/hyperledger/firefly/issues/1527

Make sure that in the case where the NS fails to restart because of another plugin has failed do not start the blockchain plugin again when it was successfully started before.

Played around with the idea of using context to clear everything but it didn't make sense. Also I don't think a mutexLock is needed for this. 

If you are wondering how all the other plugins work it's because at initialisation part those plugins return a struct that we then use as part of starting the managers/plugins.  So we can check for the existence of that struct and not re-initialise that manager/plugin. In the case of the blockchain plugin, it's a shared struct and we just start a new event streams in the init part.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-19 17:14:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1526" class=".btn">#1526</a>
            </td>
            <td>
                <b>
                    Use codecov github action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Move to using the GitHub action as the bash script is not using the token correctly 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 16:10:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1525" class=".btn">#1525</a>
            </td>
            <td>
                <b>
                    fix: parallelize ensuring active pools on startup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When a large number of token pools are active and namespace is restarted, it take a long time to activate one by one each token pool. This PR spins a new go routine for each API call.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 15:29:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1524" class=".btn">#1524</a>
            </td>
            <td>
                <b>
                    update ff cli to main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 14:15:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1523" class=".btn">#1523</a>
            </td>
            <td>
                <b>
                    Fix docs links
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-15 11:06:54 +0000 UTC
    </div>
</div>

