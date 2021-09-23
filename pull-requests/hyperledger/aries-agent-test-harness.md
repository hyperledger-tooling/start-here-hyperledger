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
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/348" class=".btn">#348</a>
            </td>
            <td>
                <b>
                    Add verity afj dotnet runsets
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds Verity with javascript and dotnet agents. They are failing locally, so this PR is just to try the execution in GHA to determine if the same issue exists as locally. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-23 17:56:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/347" class=".btn">#347</a>
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
        Created At 2021-09-23 03:52:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/346" class=".btn">#346</a>
            </td>
            <td>
                <b>
                    further increase waits in javascript backchannel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

An added increase in javascript backchannel wait times for certain operations in hopes it fixes the failures in the daily test runsets. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-22 23:17:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/345" class=".btn">#345</a>
            </td>
            <td>
                <b>
                    increased the javascript wait time
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

Increased the wait times for certain calls in the javascript backchannel. Hopefully this should clear up the failures in the daily runsets. Locally all these tests are passing. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-21 23:54:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/344" class=".btn">#344</a>
            </td>
            <td>
                <b>
                    Support afgo-acapy RFC0453 interop, and fix 0023 interop issues
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                AFGO-ACAPy interop tests that are now enabled:
- all didexchange tests 
- all JSON-LD issue-credential tests, with the exception of BBS+ with ACA-Py issuer, as there's an intermittent error where ACA-Py gets the public orb DID of the afgo holder instead of a peer DID.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-21 21:24:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/343" class=".btn">#343</a>
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
        Created At 2021-09-18 03:52:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/342" class=".btn">#342</a>
            </td>
            <td>
                <b>
                    Add findy and verity links to interop, tweak to script and findy action
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
        Created At 2021-09-18 00:03:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/341" class=".btn">#341</a>
            </td>
            <td>
                <b>
                    Add backchannel for findy-agent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Laura Vuorenoja <laura.vuorenoja@op.fi>

Add backchannel for testing compatibility with [Findy Agency](https://findy-network.github.io) agent. Current interoperability target for findy-agent is IOP1.0 excluding revocation.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-17 09:39:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/340" class=".btn">#340</a>
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
        Created At 2021-09-17 03:52:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/339" class=".btn">#339</a>
            </td>
            <td>
                <b>
                    removed running workflows in PRs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #337

Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-16 20:30:07 +0000 UTC
    </div>
</div>

