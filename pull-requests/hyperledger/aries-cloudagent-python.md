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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2858" class=".btn">#2858</a>
            </td>
            <td>
                <b>
                    fix: states for discovery record to emit webhook
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds states to the the Discover Features record in order to trigger emitting webhooks containing the disclosed features to the controller. Without this change, retrieving the supported features of the remote agent is _extremely_ inconsistent. You just have to hope that the disclosure comes back in 5 seconds or try doing an exponential back off polling of the discover feature record to see if it showed up.

And a few other simplifications.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-26 18:45:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2856" class=".btn">#2856</a>
            </td>
            <td>
                <b>
                    chore: propose official deprecations of a couple of features
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                With this PR I'd like to propose that we move the following features to deprecated status:

- Aries RFC 160: Connection Protocol
- Aries RFC 0036: Issue Credential 1.0
- Aries RFC 0037: Present Proof 1.0
- `did:sov:...` as Protocol Doc URI

By moving these to deprecated status, we inform the community that these are features that should no longer be used and steer them to DID Exchange and using didcomm.org as the doc uri in their projects.

These items should more or less already be considered deprecated but there are some final efforts that need to be made to tie up loose ends. With the introduction of qualified DIDs in the pending 0.12.0 release and automatically always emitting https://didcomm.org (by setting the flag for it to be permanently set to `true`), we move close enough to these loose ends being tied off to, in my opinion, move these features to official deprecated status.

In practice, this PR affects the code in the following ways:

- Prints a deprecation notice on startup (to stderr) that these features are now deprecated.
- When a message with type starting with `did:sov:` is received, log a deprecation warning
- When a connection protocol operation is taken, log a warning message (this one might be a bit aggressive; I'd be happy to tone this back if it's too much)
- Mark the Admin API endpoints as deprecated in the OpenAPI/Swagger spec and UI. The endpoints are still usable but are greyed out.
  - To clarify, only the Admin API endpoints triggering connection protocol specific operations are marked as deprecated. Other connection management endpoints are NOT marked as deprecated (e.g. listing connections, deleting a connection, etc.).

Let me know your thoughts.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-22 21:54:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2854" class=".btn">#2854</a>
            </td>
            <td>
                <b>
                    Increase promote did retries
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Doh! I think I must have accidentally deleted the wait in between retries somehow and not noticed.

Hopefully this should prevent the errors during promote did.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-22 17:00:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2853" class=".btn">#2853</a>
            </td>
            <td>
                <b>
                    Change did <--> verkey logging on connections
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See https://github.com/hyperledger/aries-cloudagent-python/issues/2846
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-22 16:51:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2852" class=".btn">#2852</a>
            </td>
            <td>
                <b>
                    Update GHA so that broken image links work on docs site - without breaking them on GitHub
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Links to images are different when the markdown page is displayed by GitHub vs. when deployed as documentation. Fix the links on the fly as the mkdocs site is created.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-22 15:14:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2850" class=".btn">#2850</a>
            </td>
            <td>
                <b>
                    fix: did exchange multiuse invites respond in kind
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes: #2817 

DID Exchange was responding incorrectly to requests, sending unqualified DIDs with a `did_rotate~attach` (which is nonsensical). This fixes it to only send a `did_rotate~attach` when the DID associated with the connection is a qualified DID. Additionally, this change also ensures that the webhook for the new connection request will only be emitted after the request has been attached to the connection record. Without this, a race condition can occur for controllers that try to accept the request before ACA-Py finishes storing the request.

As a side note, I left a todo wondering out loud about whether the webhook for the newly created connection record (the one that gets generated from a multi-use connection record) should happen at all.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-21 17:15:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2849" class=".btn">#2849</a>
            </td>
            <td>
                <b>
                    Prevent revocable cred def being created without tails server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Addresses https://github.com/hyperledger/aries-cloudagent-python/issues/2838.

Simply returns an error response when creating a revocable cred def without a tails file configured. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-21 16:04:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2848" class=".btn">#2848</a>
            </td>
            <td>
                <b>
                    Minor updates to the documentation - links, navigation and markdown
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-21 15:58:45 +0000 UTC
    </div>
</div>

