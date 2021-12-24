---
layout: default
title: aries-agent-test-harness
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-agent-test-harness
---

# aries-agent-test-harness <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-agent-test-harness){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/406" class=".btn">#406</a>
            </td>
            <td>
                <b>
                    moved crons so they do not overlap
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

This PR should fix the failing send reports in a couple of runsets. Cron jobs were overlapping and the allure server was busy processing when some runsets asked to generate the report. This caused a failure in the runset. 

A more sophisticated solution can be investigated in the future so we don't have to set the job time in the workflows. See #403 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-22 17:44:09 +0000 UTC
    </div>
</div>

