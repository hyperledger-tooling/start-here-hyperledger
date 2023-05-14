---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/842" class=".btn">#842</a>
            </td>
            <td>
                <b>
                    refactor maybe_known.rs: MaybeKnown enum
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - fixes #839 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-13 07:14:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/840" class=".btn">#840</a>
            </td>
            <td>
                <b>
                    Fix/protocols problem report
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR addresses #835 and #836, essentially adding a `ProblemReport` message to both the `IssueCredential` and `PresentProof` protocols.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-12 11:55:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/838" class=".btn">#838</a>
            </td>
            <td>
                <b>
                    Split publish_local_revocations in BaseAnoncreds
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Splits `publish_local_revocations` method associated with `BaseAnoncreds` trait into `get_rev_reg_delta` and `clear_rev_reg_delta` in order for `IndySdkAnonCreds` to not depend on a `PoolHandle`. Local revocations' publishing is now implemented in an already existing method associated with `RevocationRegistry` which exposes this functionality to the client code.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-12 07:54:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/837" class=".btn">#837</a>
            </td>
            <td>
                <b>
                    Add indy-vdr-proxy profile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds a new profile `VdrProxyProfile` which uses a running instance of [indy-vdr-proxy](https://github.com/hyperledger/indy-vdr/tree/main/indy-vdr-proxy) (through [indy-vdr-proxy-client](https://github.com/mirgee/indy-vdr/pull/1/files)) to read and write transactions instead of communicating with the ledger directly.

This may be useful in situations where
* a service is limited in its access to the public internet for security reasons or
* the client wants quick and easy access to a ledger without necessarily having to obtain the genesis file and set up and maintain their own ledger connection.

The `VdrProxyProfile` profile reuses existing `IndyVdrLedger` implementation of the `BaseLedger` trait and request submitting is injected through an implementation of the `RequestSubmitter` trait.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-10 13:03:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/833" class=".btn">#833</a>
            </td>
            <td>
                <b>
                    Fix/notification problem report
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As per the [RFC](https://github.com/hyperledger/aries-rfcs/tree/main/features/0015-acks#relationship-to-problem-report) the `ProblemReport` message can be a part of the `notification` message family (which only contains the `ack` message that's borrowed to other protocols).

This PR adds a `ProblemReport` message to the protocol to match the AFJ implementation (which is, technically, correct).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-09 13:23:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/832" class=".btn">#832</a>
            </td>
            <td>
                <b>
                    Remove extra warn log
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">skip-ios</span><span class="chip">skip-android</span><span class="chip">skip-napi-m1</span><span class="chip">skip-ci</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-09 09:58:36 +0000 UTC
    </div>
</div>

