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

In draft state, need to write some tests.
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2305" class=".btn">#2305</a>
            </td>
            <td>
                <b>
                    Fix alice/faber demo execution
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds the `--debug-webhooks` flag for all demo agents, as it is required to distinguish between credential offers and presentation requests for different credential types.

It also works around an issue with #2234 which causes the agents to exit with a RuntimeError due to the call to `loop.run_until_complete` within the logging configuration. I think a more complete fix might be to use a ContextVar to store the current DID identifier and set that when a tenant context is initialized, to avoid any async operations in the logger config.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-12 21:03:40 +0000 UTC
    </div>
</div>

