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
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/401" class=".btn">#401</a>
            </td>
            <td>
                <b>
                    aries-vcx: Send presentation ack always
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                acapy now seems to expect presentation ack even if the presentation is evaluated as invalid. This fixes some currently failing tests.

Signed-off-by: Miroslav Kovar <miroslavkovar@protonmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-11 14:39:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/400" class=".btn">#400</a>
            </td>
            <td>
                <b>
                    aries-vcx: Fix failing tests, enable revocations where acapy is prover
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Miroslav Kovar <miroslavkovar@protonmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-10 13:33:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/399" class=".btn">#399</a>
            </td>
            <td>
                <b>
                    Centralize docker host IP script.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - This is an update to the previous commit to update the support for Docker networking.  The `getDockerHost` has been pulled out and placed in a central location where it can be updated as needed rather than having to update dozens of scripts the next time there is a change.

Signed-off-by: Wade Barnes <wade@neoterictech.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 18:35:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/398" class=".btn">#398</a>
            </td>
            <td>
                <b>
                    Add support for changes to internal Docker networking.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Networking changes introduced in Docker 4.1.x and forward on Windows and MAC stop the direct use of the internal docker host IP returned by the `docker run --rm --net=host eclipse/che-ip` process.  On Windows and MAC `host.docker.internal` needs to be used for internal connections between containers.

Signed-off-by: Wade Barnes <wade@neoterictech.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-06 21:57:50 +0000 UTC
    </div>
</div>

