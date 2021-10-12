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
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/359" class=".btn">#359</a>
            </td>
            <td>
                <b>
                    Add support for testing RFC-0044 mime types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Adds `/agent/start` backchannel POST command, which tells the backchannel to (re)start its agent, and includes a set of parameters to include in the agent's configuration (whether as command-line parameters, environment variables, or otherwise). Parameters have generic names on the AATH side, and must be translated by the backchannel for the given agent implementation. In this PR only one parameter is introduced, `mime-type` to specify the default mime type for the agent's outgoing messages as per Aries RFC 0044.
- Adds support for `/agent/start` to afgo backchannel, handling the `mime-type` parameter.
- Adds a new step that (re)starts a given agent with a given set of extra parameters.
- Adds a BDD feature for RFC 0044, that restarts Acme and Bob with given default mime types, and performs didexchange to demonstrate permissive agent acceptance of incoming mime types.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 20:10:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/358" class=".btn">#358</a>
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
        Created At 2021-10-07 03:52:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/357" class=".btn">#357</a>
            </td>
            <td>
                <b>
                    waits added to dotnet backchannel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

Added waits for Connection, Issue Credential, and Proof. This should get us 5 passing tests. However there is an issue with the dotnet agent on issuing a credential when the test does a proposal. Details of this issue is documented in #356. More investigation on what is going on in that issue is required. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-05 22:35:23 +0000 UTC
    </div>
</div>

