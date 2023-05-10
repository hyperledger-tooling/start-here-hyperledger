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
                <span class="chip">skip-ci</span>
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/831" class=".btn">#831</a>
            </td>
            <td>
                <b>
                    this PR fixes #820 (Credential and Presentation attributes mime-type adjustments)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                as instructed AttrValue enum was created with two variants Plain and Encoded, the plain having { value: String } and Encoded with { value: String, mime_type: MaybeKnown<MimeType> }, which will facilitate in easy deserialization,

the AttrValue has been used in both the attributes (CredentialAttr and PresentationAttr), and the unit tests have been adjusted accordingly,

hope that this PR will solves the issue, any changes or feedback is welcomed

Thank You,
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-07 10:09:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/830" class=".btn">#830</a>
            </td>
            <td>
                <b>
                    Verifier presentation failure adjustments
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes an emerging problem regarding the verifier not doing anything in case the presentation verification fails (a problem report might be generated, but not sent, so the prover would be in the dark). 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-05 08:39:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/829" class=".btn">#829</a>
            </td>
            <td>
                <b>
                    First draft of new ledger traits
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">skip-ci</span>
            </td>
            <td>
                PR aimed towards solving #815 as well as refactoring the other core traits (Wallet, AnonCreds).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-04 07:25:47 +0000 UTC
    </div>
</div>

