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
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/267" class=".btn">#267</a>
            </td>
            <td>
                <b>
                    fix typo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

conection instead of connection. :(
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-24 19:23:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/266" class=".btn">#266</a>
            </td>
            <td>
                <b>
                    Cred id bypass invite create
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates the secondary get of the inviter's connection_id at the point the invitee accepts the invitation in the 160 Connection Protocol tests. There is now a call to get the connection id based on the invitation id. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-23 19:47:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/264" class=".btn">#264</a>
            </td>
            <td>
                <b>
                    Connection ID shared between roles support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

This adds a bypass to getting the connection_id on the inviter invitation creation step. In the Invitation acceptance step for the invitee, the connection id returned is also used as the inviter connection id. It is assumed that the agent uses a shared connection id between the roles. 

closes #262
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-22 14:57:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/263" class=".btn">#263</a>
            </td>
            <td>
                <b>
                    Update to readme for AND OR tags in Execution
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

Updated the README to explain how to use AND OR with tags in the execution of tests with ./manage script. 

Also fixed a typo in the afgo yml file. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-21 15:24:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/261" class=".btn">#261</a>
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
        Created At 2021-06-20 03:56:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/260" class=".btn">#260</a>
            </td>
            <td>
                <b>
                    Afgo Backchannel Proof Support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds Proof support to the afgo backchannel. Coming along with the proof tests are more issue cred tests. At this point Indy creds are supported. json-ld will need further work. 
The yml file for the daily run of the afgo tests has been updated. There are now a total of 7 test scenarios, and all are expected to pass. 

I think (99% sure) that I have fixed the randomly failing flakey test/backchannel code. So we should see a consistently passing full set of afgo tests.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-18 21:29:40 +0000 UTC
    </div>
</div>

