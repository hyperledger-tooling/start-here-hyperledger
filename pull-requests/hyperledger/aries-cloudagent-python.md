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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2223" class=".btn">#2223</a>
            </td>
            <td>
                <b>
                    Disable webhook trigger on initial response to multi-use connection invitation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Disable the webhook emitter when cloning a multi-use connection record, as it is "overhead": the webhook is fired once when the multi-use invitation is created, and subsequent interactions should only fire for subsequent updates of the new (cloned, contact-specific) connection record.

Fixes #2217 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-02 18:08:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2222" class=".btn">#2222</a>
            </td>
            <td>
                <b>
                    Fix formatting and grammatical errors in different readme's
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Noticed some of the docs contain formatting errors and could do with some improved grammar. Content stays the same with grammar fixed (shoutout to GPT-4)

Files improved:
- AdminAPI.md
- AnoncredsProofValidation.md
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-02 17:50:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2221" class=".btn">#2221</a>
            </td>
            <td>
                <b>
                    Fix broken link in README
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Link to the Trust Over IP framework PDF was broken, now fixed. All other links confirmed working
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-02 17:01:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2220" class=".btn">#2220</a>
            </td>
            <td>
                <b>
                    Update AriesOpenAPIDemo.md clarify callback can be one of webhook or websocket depending how agent is configured
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-27 16:22:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2219" class=".btn">#2219</a>
            </td>
            <td>
                <b>
                    Update Alice Wants a JSON-LD Credential to fix invocation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Addresses issue #2215
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-26 21:03:41 +0000 UTC
    </div>
</div>

