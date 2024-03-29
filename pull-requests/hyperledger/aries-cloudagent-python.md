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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2860" class=".btn">#2860</a>
            </td>
            <td>
                <b>
                    Feature: use decorators for admin api authentication
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves #2318 

Opening draft PR early for feedback while I work through the changes across the code (and fixing/updating/adding tests as needed).

The PR removes the authentication middleware and the logic they deal with, and implements two decorators:

- `admin_authentication`: to be used for routes that should ONLY be invoked by an administrator, such as the multitenancy endpoints, the server endpoints and so on, independently of the mode the agent is running as.
- `tenant_authentication`: to be used to require authentication by either providing a tenant token (multi-tenant mode) or a valid api-key (single-tenant mode).

Both decorators account for unauthenticated `options` requests as well as insecure mode. Insecure paths will just not be decorated. Middleware code - currently commented-out - will be removed.

I think the bit of refactoring required for this to work (including plugins once released) is well worth the flexibility - looking for early feedback especially from @dbluhm, @ianco, @jamshale 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-28 19:48:30 +0000 UTC
    </div>
</div>

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

