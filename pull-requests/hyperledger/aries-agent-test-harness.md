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
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/278" class=".btn">#278</a>
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
        Created At 2021-07-05 03:52:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/277" class=".btn">#277</a>
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
        Created At 2021-07-04 03:52:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/276" class=".btn">#276</a>
            </td>
            <td>
                <b>
                    Auto response state handling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR removes the intermediate state handling in the Connection and DID Exchange Protocols. The tests still check for an initial state (ie invited) and and end state of `completed`. As for auto responding and auto accepting, the backchannel is going to have to know it's in that auto mode and reply back to the calls it doesn't need to make to the agent with 200 response code.  Backchannel developers can see the examples in the DID Exchange and Connection POST Handlers in the Aca-py Backchannel.

Closes #268 

@smithbk @Matt-Spence If there are any other state asserts that get in the way, let me know and I'll remove them as well.  Issue Cred and Proof will follow the same pattern as above but will come later. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-02 21:46:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/275" class=".btn">#275</a>
            </td>
            <td>
                <b>
                    Add backchannel-specific extra parameters support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Can be used to, for example, run all tests using aca-py askar vs indy libraries

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-02 19:19:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/274" class=".btn">#274</a>
            </td>
            <td>
                <b>
                    Switch to 'slim' docker image for acapy back channel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This reduces the image size by about 400Mb on my system. It should also be a little faster, combining the pip package installs and removing one apt-get update.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-02 17:35:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/273" class=".btn">#273</a>
            </td>
            <td>
                <b>
                    Back-channels cleanup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR applies Black formatting to the back channel implementations, fixes a bunch of Python warnings and removes unused imports. It also removes the checks for the indy-sdk Python library which were inherited from the demo agents, but aren't necessary here (if it's needed but not installed, then the tests will fail anyway).

It also fixes a failure when running `manage stop` on my system by adjusting the check for `docker_result`, and aborts `manage build` if a docker build fails.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-01 02:33:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/271" class=".btn">#271</a>
            </td>
            <td>
                <b>
                    feat: integrate orb did method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds `orb`, a new service, which runs a small orb network and a
universal resolver orb driver instance.

Integrates the service with the afgo backchannel, by having the service
create an orb did and save the value in a data folder for the afgo backchannel
to load.

Adds a general way to load files into agent containers:
A directory named <agent-name>.data (eg, afg-master.data), if present within the
backchannel's folder, will be mounted as a volume within the given agent,
to the path `/data-mount`.

Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-30 21:42:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/270" class=".btn">#270</a>
            </td>
            <td>
                <b>
                    fixes for new connection_protocol field in messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

Fixes to support the new connection_protocol field. This will fix all failing tests across AIP20 and AIP10, except for one JSON_LD test, which I believe is expected to fail.  This PR has to be merged with #1281 in aries-cloudagent-python to work.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-30 01:12:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/269" class=".btn">#269</a>
            </td>
            <td>
                <b>
                    Add dockers to docker network to fix ngrok issues for mobile
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
        Created At 2021-06-29 16:43:08 +0000 UTC
    </div>
</div>

