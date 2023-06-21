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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2273" class=".btn">#2273</a>
            </td>
            <td>
                <b>
                    Add replacement_id to API.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                create/create-offer, send/send-offer now have replacement_id in the POST body to set the id

Addresses #2218

`replacement_id` for [RFC-0453](https://github.com/hyperledger/aries-rfcs/tree/main/features/0453-issue-credential-v2) was half implemented, just needed to expose it to the API for the issuer to set the value.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-20 00:46:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2272" class=".btn">#2272</a>
            </td>
            <td>
                <b>
                    Minor revisions to the README.md and DevReadMe.md
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
        Created At 2023-06-16 19:22:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2269" class=".btn">#2269</a>
            </td>
            <td>
                <b>
                    Fix: Do not replace public verkey on mediator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes a case when public verkey of the mediated agent is removed from the keylists of its mediator during establishing a connection.

Assuming there is mediation established for an agent.
If the DID was promoted to public via POST /wallet/did/public?did={}&mediation_id={non_empty_id} then an ATTRIB 'endpoint' transaction was created on the ledger with the url pointing to the mediator and the respective routing_keys.

Next, the Inviter creates an invitation using the public=true (or use_public_did: true) flag, the communication of the Inviter goes through the mediator as it should. Then in the Inviter's accept-request phase, the public verkey is removed from the keylist of the mediator. 
That prevents any next attempts to answer to the Inviter's invitations with its public DID since the mediator does no longer have the routing key (verkey) associated to the public DID.

In conclusion, the public verkey must remain in the mediator as the routing key.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-15 14:11:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2268" class=".btn">#2268</a>
            </td>
            <td>
                <b>
                    Create .readthedocs.yaml file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add readthedocs YAML file as required by RTD.  Per this [blog post](https://blog.readthedocs.com/migrate-configuration-v2/), this file is now required for publishing the type of documentation we generate to the RTD sites. For those not aware, here is the link to the RTD site for ACA-Py -- https://aries-cloud-agent-python.readthedocs.io

Here is the link to the version of the docs generated from this branch with this new file: https://aries-cloud-agent-python.readthedocs.io/en/swcurran-add-rtd/. LGTM!
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-14 23:43:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2267" class=".btn">#2267</a>
            </td>
            <td>
                <b>
                    Add devcontainer for ACA-Py
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Addressing an issue where it is difficult to get set up to debug and begin coding by adding a devcontainer.

See Issue #2251 - this is only one small part of developer documentation. I wanted this out for feedback while we identify other areas of concern.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-14 23:36:28 +0000 UTC
    </div>
</div>

