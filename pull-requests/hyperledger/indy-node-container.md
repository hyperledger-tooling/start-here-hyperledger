---
layout: default
title: indy-node-container
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-node-container
---

# indy-node-container <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-node-container){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-node-container/pull/94" class=".btn">#94</a>
            </td>
            <td>
                <b>
                    Create trivy-all-slack.yml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Commit text: workflow file for slack messages after weekly trivy scan, project context IDunion (Germany)

This file was created to get Slack notifications on the IDunion project Slack workspace channel 'docker_indy-node'. The workflow is doing a weekly trivy scan and filters all high and critical CVEs and publishes them to the mentioned Slack channel. For that to work a secret webhook URL needs to be included in this repo. The name of the secret needs to be

SLACK_WEBHOOK_URL_IDU

corresponding to the name in the file. The webhook URL needs to be a secret otherwise it will be disabled.

Best regards
Sebastian
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 09:33:17 +0000 UTC
    </div>
</div>

