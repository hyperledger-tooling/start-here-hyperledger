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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/403" class=".btn">#403</a>
            </td>
            <td>
                <b>
                    Upgrade to IAS v4 and calibrate flags for Azure
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                IAS v3 has reached end-of-life. Moving to v4 to support SGX HW mode.

Also, update flags in quote verification. Such more flexible policy evaluation allows to quote verification on Azure machines.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-23 02:58:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/402" class=".btn">#402</a>
            </td>
            <td>
                <b>
                    Fix a problem with the client build and canonicalize python clean
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix client flags in the python setup file.

Fix a problem with dependency on SGX_SDK (not required for the client) when cleaning. Basically this makes clean in the python directory the same as it is in all of the other directories.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-21 20:34:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/401" class=".btn">#401</a>
            </td>
            <td>
                <b>
                    Remove tinyscheme download from pdo-dev image
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
        Created At 2023-02-21 19:48:01 +0000 UTC
    </div>
</div>

