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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1692" class=".btn">#1692</a>
            </td>
            <td>
                <b>
                    Multi-tenancy stale wallet clean up
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is intended to supersede #928. Due to significant changes since the original PR was opened, I cherry-picked a commit but had to modify it. History has not been well preserved, unfortunately. Credit to @TimoGlastra for the original work on the `ProfileCache` especially and for assistance in finding the solution implemented here.

This PR adds a LRU cache for profiles opened by `MultitenantManager` (corresponding to wallet types `indy` and `askar`, but not `askar-profile`). `weakref.finalize` is used to ensure the profiles are closed when they fall out of scope. An ordered dictionary of profiles holds a (strong) reference to the profile until it is evicted. If that profile happens to still be in use at the time it is evicted, it will not be closed until other (strong) references to it expire, i.e. after processing of a message or admin request has finished. This exact scenario is unlikely but possible.

In addition to this profile caching mechanism, I also updated a few aspects of the `BaseMultitenantManager` and its subclasses to make them more consistent with conventions used in ACA-Py.

Also, after being very confused by handling of askar profiles (not to be confused with `AskarProfile`s) within the `AskarProfileMultitenantManager` and `AskarProfile`, I did some light updates to (I hope) improve clarity.

A brief listing of known limitations:
- As implemented, the capacity of the LRU cache is statically defined as 100.
- A temporally based system for evicting profiles from the cache is likely better than a max capacity based system.
- 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-25 16:31:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1690" class=".btn">#1690</a>
            </td>
            <td>
                <b>
                    Fix: DIF proof proposal when creating bound presentation request [Issue#1687]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.7.4</span>
            </td>
            <td>
                Signed-off-by: Shaanjot Gill <shaangill025@users.noreply.github.com>
- resolve #1687 
- So the validation for `/present-proof-v2.0/send-proposal` is working but the problem was that with `auto_respond_presentation_proposal` flag on it would create an invalid bound request from the proposal [`input_descriptors` was not enclosed in `presentation_definition`]. I am surprised that I didn't catch this earlier.
- @swcurran According to the [RFC](https://github.com/hyperledger/aries-rfcs/blob/main/features/0510-dif-pres-exch-attach/README.md#examples-propose-presentation), the `propose-presentation` message only expects `input_descriptors` and no `options` [for `challenge` and/or `domain`]. With auto flag, there will be no opportunity to add a domain to the request, so I have updated the schema to allow `options` in the `propose-presentation` message. `challenge` is always required for verifying presentation, if `options` is not specified then it is randomly assigned.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-25 08:22:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1688" class=".btn">#1688</a>
            </td>
            <td>
                <b>
                    Remove references to play with von
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-24 17:05:34 +0000 UTC
    </div>
</div>

