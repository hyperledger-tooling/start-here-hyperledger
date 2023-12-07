---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2655" class=".btn">#2655</a>
            </td>
            <td>
                <b>
                    Slight improvement to credx proof validation error message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Slight improvement to an error message.  (This confused me as it logged a stack trace during integration testing but didn't report a failed test.  Reason = it's not an error, just a proof validation failure.)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-07 17:27:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2653" class=".btn">#2653</a>
            </td>
            <td>
                <b>
                    Connection and DIDX Problem Reports
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - add current message thread to problem report messages to identify which message/thread encountered the problem.
- problem report handlers will find connections based on thread/request id
- register didx problem report so handler will be active and deal with didx problem reports
- update tests to match new handler logic

fixes #2650 
fixes #2598

A lot of underlying issues uncovered (and now addressed) arising from #2530 investigation. 

Synopsis is the implemented logic for sending/handling connection (and didx) problem reports that require a fully working connection. This prevented us from notifying if the problem arose during the request or early response stages. That is addressed by allowing the problem report message types to skip the active check in the responder. Then the next issue was the agent receiving the problem report could not match up their connection, so the sender adds the failing message's thread to the problem report message before delivery, the receiver can then look up connections by a known thread id. Then the DIDX problem report code was always failing when trying to determine the messages targets, so that code was updated to handle diddoc attach conversion to diddoc and then resolve the targets. Then uncovered the fact that the DIDX problem reports (and handler) were not registered in the protocol message registry so those wouldn't get handled when we finally parsed the targets.

Sigh, lots of stuff that just never worked... 🤷 ...hoping that these fixes will be of use when there are issues in the early stages of connecting agents.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-06 19:59:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2651" class=".btn">#2651</a>
            </td>
            <td>
                <b>
                    Update integration tests for anoncreds-rs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">AnonCreds</span>
            </td>
            <td>
                Final update from the `anoncreds-rs` branch, brings across some integration tests, and also includes a bit of cleanup.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-04 18:55:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2645" class=".btn">#2645</a>
            </td>
            <td>
                <b>
                    feat: add did:jwk resolver
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This implements a did:jwk resolver. See https://github.com/hyperledger/aries-acapy-plugins/pull/47 for context.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-01 22:07:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2643" class=".btn">#2643</a>
            </td>
            <td>
                <b>
                    Initial migration of anoncreds revocation code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">AnonCreds</span>
            </td>
            <td>
                Adds revocation support from the anoncreds-rs branch.  Still a few TODO's but this PR is ready to go and I'll continue the work in the next PR.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-30 19:04:56 +0000 UTC
    </div>
</div>

