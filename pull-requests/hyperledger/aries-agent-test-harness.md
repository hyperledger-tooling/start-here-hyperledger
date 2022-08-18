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
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/550" class=".btn">#550</a>
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
        Created At 2022-08-18 04:46:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/549" class=".btn">#549</a>
            </td>
            <td>
                <b>
                    Turn off auto respond flag to allow manual respond tests to run
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-15 22:05:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/548" class=".btn">#548</a>
            </td>
            <td>
                <b>
                    Fix for revocation-related tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

... also filter out another class of tests not supported by aca-py (tests with no http inbound transport, since the acapy backchannel does't support webhooks over ws)

Note in combination with aca-py PR https://github.com/hyperledger/aries-cloudagent-python/pull/1897 gets us down to one failing test ...

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-15 20:46:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/547" class=".btn">#547</a>
            </td>
            <td>
                <b>
                    Remove unsupported tests from aca-py suite
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

Remove tests relating to DID method orb and agents with no inbound transports

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-15 15:07:47 +0000 UTC
    </div>
</div>

