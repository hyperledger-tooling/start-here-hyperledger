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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1389" class=".btn">#1389</a>
            </td>
            <td>
                <b>
                    fix: typo in connection static result schema
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Bluhm <dbluhm@pm.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-02 20:22:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1387" class=".btn">#1387</a>
            </td>
            <td>
                <b>
                    fix: don't require push on outbound queue implementations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Requiring this method in concrete outbound classes should not be required -- this exact method signature is relevant only to redis. This probably should have been dropped with the outbound queue refactor but was missed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-02 18:21:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1383" class=".btn">#1383</a>
            </td>
            <td>
                <b>
                    Remove connection check on proof verify
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

Not required in general (if we are verifying a proof it means we have already received the proof) and causes an error on connectionless proof requests.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-01 16:23:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1382" class=".btn">#1382</a>
            </td>
            <td>
                <b>
                    Align OutOfBandManager.receive_invitation with other connection managers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Refactoring step before proposing changes in mediation connection
setup.

* Align `OutOfBandManager.receive_invitation` signature with the
  `ConnectionManager.receive_invitation` and
  `DIDXManager.receive_invitation`
    * rename first parameter to `invitation`
    * change return type to `ConnRecord` and leave serialization work
      for users of the manager

* Serialize the received `ConnRecord` in
  `protocols.out_of_band.v1_0.routes`

* Adapt related tests. `assert
  ConnRecord.deserialize(conn_rec)` is dubious as a test assertion but boiled down to `assert conn_rec
  is not None`.

* Use this refactoring to reduce branching in mediator connection
  handling in `conductor.py`.

Signed-off-by: Clément Humbert <clement.humbert@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-01 15:11:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1380" class=".btn">#1380</a>
            </td>
            <td>
                <b>
                    Pre release 0.7.1
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
        Created At 2021-08-31 23:14:22 +0000 UTC
    </div>
</div>

