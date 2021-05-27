---
layout: default
title: indy-node-monitor
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-node-monitor
---

# indy-node-monitor <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-node-monitor){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-node-monitor/pull/33" class=".btn">#33</a>
            </td>
            <td>
                <b>
                    Fix pipe to file issue on Windows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Only use `winpty` when running interactively on Windows.
- This fixes the `stdout is not a tty` issue seen on Windows when piping the output of the script to a file.
  - For example; `./run.sh --net smn --status > status.json`

Signed-off-by: Wade Barnes <wade@neoterictech.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-22 15:33:50 +0000 UTC
    </div>
</div>

