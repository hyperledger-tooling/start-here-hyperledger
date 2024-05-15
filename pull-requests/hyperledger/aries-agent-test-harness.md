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
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/806" class=".btn">#806</a>
            </td>
            <td>
                <b>
                    Fix agent logs in pipeline
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This should be the last PR in relation to gathering the agent logs for each runset.  This has been tested in my working branch and is successful. 
There will be two zipped artifacts at the end of each run, one will be the container-logs that have the logs to all the supporting services of the tests. The second artifact will be agent-logs which will contain all the logs for acme to mallory, along with a request log that captures test harness to backchannel communications.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-14 17:43:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/805" class=".btn">#805</a>
            </td>
            <td>
                <b>
                    debug test container for location of logs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Still having issues locating the agent logs. A few more debug statements added. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-13 21:05:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/804" class=".btn">#804</a>
            </td>
            <td>
                <b>
                    debug test container for location of logs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Acquiring the agent logs is still not correct. Added a few debug statements to determine where we are in the test container. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-13 18:22:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/803" class=".btn">#803</a>
            </td>
            <td>
                <b>
                    archive agent logs separately
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes the path to the agent logs and archives the agent logs separately from the other container logs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-13 15:45:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/802" class=".btn">#802</a>
            </td>
            <td>
                <b>
                    added debug statements to action to find logs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The last PR did not pick up the agent logs. Added debug statements to the action to list the folders in questions to find the logs in the agent containers. 

To test this we should only need to run one of the acapy runsets in the GitHub pipeline.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-10 19:24:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/801" class=".btn">#801</a>
            </td>
            <td>
                <b>
                    added agent logs in test pipeline
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR enables acapy agent logs to be captured in the interop test pipeline. We will be able to see the state of an agent in the container-logs attachment on the run in GitHub. 

There may be a slight risk of disk space on the runner doing this, so we will give it a try and if it is a problem we can revert this change. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-10 15:49:56 +0000 UTC
    </div>
</div>

