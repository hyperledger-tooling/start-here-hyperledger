---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1024" class=".btn">#1024</a>
            </td>
            <td>
                <b>
                    chore(release): v0.2.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ci-test</span>
            </td>
            <td>
                Release version 0.2.4
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-10 14:07:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1021" class=".btn">#1021</a>
            </td>
            <td>
                <b>
                    feat(proofs): delete associated didcomm messages 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves #860 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-08 20:07:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1020" class=".btn">#1020</a>
            </td>
            <td>
                <b>
                    feat(proofs): proofs module migration script for 0.3.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #996
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-08 19:58:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1019" class=".btn">#1019</a>
            </td>
            <td>
                <b>
                    fix: avoid crash when an unexpected message arrives
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Pavel Zarecky <zarecky@procivis.ch>

This catch block is added to avoid potential crash, when an unexpected message arrives from a connection.

See #1018

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-08 11:27:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1017" class=".btn">#1017</a>
            </td>
            <td>
                <b>
                    feat: Added baseMediatorReconnectionIntervalMs and maximumMediatorReconnectionIntervalMs to Agent configuration for controlling back off strategy on mediator reconnection
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sergi Garreta <sergi.garreta@entrust.com>

Fixes Issue #1002 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-07 13:40:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1016" class=".btn">#1016</a>
            </td>
            <td>
                <b>
                    chore: add @janrtvld to maintainers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add @janrtvld to maintainers as discussed in [Discord](https://discord.com/channels/905194001349627914/941708033434738768/1016248809589850132).

Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-07 07:24:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1014" class=".btn">#1014</a>
            </td>
            <td>
                <b>
                    feat: problem report on decline
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Waiting on Author</span>
            </td>
            <td>
                Adds a new problem report reason for credential / presentation decline and sends a problem report when declining an offer or request. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-06 18:13:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1013" class=".btn">#1013</a>
            </td>
            <td>
                <b>
                    fix(ledger): check taa version instad of aml version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1010 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-06 11:59:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1011" class=".btn">#1011</a>
            </td>
            <td>
                <b>
                    fix(ledger): remove poolConnected on pool close
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes issue where cannot reconnect to ledger after rotating wallet key

Signed-off-by: Niall Shaw <niall.shaw@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-06 07:34:36 +0000 UTC
    </div>
</div>

