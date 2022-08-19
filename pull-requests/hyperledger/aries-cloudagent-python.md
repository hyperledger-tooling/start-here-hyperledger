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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1904" class=".btn">#1904</a>
            </td>
            <td>
                <b>
                    Update for the v1.0.0-rc0 release. Changelog comment added for v0.7.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Update for the v1.0.0-rc0 release. Changelog comment added for v0.7.4
- Added this PR to changelog

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-18 19:41:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1902" class=".btn">#1902</a>
            </td>
            <td>
                <b>
                    fix: update RouteManager methods use to pass profile as parameter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adapt uses of `RouteManager` to pass the profile as argument.
This is following a refactoring in #1851

Signed-off-by: Clément Humbert <clement.humbert@sicpa.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-18 11:51:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1900" class=".btn">#1900</a>
            </td>
            <td>
                <b>
                    feat: added message to forward event handler
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Peter Strobel <peter@indicio.tech>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-16 19:32:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1899" class=".btn">#1899</a>
            </td>
            <td>
                <b>
                    Feat/public did endpoints for agents behind mediators
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR supports publishing endpoint information with routing keys in accordance with the did:sov specification. Routing keys are retrieved from `mediation_id` if specified, or else a default mediator. If no mediated connection is present, `routingKeys` defaults to an empty array. 

This PR allows for publishing DIDs with routing keys; PR #1863 allows for resolving DIDs with routing keys.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-15 23:23:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1897" class=".btn">#1897</a>
            </td>
            <td>
                <b>
                    Fixes a few AATH failures
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes:
- one 023-did-exchange error
- 0434-oob errors
- one 0183-revocation error

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-12 18:46:22 +0000 UTC
    </div>
</div>

