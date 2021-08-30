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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/340" class=".btn">#340</a>
            </td>
            <td>
                <b>
                    Support invitation messages with public DID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                Moved from [here](https://github.com/hyperledger/aries-vcx/pull/7).

Adds libvcx API:

### Pubic agents
- `vcx_public_agent_create` - create new public agent 
- `vcx_public_agent_generate_public_invite` - generate public DID based invitation with custom label
- `vcx_public_agent_serialize` - serialize public agent info
- `vcx_public_agent_deserialize` - deserialize public agent info into an Public Agent object
- `vcx_public_agent_release`- release Public Agent object from libvcx memory state

### Connections
- `vcx_connection_create_with_connection_request` - create new Connection from Aries "Connection Request" message

# Workflow
The idea is
- Create "public agent" in Agency, write its info on ledger under your public DID
- Generate Connection Invitation containing your DID
- Publish Connection Invitation somewhere publicly (for example as QR code). Anyone can see, use it, scan it.
- Check your Public Agent for newly received Aries messages of "Connection Request" type
- For each new "Connection Request", create new Connection object and progress the aries connection protocol as usual
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-23 12:47:38 +0000 UTC
    </div>
</div>

