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
                PR <a href="https://github.com/hyperledger/caliper/pull/1515" class=".btn">#1515</a>
            </td>
            <td>
                <b>
                    Remove fisco-bcos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Node 16 is now out of lts. Fisco bcos will not work on node 18 or higher due to it not being compatible with openssl 3 so caliper at the moment can't move it's builds to node 18 or node 20. Also openssl 1.1 is now out of support and so the connector is using crypto libraries which are no longer supported. As we have no-one who can maintain this connector, it should be dropped.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-21 19:12:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1514" class=".btn">#1514</a>
            </td>
            <td>
                <b>
                    Terminate workers if caliper manager is terminated prematurely
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Caliper can run workers in multiple ways. THe most common is when they are part of the Caliper manager process, however when they are separate processes either on the same machine or remote machines, if the caliper manager is terminated unexpectedly (eg CTRL-C) then those workers still continue to drive load. We would want those workers to terminate as well. This change facilitates this by detecting if the manager is terminated prematurely and sending requests to the workers to terminate

This is a resubmitted PR of a collaboration between myself and @captainIRS (#1435 )

Signed-off-by: Dave Kelsey <d_kelsey@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-21 08:34:12 +0000 UTC
    </div>
</div>

