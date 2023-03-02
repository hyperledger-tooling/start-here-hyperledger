---
layout: default
title: private-data-objects
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/private-data-objects
---

# private-data-objects <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/private-data-objects){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/412" class=".btn">#412</a>
            </td>
            <td>
                <b>
                    Start moving towards service startup that could be used for "production"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Three big changes in this PR:

1. Dropped the "count" parameter from the service start up script; a service instance will now start for each of the configuration files in the configuration directory. And... the configuration directory is a parameter to startup. That should make it possible to separate "test" configuration from a "production" configuration.
2. Changed all the hard coded localhost references in the configuration files to PDO_HOSTNAME. We have the variable. Its supposed to be used. Now it is used.  And... the configuration files can be placed in an alternate directory. Again, goal is to simplify configuring a set of services for "production".
3. Fixed up a bunch of problems that popped up in docker tests. Turns out that the way we had the dockerfiles the hardcoded localhost was NECESSARY to test correctly. Ughh... Fixed that. Not pretty, but it work.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-01 21:54:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/406" class=".btn">#406</a>
            </td>
            <td>
                <b>
                    Changes to support EPID quote verification within CCF PDO TP
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Tested in SIM and HW mode on Azure ACC VMs. Tested on bare metal as well as docker end to end for both CCF and Sawtooth. Have not tested while operating within proxy environment. Docker end to end test in HW mode needs a patch to work within proxy environment. Will push patch separately. Thanks.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-24 21:40:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/405" class=".btn">#405</a>
            </td>
            <td>
                <b>
                    Update threading to make the client work with Ubuntu 22
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Some pretty significant changes to the replication and transaction threading modules to address a problem where threads were not terminating in ubuntu 22. we were using the threadpoolexecutor in an unusual way. this moves back to more basic threads. in the future we should re-examine. threadpoolexecutor is probably the right way to go, but a lot of the logic will have to adjust to use it in the more traditional way.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-24 15:53:30 +0000 UTC
    </div>
</div>

