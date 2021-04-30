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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1120" class=".btn">#1120</a>
            </td>
            <td>
                <b>
                    allow for no body
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: sklump <srklump@hotmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-26 13:06:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1118" class=".btn">#1118</a>
            </td>
            <td>
                <b>
                    make long strings look like elsewhere in aca-py; cover new routes code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: sklump <srklump@hotmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-26 11:36:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1116" class=".btn">#1116</a>
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
                This is a PR that contains changes in endorser protocol.

The changes are defined in the issue
#1040 
#1028 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-24 11:13:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1115" class=".btn">#1115</a>
            </td>
            <td>
                <b>
                    Add generic JWE envelope handling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This decouples the in-memory pack/unpack from the envelope handling code, to allow other encryption methods in future.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-23 23:02:21 +0000 UTC
    </div>
</div>

