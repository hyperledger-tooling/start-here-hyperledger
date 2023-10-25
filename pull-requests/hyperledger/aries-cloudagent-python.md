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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2562" class=".btn">#2562</a>
            </td>
            <td>
                <b>
                    Update demo/playground scripts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                To simplify (from the end user perspective) usage of the scripts leveraging the playground demo, I've docker-ized them; no more installing requirements (or python for that matter).

The scripts themselves are still simple, test that the playground agents are running, illustrate how to connect. When working on the mediator service, we added another script/test that would connect through the mediator service. 

I picked up this "technique" from @dbluhm when adding in anoncreds-rs. It was a great way to prove it all worked and illustrated the intended flow/usage.

This allows us to get rid of a `requirements.txt` and any PRs for dependabot on that file. Still have a poetry.lock, but those dependabot PRs seem to go smoother.

Closes #2555 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-24 23:50:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2561" class=".btn">#2561</a>
            </td>
            <td>
                <b>
                    refactor: use did-peer-2 instead of peerdid
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Speaking frankly, I felt that the peerdid library was a bit overly complicated. On top of that, peerdid is not up to date with the corrections proposed in this PR to the did:peer method specification:

https://github.com/decentralized-identity/peer-did-method-spec/pull/62

did-peer-2 is a minimal implementation of did:peer:2 and did:peer:3. It is up to date with the above PR. The corrections to the spec and the library lend themselves to a simpler implementation of the did:peer:2 and did:peer:3 resolvers. This refactor supports work to add did:peer:2 support to OOB + DID Exchange.

New in this PR is a cleanup mechanism for the did:peer:3 to did:peer:2 mapping records. When a connection is deleted, we check whether there are any potential mappings to remove.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-24 01:15:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2560" class=".btn">#2560</a>
            </td>
            <td>
                <b>
                    fix: clean up requests and invites
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                On connection deletion, all records strongly associated with the connection should be deleted. These records include connection metadata, connection requests, and connection invitations.

Records referencing the connection ID such as mediation or routing records are not "strongly" associated with the connection; there are other mechanisms in place to enable deletion of these records through the Admin API. The records for metadata, requests, and invitations, on the other hand, cannot be cleaned up any other way.

This PR makes sure these records are deleted when the connection is deleted.

It might be a good idea for us to look at other records that ought to be cleaned up automatically. Those can be addressed in future work.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-24 01:14:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2559" class=".btn">#2559</a>
            </td>
            <td>
                <b>
                    refactor: replace multiformats library
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This replaces the multiformats library with a very basic implementation included directly within ACA-Py. Given that the multiformats library has gone stale and my PR has languished, I think this is a good alternative to using that library. The implementation is very simple and currently only supports the minimum currently required by ACA-Py. Expanding the implementation in the future should be trivial.

Fixes #2501 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-19 15:19:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2558" class=".btn">#2558</a>
            </td>
            <td>
                <b>
                    Fix: RevRegEntry Transaction Endorsement
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #2441 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-19 14:32:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2554" class=".btn">#2554</a>
            </td>
            <td>
                <b>
                    fix: taa rough timestamp timezone from datetime
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2553
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-18 18:10:29 +0000 UTC
    </div>
</div>

