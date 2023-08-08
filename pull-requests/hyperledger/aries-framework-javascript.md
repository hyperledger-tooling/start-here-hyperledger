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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1542" class=".btn">#1542</a>
            </td>
            <td>
                <b>
                    fix: listen to incoming messages on agent initialize not constructor
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
        Created At 2023-08-08 10:07:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1541" class=".btn">#1541</a>
            </td>
            <td>
                <b>
                    chore: DidCommV2: Sync with the main branch
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
        Created At 2023-08-06 09:41:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1540" class=".btn">#1540</a>
            </td>
            <td>
                <b>
                    fix: DidCommV2 - avoid breaking changes 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR aims to avoid breaking changes compared to the main branches.

- Preserved export of `AgentMessage` class which actually is `DidCommV1Message`. 
  - `AgentBaseMessage` is a common interface for V1/V2 - used internally
- Preserved name `Attachment` for DidCommV1 message attachments       
- Preserved name `SigningProvider`

Differences with the `main`
- `outOfBandInvitation` field of the OutOfBand record is optional
  - Reason: for DidCommV2 added separate field `v2OutOfBandInvitation`   
- `TransportSession` - `keys` and `inboundMessage`refers to different types but it should not break implementations.



TransportSession
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-04 07:49:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1538" class=".btn">#1538</a>
            </td>
            <td>
                <b>
                    feat: support askar profiles for multi-tenancy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds support for using askar profiles in multi-tenancy, so you don't have to create a new database for each tenant.

As commented on #1486, I've made some 'hacks' to make it work with the currrent API. I think extracting the wallet management from the wallet implementation can clean some things up, as well as having a more sophisticated wallet provider that is a bit more aware of having possible multilple wallets active at the same time within an agent.


The askar module now has a new `multiWalletDatabaseScheme` with two options: `ProfilePerWallet` or `DatabasePerWallet`. the database per wallet is the default to not make breaking changes, and profiel per wallet will reuse the same store for all wallets.

This is the only thing you have to do to benefit from this new feature. I've used the `initialize` method from the askar module to set everything up and register the askar `Store` from the root wallet to be used by the profile wallets. Not the cleanest, but I'm quite happy that it was at least possible to do this without significant changes.

The `AskarBaseWallet` exposes all wallet functionalitiy (such as signin, packing etc..) that is then extended by the `AskarWallet` (root / main wallet that also handles the connection to the database using a store) and `AskarProfileWallet` (uses an existing store and just creates / opens a session for a specific profile)

There's one issue I've discovered with profiles and sessions that requires a 'hack', maybe it can be fixed in Askar: https://github.com/hyperledger/aries-askar/issues/163
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-03 10:34:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1535" class=".btn">#1535</a>
            </td>
            <td>
                <b>
                    fix: force did:key resolver/registrar presence
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1528 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-01 23:53:17 +0000 UTC
    </div>
</div>

