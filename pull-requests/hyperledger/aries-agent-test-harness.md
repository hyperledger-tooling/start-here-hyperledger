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
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/564" class=".btn">#564</a>
            </td>
            <td>
                <b>
                    Changes by create-pull-request action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Automated changes by [create-pull-request](https://github.com/peter-evans/create-pull-request) GitHub action
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-08 03:12:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/561" class=".btn">#561</a>
            </td>
            <td>
                <b>
                    New custom agent config for revocation notification
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

This PR adds a custom agent config file that enabled revocation notification to be used when AATH agents are used as a service for AMTH.  To use the new config and have your agents notify holders of revocation of their credentials do this, 
`LEDGER_URL_CONFIG=http://test.bcovrin.vonx.io TAILS_SERVER_URL_CONFIG=https://tails.vonx.io AGENT_CONFIG_FILE=/aries-backchannels/acapy/auto_rev_noti_agent_config.yaml ./manage start -a acapy-main -b acapy-main`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-03 00:06:56 +0000 UTC
    </div>
</div>

