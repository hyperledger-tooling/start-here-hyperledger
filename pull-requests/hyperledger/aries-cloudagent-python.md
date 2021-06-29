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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1275" class=".btn">#1275</a>
            </td>
            <td>
                <b>
                    Update bdd tests to support askar; fix ledger method signatures
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Ledger methods are updated to provide endorser support for revocation updates

bdd updates are to allow tests to be run using askar wallet

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-28 21:18:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1274" class=".btn">#1274</a>
            </td>
            <td>
                <b>
                    Add `wait_for_event` method on event bus
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We've found this to be generally useful in some of our coding efforts and after a brief discussion with @esune noting that it would be of use in some of his ongoing work, we figured it would be good to pop this out of our ongoing work so it can be used elsewhere.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-28 20:01:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1273" class=".btn">#1273</a>
            </td>
            <td>
                <b>
                    Fix manual event handling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

Fixes the OpenAPI example

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-28 20:00:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1272" class=".btn">#1272</a>
            </td>
            <td>
                <b>
                    Connection protocol used in ConnRecord
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Now able to tell if a ConnRecord was created using `0160`, `0023` and `0023 with didcomm v2 envelope` [in future]
- Should fix AATH connection tests, as `connection_protocol` can be used instead of relying on `missing invitation_msg_id` which is no longer the case as to support connection_reuse [`RFC 0434`]
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-28 18:00:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1267" class=".btn">#1267</a>
            </td>
            <td>
                <b>
                    Add support for shared components
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add `indy-vdr` ledger client
- Add `indy-credx` credential handling
- Add `aries-askar` storage backend

The `performance`, `alice`, and `faber` demo agents should all support the `--wallet-type askar` argument for testing with the new backend components, as does the agent itself when run with `aca-py`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-25 03:17:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1266" class=".btn">#1266</a>
            </td>
            <td>
                <b>
                    Fix performance demo, clean up some warnings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-24 20:53:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1265" class=".btn">#1265</a>
            </td>
            <td>
                <b>
                    OOB- 0160 connection reuse fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Should fix `HandshakeReuse validation failed` error when trying to reuse 0160 connection [public_did]
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-24 16:43:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1259" class=".btn">#1259</a>
            </td>
            <td>
                <b>
                    fix: credentials must specify additional types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                While writing test for AATH I noticed in the vc-data-model section on [types](https://www.w3.org/TR/vc-data-model/#types), the following excerpt:

> All credentials, presentations, and encapsulated objects MUST specify, or be associated with, additional more narrow types (like UniversityDegreeCredential, for example) so software systems can process this additional information.

This is also tested in the vc-test-suite: https://github.com/w3c/vc-test-suite/blob/gh-pages/test/vc-data-model-1.0/10-basic.js#L95-L99

This PR adds this restriction to the validation of VCs in ACA-Py
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-23 16:15:01 +0000 UTC
    </div>
</div>

