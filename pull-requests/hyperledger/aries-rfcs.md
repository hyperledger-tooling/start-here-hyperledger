---
layout: default
title: aries-rfcs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-rfcs
---

# aries-rfcs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-rfcs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/652" class=".btn">#652</a>
            </td>
            <td>
                <b>
                    WIP - RFC0510: updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * presentation_definitions -> presentation_definition
* add `options` object
* add option for BbsBlsSigantureProof2020
* add `nonce` option for BbsBlsSignatureProof2020
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-04 20:46:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/651" class=".btn">#651</a>
            </td>
            <td>
                <b>
                    Added Method 2 to Static Peer DIDs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As Discussed in last week's WG meeting.
Signed-off-by: Sam Curren <telegramsam@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-04 16:04:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/650" class=".btn">#650</a>
            </td>
            <td>
                <b>
                    Changed public DID language, removed GUID requirement in URL
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As discussed in our WG meeting last week.
Signed-off-by: Sam Curren <telegramsam@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-04 14:36:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/649" class=".btn">#649</a>
            </td>
            <td>
                <b>
                    0183 revocation notification AIP v2 changes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Small changes for AIP v2 as discussed on Aries call, including sync with please-ack decorator and describe meaning of OUTCOME in this context
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 22:22:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/646" class=".btn">#646</a>
            </td>
            <td>
                <b>
                    add 0646: W3C Credential Exchange using BBS+ Signatures
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">AIP 2.0</span>
            </td>
            <td>
                Initial draft PR. Still needs some things resolved and would be best if we merge it after the issues discussed at IIW are resolved. This mainly involves updating the BBS+ LD Proofs spec and defining how private holder binding can be achieved.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-28 16:35:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/645" class=".btn">#645</a>
            </td>
            <td>
                <b>
                    fix incorrect thid wording in did exchange RFC
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As discussed on the WG call a few weeks ago. The did exchange protocol required the `thid` property to be equal to the message ID. This is an unnecessary restriction
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-28 15:39:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/644" class=".btn">#644</a>
            </td>
            <td>
                <b>
                    simplify please ack decorator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">AIP 2.0</span>
            </td>
            <td>
                Simplify please ack decorator for inclusion in AIP 2.0 (#632). I simplified it to the most basic version where you can only indicate whether you want an ack on RECEIPT or OUTCOME. 

I'm not sure if I removed too much, but I think this basic variant will be quite easy to implement for agents, while still providing a lot of value.

@dhh1128 as the original author of the RFC, what do you think?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-28 15:29:02 +0000 UTC
    </div>
</div>

