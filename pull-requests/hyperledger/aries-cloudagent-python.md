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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2698" class=".btn">#2698</a>
            </td>
            <td>
                <b>
                    fix: update constants in TransactionRecord
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves: #1650
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-04 22:28:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2696" class=".btn">#2696</a>
            </td>
            <td>
                <b>
                    Feature/emit did peer 4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Still requires manual testing, but similar implementation to did:peer:2.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-04 00:03:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2694" class=".btn">#2694</a>
            </td>
            <td>
                <b>
                    fix: save multi_use to the DB for OOB invitations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It was reported by a collegue that when using Out-of-band invitations with the connections handshake protocol, along with a public DID and connection re-use enabled, ACA-Py was only able to handle a single invitations. As if Connection Re-use wasn't working or the multi_use flag was ignored.

Turns out, we flat out weren't saving the multi_use flag to the database which is a big problem if you want to re-use the invitation. When DID-Exchanged is used, since DID-Exchange allows for a connection-less exchange of information. We only say the behaviour of the OOB Invitation getting deleted if we ran through the receive_reuse_message() method in the manager, which deletes the record if it's not set for multi_use.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-03 19:08:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2692" class=".btn">#2692</a>
            </td>
            <td>
                <b>
                    did peer 4 resolution
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Using https://github.com/decentralized-identity/did-peer-4.

based on the behaviour expected by the specification. 

https://identity.foundation/peer-did-method-spec/#method-4-short-form-and-long-form
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-02 21:26:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2690" class=".btn">#2690</a>
            </td>
            <td>
                <b>
                    Improve api documentation and error handling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add examples and descriptions to the swagger docs. Mostly used the indy examples.

There was some confusion with request params object attributes with camel vs snake casing. The anoncreds library does camel case like the spec decribes. Everywhere else has snake case. I changed everything so that only the inner anoncreds schema, cred_def and rev_reg_def objects are in camel case. I think this makes things a bit more clear but it is still a bit confusing when you are used to the indy api. 

I changed the POST rev_reg_def endpoint to have a wrapper like schema and cred_def with an options object where you can put the endorser connection id.

Changed the GET all creds defs return object to be in a wrapper like schemas.

Fixed a couple mistakes and improved the error handling. I think a majority of errors give information about the cause now. Can still get 500 errors with unexpected param values.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-29 19:16:17 +0000 UTC
    </div>
</div>

