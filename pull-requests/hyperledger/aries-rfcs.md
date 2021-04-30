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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/643" class=".btn">#643</a>
            </td>
            <td>
                <b>
                    Add ECDH-ES for Anoncrypt in Envelope v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">AIP 2.0</span>
            </td>
            <td>
                Signed-off-by: Troy Ronda <troy@troyronda.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-26 20:40:36 +0000 UTC
    </div>
</div>

