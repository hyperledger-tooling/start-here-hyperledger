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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2861" class=".btn">#2861</a>
            </td>
            <td>
                <b>
                    feat: Add new format and implement VCDICredFormatHandler
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
        Created At 2024-03-31 14:10:33 +0000 UTC
    </div>
</div>

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

