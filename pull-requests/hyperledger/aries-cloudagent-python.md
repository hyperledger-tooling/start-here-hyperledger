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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1448" class=".btn">#1448</a>
            </td>
            <td>
                <b>
                    Endorser protocol updates - refactor to use event bus
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add a function to the protocol to (potentially) subscribe to events

Register/subscribe to all protocol events on aca-py startup

Add meta-data to the endorser transaction record to pass information downstream (e.g. save cred def revocation info so it's available to the revocation registry tasks)

(see https://hackmd.io/51flx8CVS1ypyOjEqVl1tg?view#Implementation-Details)

There are some issues when running with askar but I will deal with those on a separate PR

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-17 23:42:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1446" class=".btn">#1446</a>
            </td>
            <td>
                <b>
                    Add credential validation to offer issuance step
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This pull request adds an additional credential instance validation for any missing attributes. With this check eliminate errors at the issuance stage where in case of missing attributes, Aca-Py returns 500 error right now. And exchange record goes into a fault state.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-15 13:44:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1445" class=".btn">#1445</a>
            </td>
            <td>
                <b>
                    fix: help text for open-mediation flag
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Bluhm <dbluhm@pm.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-14 19:07:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1442" class=".btn">#1442</a>
            </td>
            <td>
                <b>
                    Add missing param to ws protocol
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
        Created At 2021-10-13 15:08:04 +0000 UTC
    </div>
</div>

