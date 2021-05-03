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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1139" class=".btn">#1139</a>
            </td>
            <td>
                <b>
                    Adopt problem reports issue cred present proof
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                and sync up problem reports to current RFC 35
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 15:24:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1136" class=".btn">#1136</a>
            </td>
            <td>
                <b>
                    docs: add docs on issuing jsonld credentials
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds documentation on issuing JSON-LD credentials. Present Proof is todo and dependant on PR #1125.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 11:21:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1135" class=".btn">#1135</a>
            </td>
            <td>
                <b>
                    fix: add missing connection_id to issue v2 schema
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Noticed while writing documentation that the connection_id was missing. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 10:15:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1134" class=".btn">#1134</a>
            </td>
            <td>
                <b>
                    Changes in Endorser Protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a WIP pull request, and it covers the changes in endorser protocol for issues defined in 

1. #1031 
2. #1029 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-02 18:35:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1133" class=".btn">#1133</a>
            </td>
            <td>
                <b>
                    Add "minimum viable message" base class for use in plugins
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As discussed in #1096, when writing plugins, having the flexibility to implement messages differently than the pattern followed within ACA-Py can be really significant. This PR defines a minimized base message class that is unopinionated and trivial to extend.

This PR also addresses concerns around message serialization in anticipation of changes coming with DIDComm v2 by defining `serialize` and `deserialize` methods that specify the output/input format. At present, the `AgentMessage` class only implements DIDComm v1 message structure.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-01 02:35:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1132" class=".btn">#1132</a>
            </td>
            <td>
                <b>
                    fix: run_tests script
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Bluhm <dbluhm@pm.me>

Not sure what happened (perhaps related to Ubuntu 18.04 EOL?) but `run_tests` stopped working all of a sudden. This switches image base to `python:3.6.13`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-30 22:50:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1131" class=".btn">#1131</a>
            </td>
            <td>
                <b>
                    Add check after cred def created in integration test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

Adds small delay plus check that cred def was created (to address random failure of integration tests)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-30 15:43:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1130" class=".btn">#1130</a>
            </td>
            <td>
                <b>
                    feat: feedback from responder methods about message delivery
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As a result of some discussion in #950, I did a quick investigation of what it would look like to provide some feedback to the responder send methods about message delivery so that from the `forward` message handler, for example, we could determine whether the message was sent directly or not. This doesn't provide a ton of information but I think it provides just enough to know whether a push notification should be sent to a mobile device or not from the forward message handler, as @TimoGlastra described in the comments of that issue.

I think there are a lot of ways to end up at similar functionality though this one ended up being simpler than I anticipated. Interested to hear thoughts.

Signed-off-by: Daniel Bluhm <dbluhm@pm.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-30 14:27:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1129" class=".btn">#1129</a>
            </td>
            <td>
                <b>
                    fix: do not require indy or bbs to be installed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>

This should fix the issues with not having the indy and bbs libraries installed. There were a few offenders besides me for the indy library, but they should all be fixed now.

Fixes #1127
Fixes #1128 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-30 07:48:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1125" class=".btn">#1125</a>
            </td>
            <td>
                <b>
                    DIF Presentation Exchange and present-proof-v2 Updates
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
        Created At 2021-04-29 16:48:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1124" class=".btn">#1124</a>
            </td>
            <td>
                <b>
                    Fix: stateless record webhooks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This should hopefully address #1123.

### Changes
**fix: stateless records emit events**

Error on the side of caution for BaseRecord.emit_event, using topic
without state when none is given, and inserting the serialized record as
the payload if no payload is given.

Events are only not emitted by records when no record topic is set.

**fix: relax admin server record event pattern**

Should now accept stateless record event topics

**fix: add event namespace to base records to allow plugins to override**

**test: record topic parsing for webhook**
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-28 13:08:27 +0000 UTC
    </div>
</div>

