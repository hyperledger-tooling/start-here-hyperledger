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
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/758" class=".btn">#758</a>
            </td>
            <td>
                <b>
                    Refactored ngrok support with necessary AuthToken
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR refactors ngrok support in AATH. As of Dec 26 2024, AATH stopped working with ngrok because of the enforcement of an AuthToken to start ngrok services. Users that need to use ngrok support in AATH will need to acquire, either free or paid for, an AuthToken from ngrok. 

At this point forward, if you are using the `-n` option on the manage script, you will also have to set an `NGROK_AUTHTOKEN` environment variable. This can be done like this for example;
```
NGROK_AUTHTOKEN=2ZrwpFakeAuthToken_W4VDBxavAzdB5K3wsDGz LEDGER_URL_CONFIG=http://test.bcovrin.vonx.io TAILS_SERVER_URL_CONFIG=https://tails.vonx.io AGENT_CONFIG_FILE=/aries-backchannels/acapy/auto_issuer_config.yaml ./manage start -a acapy-main -b acapy-main -n
```

Behavioural changes in this PR are as follows:
- There is now one ngrok container started instead of one for every Aries agent. 
- This ngrok container starts all the tunnels needed.  Note, if you have a free ngrok account and associated AuthToken then you will only be able to start 3 tunnels in the ngrok container. This shouldn't be a problem since we have not come into a use case where more than 2 are needed. 

Closes #757 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-05 22:28:51 +0000 UTC
    </div>
</div>

