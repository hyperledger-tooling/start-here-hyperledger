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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2732" class=".btn">#2732</a>
            </td>
            <td>
                <b>
                    0.12.0rc0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                @dbluhm -- note the update in the documentation for the DID Resolver documentation. I assume that is OK, but didn't actually try it.  I'll try to get to that. I wanted to keep the version updated so that it will be found in a repo search as we publish new releases.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-23 21:08:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2731" class=".btn">#2731</a>
            </td>
            <td>
                <b>
                    Relax validation of holder DID when submitting a credential request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See issue https://github.com/hyperledger/aries-cloudagent-python/issues/2714

Relax validation to allow did:peer (or any value) for the holder/prover did on a credential request.

This works with an askar wallet, but anoncreds-askar will fail due to its own did validation (see issue https://github.com/hyperledger/anoncreds-rs/issues/307)

This PR will work once the anoncreds-rs issue is also fixed.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-23 19:41:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2729" class=".btn">#2729</a>
            </td>
            <td>
                <b>
                    Update devcontainer documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Most of the documentation was pretty good but I tried to make it more obvious that this is a good option.

- I added more configurations to make it more obvious you can deploy multiple agent debug sessions. 
- You don't actually need to expose ports to access the admin api so I removed that stuff.
- If you run your von-network and tails server from inside the dev container you can use local host and all the webhooks work as well.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-19 21:30:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2723" class=".btn">#2723</a>
            </td>
            <td>
                <b>
                    Remove exception on connectionless presentation problem report handler
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is to support being able to get callbacks to [vc-authn-oidc](https://github.com/bcgov/vc-authn-oidc) when a user declines the presentation request sent to their agent.

Presently ACA-PY is throwing an exception if the problem report does not contain a connection record.
Remove that exception and allow the recieve_problem_report to continue (and supply None for the connection ID in that case).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-17 23:16:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2722" class=".btn">#2722</a>
            </td>
            <td>
                <b>
                    Update the SupportedRFCs Document to be up to date
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I'd welcome feedback on this on other things we want to highlight in this document.

@dbluhm @andrewwhitehead @ianco, do you think these AIP 2.0 comments are still accurate:

| RFC | Supported | Notes |
 --- | :--: | -- |
| [0211-route-coordination](https://github.com/hyperledger/aries-rfcs/tree/b3a3942ef052039e73cd23d847f42947f8287da2/features/0211-route-coordination)   | :warning:  | Only pre-AIP 2.0 version. Must be updated to use `did:key` for full AIP 2.0 support  |
| [0360-use-did-key](https://github.com/hyperledger/aries-rfcs/tree/b3a3942ef052039e73cd23d847f42947f8287da2/features/0360-use-did-key)     | :warning:  |  Creating and resolving `did:key` DIDs is supported, but not all protocols are updated yet to use `did:key`. This is a breaking change for AIP 1.0 -> AIP 2.0.                |
| [0587-encryption-envelope-v2](https://github.com/hyperledger/aries-rfcs/tree/b3a3942ef052039e73cd23d847f42947f8287da2/features/0587-encryption-envelope-v2) | :construction: | Support for the DIDComm V2 envelope format is a work in progress, including the PRs ([AIP-2 base64url consistency](https://github.com/hyperledger/aries-cloudagent-python/pull/1188) and [Small AIP-2 updates](https://github.com/hyperledger/aries-cloudagent-python/pull/1056)) |

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-17 22:54:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2721" class=".btn">#2721</a>
            </td>
            <td>
                <b>
                    Fix subwallet record removal
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If subwallet initialization fails (for example due to an invalid wallet key: #2682) then the wallet record is meant to be removed. This could fail because a session was not being opened first.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-17 22:06:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2720" class=".btn">#2720</a>
            </td>
            <td>
                <b>
                    Breaking - remove endorser capability to write ledger transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                WIP as I am still testing the changes.

I didn't remove the "request endorser to write transaction" flag.  In the author I hardcode to false.  In the endorser I raise an error if the author requests this function.  (Handles the case where the endorser is updated and the author isn't.)

See issue #2711 

There is some work to do on problem reports, I added a separate Issue for this task.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-17 21:44:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2719" class=".btn">#2719</a>
            </td>
            <td>
                <b>
                    Upgrade anoncreds to 0.2.0.dev7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Used an exact version of the dev pre-release. Figured is would be changed anyway when this becomes non pre-release. 

Fixed some calls to the anoncreds library. Required fetching some additional objects from the wallet. Fixed the unit tests.

These would have been quicker and easier to fix if the unit tests caught them. For some of the unit tests I was able to interact with anoncreds and create objects with it, but for some objects like creating credentials and revocation registries I was mocking the objects. These ended up being the broken calls so only the integration tests caught them.

Would be nice if the unit tests could create all the anoncreds objects instead of mocking them. Will try and do this more when I see the opportunity. 

Changed the devcontainer poetry version to match the version used to upgrade.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-17 18:28:23 +0000 UTC
    </div>
</div>

