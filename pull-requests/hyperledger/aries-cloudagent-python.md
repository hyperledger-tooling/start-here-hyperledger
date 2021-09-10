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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1407" class=".btn">#1407</a>
            </td>
            <td>
                <b>
                    feature/inbound-transport-profile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When implementing a custom inbound transport there is no way to access settings through the profile. This PR adds a root profile to the `BaseInboundTransport` class that allows custom implemented inbound transports access to the profile provided to `InboundTransportManager`.

main changes:
- transport/inbound/base.py, now has a `root_profile` attribute.
- transport/inbound/manager.py,  passes profile into `register_transport`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 22:11:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1406" class=".btn">#1406</a>
            </td>
            <td>
                <b>
                    Fix aip 20 behaviour and other cleanup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes issue https://github.com/hyperledger/aries-cloudagent-python/issues/1333

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 20:51:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1405" class=".btn">#1405</a>
            </td>
            <td>
                <b>
                    Typos in the demo's README.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixed a few typos in the demo's README.md and changed the "ACA-Py" abbreviation to be consistent throughout the text.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 15:05:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1400" class=".btn">#1400</a>
            </td>
            <td>
                <b>
                    Run integration tests using external ledger and tails server
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
        Created At 2021-09-07 23:41:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1395" class=".btn">#1395</a>
            </td>
            <td>
                <b>
                    Connectionless proof demo
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
        Created At 2021-09-03 22:47:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1394" class=".btn">#1394</a>
            </td>
            <td>
                <b>
                    Implement get_credentials, credential_revoked for credx backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add test coverage for indy-credx issuance happy path
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-03 21:03:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1393" class=".btn">#1393</a>
            </td>
            <td>
                <b>
                    Import cleanups
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
        Created At 2021-09-03 18:47:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1392" class=".btn">#1392</a>
            </td>
            <td>
                <b>
                    fix: return type of inject
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Corrected the return type of these instances of `inject`. Apologies for missing these on the first pass.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-03 15:52:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1390" class=".btn">#1390</a>
            </td>
            <td>
                <b>
                    Add no-op handler for generic ack message (RFC 0015)
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
        Created At 2021-09-03 00:55:23 +0000 UTC
    </div>
</div>

