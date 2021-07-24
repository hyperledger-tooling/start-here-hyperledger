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
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/303" class=".btn">#303</a>
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
        Created At 2021-07-24 03:52:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/302" class=".btn">#302</a>
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
        Created At 2021-07-23 03:52:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/301" class=".btn">#301</a>
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
        Created At 2021-07-22 03:52:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/300" class=".btn">#300</a>
            </td>
            <td>
                <b>
                    fix: afj and dotnet interop issues
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                AFJ had a lot of changes that were not updated in AATH. 4 issues:

1. AFJ sends https messages by default. Although .NET supports https, the backchannel did not -> Updated .NET backchannel to support https messages
2. AFJ includes both the `IndyAgent` and `did-communication` services in a did doc. .NET errors if other services than `IndyAgent` are present. As I don't suspect AF.NET to be updated in the near future I'v made a PR to AFJ: https://github.com/hyperledger/aries-framework-javascript/pull/402. We will wait with sending this until we support did exchange.
3. .NET crashes if no `mime-type` is present ([optional according to the RFC](https://github.com/hyperledger/aries-rfcs/blob/master/features/0036-issue-credential/README.md#mime-type-and-value)). AFJ doesn't send a mime-type if it is not explicitly set -> Updated AFJ to emit `mime-type` value of `text/plain` if not set
4. AFJ didn't take the presentation preview property quirk (as described [here](https://github.com/hyperledger/aries-agent-test-harness/issues/259#issuecomment-884553477)) into account. -> fixed.

This PR should be merged after https://github.com/hyperledger/aries-framework-javascript/pull/402 is merged and I had the chance to update the dependency in here.

afj-dotnet and acapy-dotnet-javascript fully passing now
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-21 21:47:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/299" class=".btn">#299</a>
            </td>
            <td>
                <b>
                    Mobile wait states
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add a delay to wait for mobile to make a connection request before responding

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-20 18:14:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/298" class=".btn">#298</a>
            </td>
            <td>
                <b>
                    chore: update afj backchannel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates AFJ backchannel to latest release on NPM. Haven't updated yet to use the main branch but that should be a minor addition now.

Let's hope this also resolves #282 (works for me locally)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-19 16:09:59 +0000 UTC
    </div>
</div>

