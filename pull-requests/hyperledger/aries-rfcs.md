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
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/805" class=".btn">#805</a>
            </td>
            <td>
                <b>
                    Aries RFC Index Update - 20231206
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-06 22:56:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/804" class=".btn">#804</a>
            </td>
            <td>
                <b>
                    Proposes the DIDComm RPC Protocol for App Attestation and more
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The DIDComm Remote Procedure Call (DRPC) protocol enables a [JSON-RPC]-based request-response interaction to be carried out across a DIDComm channel. The protocol is designed to enable custom interactions between connected agents, and to allow for the rapid prototyping of experimental DIDComm protocols. An agent sends a DIDComm message to request a remote service be invoked by another agent, and gets back a response in subsequent DIDComm message. The protocol enables any request to be conveyed that the other agent understands. Out of scope of this protocol is how the requesting agent discovers the services available from the responding agent, and how the two agents know the semantics of the [JSON-RPC] requests and responses. By using DIDComm between the requesting and responding
agents, the security and privacy benefits of DIDComm are accomplished, and the generic parameters of the messages allow for flexibility in how and where the protocol can be used.

[JSON-RPC]: https://www.jsonrpc.org/specification

The initial proposed use of this protocol is for App Attestation.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-05 20:01:28 +0000 UTC
    </div>
</div>

