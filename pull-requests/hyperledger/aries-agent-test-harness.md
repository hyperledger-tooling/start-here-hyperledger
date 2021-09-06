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
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/328" class=".btn">#328</a>
            </td>
            <td>
                <b>
                    Pin tar version for javascript backchannel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

Pin the tar version due to security vulnerability.

Manually "fixed" the yarn.lock file, not sure that this is the best approach :-S

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-03 22:01:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/327" class=".btn">#327</a>
            </td>
            <td>
                <b>
                    Auto respond handling for Issue Credential/Proof 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds support for auto-respond in AATH, along with the removal of interim agent state checks.  These changes affect Issue Credential 1.0 and 2.0 along with Presentation 1.0 and 2.0.  

There are two instances (one for Issue Credential and one for Presentation) where the state check could not  be removed at this time. Removing them causes problems with the Acapy to Dotnet runset. 
One is in `@when('"{issuer}" offers a credential')` on line 254 of `0036-issue-credential.py`.
```
assert expected_agent_state(context.holder_url, "issue-credential", context.cred_thread_id, "offer-received")
```
The other is in `@when('"{verifier}" sends a request for proof presentation to "{prover}"')` on line 174 of `0037-present-proof.py`
```
assert expected_agent_state(context.prover_url, "proof", context.presentation_thread_id, "request-received")
```
For backchannel developers that do not need this state check in an auto responding agent, please just return 200, with the expected state for now. These lines will be removed once the problem is determined and fixed. 
See outstanding issues below for further details of this issue. 

**HOW TO VERIFY**
This PR affects all run sets and all agents. No need to run them all, but a few runset executions would be prudent. Get the runset configurations from [here](https://github.com/hyperledger/aries-agent-test-harness/tree/main/.github/workflows). 


**OUTSTANDING ISSUES**
Mobile Issue: @ianco I've added the state checks in certain instances where the mobile tests are expected to wait, to the acapy backchannel. However, I only get 9 out of 10 passing. At the end of some of the tests I also get a `something went wrong` error in Trinsic Wallet, but the credential is issued properly and the presentation is made. Wondering if you can take a look and let me know if it is something I've done or this is expected? 

Dotnet Backchannel Issue: @TimoGlastra It seems, with all the state checks removed, Dotnet or the combination of Dotnet with Acapy has a problem. Executing Dotnet in all agent rolls doesn't cause this issue. I've logged an issue for this #326 . I'm wondering if you can take a look and help diagnose the problem. I'm assuming the Dotnet backchannel was doing something to advance the protocol in those state checks. 

**AWARENESS**
@smithbk @Matt-Spence 

**SPAWNED ISSUES**
#325 
#326 
#330 

Closes #320
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-03 16:29:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/324" class=".btn">#324</a>
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
        Created At 2021-09-01 03:52:20 +0000 UTC
    </div>
</div>

