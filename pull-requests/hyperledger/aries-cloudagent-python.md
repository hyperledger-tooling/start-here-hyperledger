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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2313" class=".btn">#2313</a>
            </td>
            <td>
                <b>
                    Add workaround for ARM based macs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - ARM based macs caused dependency issues with indy-vdr and ursa-bbs-signatures
- Solution checks for architecture and updates DOCKER_DEFAULT_PLATFORM
- Closes #2311 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-19 14:53:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2309" class=".btn">#2309</a>
            </td>
            <td>
                <b>
                    API endpoint to decommission revocation registry
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes issue #2304 

There are two active registries at a given time, this API endpoint - given a `cred_def_id` - will find and decommission the active revocation registries and will kick off the procedure to create new active registries (same as when a registry is full).

Note that the `pytest` doesn't have a handler to transition the `init` state registries to `active`, so we simulate that before testing the decommission code. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-18 02:12:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2308" class=".btn">#2308</a>
            </td>
            <td>
                <b>
                    Add .indy_client folder to Askar only image.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes https://github.com/hyperledger/aries-cloudagent-python/issues/2307
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-17 22:41:06 +0000 UTC
    </div>
</div>

