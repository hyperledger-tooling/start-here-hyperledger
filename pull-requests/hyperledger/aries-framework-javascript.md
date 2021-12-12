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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/573" class=".btn">#573</a>
            </td>
            <td>
                <b>
                    build: add arm test ledger setup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Ledger setup didn't fully work for ARM baed macs. This PR adds an extra dockerfile that can be used to set up the test ledger on ARM macs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-11 15:22:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/571" class=".btn">#571</a>
            </td>
            <td>
                <b>
                    chore(release): v0.1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ci-test</span>
            </td>
            <td>
                Release version 0.1.0
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 10:47:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/566" class=".btn">#566</a>
            </td>
            <td>
                <b>
                    feat: expose wallet API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As a developer, I want to have more granular control of the wallet so that I can decide what flow to run in my business logic according to the state of the wallet. For example, I want to run a different branch (UI screens) of my code if the wallet does not exist without creating the wallet immediately.

I moved the creation of master secret into a create method. It should happen only once. It was unnecessarily called during every open wallet operation.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-07 14:58:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/565" class=".btn">#565</a>
            </td>
            <td>
                <b>
                    chore: disable unnecessary type check in Dispatcher test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jakub Koci <jakub.koci@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-07 14:42:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/564" class=".btn">#564</a>
            </td>
            <td>
                <b>
                    docs: Proofs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Initial documentation for dealing with Proofs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-07 08:45:08 +0000 UTC
    </div>
</div>

