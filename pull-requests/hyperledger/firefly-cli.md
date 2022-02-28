---
layout: default
title: firefly-cli
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-cli
---

# firefly-cli <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-cli){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/149" class=".btn">#149</a>
            </td>
            <td>
                <b>
                    Use fabconnect image version in manifest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                While investigating https://github.com/hyperledger/firefly/issues/537 I discovered that we weren't actually using the version of fabconnect listed in the manifest, and were always pulling latest still. This caused lots of inconsistencies depending on when someone pulled the stack and sometimes resulted in a broken stack.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-22 15:45:04 +0000 UTC
    </div>
</div>

