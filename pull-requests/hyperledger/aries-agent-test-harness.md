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
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/227" class=".btn">#227</a>
            </td>
            <td>
                <b>
                    Fix summary results script and create GHA
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-01 00:11:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/225" class=".btn">#225</a>
            </td>
            <td>
                <b>
                    Proposed change to test parametrization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

We're currently using a combination of "example" parameters and tags to configure the tests.

I propose to use only the example parameters, not the tags, to provide the configuration options for each test.  (IMHO tags should describe the tests but not configure them.  I find the mixed approach confusing, maybe it's just me!)

Looking for feedback before I make any changes - in this draft PR I updated the feature file for @T001-RFC0453, as well as the *.1 and *.2 version of this test.  With this change, the 3 scenarios can be collapsed into 1, with 3 sets of "example" parameters.  (Note I didn't collapse it yet in this PR, but you can see that all the steps are exactly the same.)

Thoughts?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-30 20:50:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/224" class=".btn">#224</a>
            </td>
            <td>
                <b>
                    KGR fixes for the new json-ld tests
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
        Created At 2021-04-29 18:13:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/223" class=".btn">#223</a>
            </td>
            <td>
                <b>
                    Docker script to start some agents to support manual testing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-27 17:31:12 +0000 UTC
    </div>
</div>

