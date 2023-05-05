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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1446" class=".btn">#1446</a>
            </td>
            <td>
                <b>
                    feat: support for did:jwk and p-256, p-384, p-512
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
        Created At 2023-05-01 17:04:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1445" class=".btn">#1445</a>
            </td>
            <td>
                <b>
                    fix: Emit RoutingCreated event for mediator routing record
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added `RoutingCreatedEvent` emit after creation of mediator routing record in `MediatorService`.

This change is required to enable mediator functionality for tenant agents as `registerRecipientKeyForTenant` will not be called for mediator routing key otherwise (done in `RoutingCreatedEvent` listener).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-01 11:39:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1444" class=".btn">#1444</a>
            </td>
            <td>
                <b>
                    fix: migration of link secret
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
        Created At 2023-05-01 10:58:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1443" class=".btn">#1443</a>
            </td>
            <td>
                <b>
                    fix: small issues with migration and WAL files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Some small issues related to the migration script, mostly to do with write ahead logging.

Now the database is always copied with the optional wal file.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-01 10:13:28 +0000 UTC
    </div>
</div>

