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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1252" class=".btn">#1252</a>
            </td>
            <td>
                <b>
                    fix: check for expanded types in context checker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The checker method that checks for properties without a context was giving incorrect results for the vaccination context. This PR also checks if compaction expands a property as described in https://github.com/w3c-ccg/vaccination-vocab/issues/22


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-20 14:37:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1250" class=".btn">#1250</a>
            </td>
            <td>
                <b>
                    DIF PE - VCHolder backend-specific tag_query building and handle no given_id credentials
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Addresses the following from #1247, @andrewwhitehead will this meet the requirement? 
> As discussed, I think this tag filtering belongs in VCHolder so that it can be specialized for the specific backends, but it's fine to merge this as-is and I can revisit it later with the shared-components work. Most important is that it works for now.
- resolve #1253 [work in progress]
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-19 21:03:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1249" class=".btn">#1249</a>
            </td>
            <td>
                <b>
                    Update get/set_did_public to use a storage record pointer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This should be much faster when there are many DIDs stored in the wallet.

The 'public' DID metadata property is now generally ignored except when auto-upgrading an existing wallet. The `get_posted_dids` method is updated to NOT filter the public DID, as it did previously.

Includes a couple fixes for warnings when running tests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-17 03:45:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1248" class=".btn">#1248</a>
            </td>
            <td>
                <b>
                    fix: delete metadata on connection deletion
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
        Created At 2021-06-17 02:46:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1247" class=".btn">#1247</a>
            </td>
            <td>
                <b>
                    DIF PE Updates and present_proof_v1_0 OOB Attachment Fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #1244 
- resolve #1242 
- resolve #1240 
- present_proof_v1 and OOB attachment fix
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-16 03:07:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1246" class=".btn">#1246</a>
            </td>
            <td>
                <b>
                    Add endorser protocol support for revocation functionality 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds endorser protocol support for revocation functionality such as:
- publishing a revocation registry definition to the ledger
- publishing a revocation entry to the ledger
It is based on #1230, so that PR should likely be merged first.c.c: @ianco 

Currently, if endorsing is requested the agent will NOT handle the generation and rotation of the revocation registry for the user. Improvements to the usability are necessary, see #1238 for reference.

A set of BDD tests validating the end-to-end flow has been added.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-15 00:28:04 +0000 UTC
    </div>
</div>

