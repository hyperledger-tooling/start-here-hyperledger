---
layout: default
title: blockchain-explorer
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/blockchain-explorer
---

# blockchain-explorer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/blockchain-explorer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/blockchain-explorer/pull/262" class=".btn">#262</a>
            </td>
            <td>
                <b>
                    Fix script to specify the BC Exprorer process
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                "stop.sh" uses "ps" command to identify the process ID of Explorer.

> ps aux | grep -v "awk" | awk '/name - hyperledger-explorer/ {print $2}'

But Alpine Linux, which is used by Explorer container, returns the following values for "ps" command.

PID   USER   TIME    COMMAND
45     root     0:12    node app/main.js name - hyperledger-explorer

So correct process ID cannot be obtained by the above method. (Misidentify "root" as process ID.) 
It works correctly by specifying the format of the output of "ps" command like follows.

> ps **-eo pid,args** | grep -v "awk" | awk '/name - hyperledger-explorer/ {print $1}'
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 05:26:44 +0000 UTC
    </div>
</div>

