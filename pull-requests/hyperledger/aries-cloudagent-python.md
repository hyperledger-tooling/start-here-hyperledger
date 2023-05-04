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
                I noticed some of the docs contain formatting errors and could do with some improved spelling/grammar. Content stays the same.

List of files changed:

Very minor linting improvements, such as indenting or languages added for better code block formatting:
- DIDMethods.md
- DIDResolutions.md
- Multitenancy.md
- UnitTests.md

Spellchecked as well (shoutout to GPT-4):
- AdminAPI.md
- AnoncredsProofValidation.md
- UsingOpenAPI.md

There are too many readme's to make a bunch more minor edits. Most others seem fine, but these above could do with improvement
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

