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
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/476" class=".btn">#476</a>
            </td>
            <td>
                <b>
                    fix(dotnet): exclude mediation tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Mediation tests were being run for some tests with dotnet.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-11 06:29:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/475" class=".btn">#475</a>
            </td>
            <td>
                <b>
                    fix: waci tags and did method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The waci tests weren't specifying any did method, causing the flow to fail after my recent pr to extend did methods
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-10 20:18:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/474" class=".btn">#474</a>
            </td>
            <td>
                <b>
                    feat: oob connectionless for issue cred and present proof
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds connectionless support for both issue credential v1/v2 and present proof v1/v2 using the oob protocol. Also removed the old AIP 1 connectionless code as it was never used.

Draft for now as it's built against my fork of ACA-Py until it get's merged into main.

This only handles attachments in OOB invitations for connectionless. Probably good to also add tests for receiving oob invitations with creating a connection and processing an attachments (Should be quite easy now with all substeps being defined).

One thing I ran into and we should probably change is that AATH is build on the expectation that the oob receive invitation will return a connection record and also connection state instead of oob state. Probably because that's how it was implemented in ACA-Py. For now I've tricked the ACA-Py backchannel into returning the state it expects for now (mapping `prepare-response` to `invitation-received`), but would be good to change this to be more in line with the RFC (having less ACA-Py driven backchannel API design would be good in general I think)

We may want to move some tests from the DIDExchange tests to the oob tests now that there is a dedicated file for out of band
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-10 17:15:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/473" class=".btn">#473</a>
            </td>
            <td>
                <b>
                    fix(acapy): check schema cred def exists before creating
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix for changes introduced in https://github.com/hyperledger/aries-cloudagent-python/pull/1721

ACA-Py now checks if a schema/cred def already exists before creating it. This PR retrieves the created schemas/cred defs and see if it already exists
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-10 16:50:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/472" class=".btn">#472</a>
            </td>
            <td>
                <b>
                    Workaround the dotnet-master build not working by using dotnet test agent everywhere -- revert later possible
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-08 21:05:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/470" class=".btn">#470</a>
            </td>
            <td>
                <b>
                    Fix bad link as highlighted in #443
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-08 20:44:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/468" class=".btn">#468</a>
            </td>
            <td>
                <b>
                    fix(afj): use npm alpha version again
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update AFJ to again use the latest alpha version from npm

Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-06 15:13:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/467" class=".btn">#467</a>
            </td>
            <td>
                <b>
                    feat: support revocation notification v1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds support for revocation notification v1 in the revocation tests. For ACA-Py it currently uses an incorrect value for the `thread_id` in the revocation notification, so this is also being used in the AATH tests. I don't think there's an implementation that implemented the actual RFC. It also supports the correct thread_id when checking if a revocation notification has been received, so if other agents do support the RFC variant it will also work (but not with ACA-Py as ACA-Py doesn't follow the RFC).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-06 13:20:43 +0000 UTC
    </div>
</div>

