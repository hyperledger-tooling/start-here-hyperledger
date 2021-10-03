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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1430" class=".btn">#1430</a>
            </td>
            <td>
                <b>
                    Selective Disclosure Check Fix - [Issue#1427]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #1427
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-01 14:34:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1429" class=".btn">#1429</a>
            </td>
            <td>
                <b>
                    Event bus Metadata
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This pr adds metadata to the event passed to an event handler. While writing a queue plugin that subscribes to events on the event bus a limitation of knowing what regular expression triggered the handler being called was identified. The event bus will call multiple handlers that match the subscribed regular expression. Currently, inside the handler, we must discover what regular expression triggered the event handler. The addition of metadata with the matched pattern in an event simplifies required logic in handlers that is error-prone.

Changes:
- event_bus.py 
  - added new EventMetaData and EventWithMetaData classes to add needed context to events
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-30 20:12:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1428" class=".btn">#1428</a>
            </td>
            <td>
                <b>
                    Update CONTRIBUTING.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-30 16:41:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1426" class=".btn">#1426</a>
            </td>
            <td>
                <b>
                    Add support for custom offers from the proposal
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## What is this PR for?

Currently, the issuer only has the ability to offer a credential that is the same as the one defined in a credential proposal. 
This PR enables the holder and issuer to negotiate about the credential via proposals and offers in order to agree on what credential the holder will receive.

### Backwards compatibility:

If the counter-offer is not defined/empty logic stays the same as It was before this change.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 12:34:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1425" class=".btn">#1425</a>
            </td>
            <td>
                <b>
                    WIP: Multiple Indy Ledger support, State Proof and leaf inclusion verification
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
        Created At 2021-09-27 16:11:53 +0000 UTC
    </div>
</div>

