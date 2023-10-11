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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2544" class=".btn">#2544</a>
            </td>
            <td>
                <b>
                    fix: correct minor typos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes some minor spelling typos:

   Congradulations -> Congratulations
   explicitely -> explicitly
   supprting -> supporting

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-11 13:33:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2541" class=".btn">#2541</a>
            </td>
            <td>
                <b>
                    Anoncreds-rs pytest update (Credential Definitions)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is the first set of updates for credential definitions API only.

Since we have not updated/implemented endorser in the anoncreds-rs branch, I have left endorser related tests as skipped.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-09 18:30:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2540" class=".btn">#2540</a>
            </td>
            <td>
                <b>
                    DRAFT: PleaseAck.md document
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is an attempt to make a start point of discussion how to implement the `please_ack` decorator support in ACA-Py. The PR contains initial version of the document that aims to find the final solution. It contains some thoughts/ideas about possible implementations.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-09 18:19:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2539" class=".btn">#2539</a>
            </td>
            <td>
                <b>
                    0.10.4
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
        Created At 2023-10-09 14:21:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2537" class=".btn">#2537</a>
            </td>
            <td>
                <b>
                    fix (backport): routing behind mediator 
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
        Created At 2023-10-08 00:07:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2536" class=".btn">#2536</a>
            </td>
            <td>
                <b>
                    fix: routing behind mediator 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a reopen of PR #2535 (after I botched my git command...). Thanks again @codespree for the fix.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-07 19:56:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2533" class=".btn">#2533</a>
            </td>
            <td>
                <b>
                    refactor: make ldp_vc logic reusable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is a refactor of LDP VC handling within ICv2 and PPv2 to make it usable outside of those protocol's handlers. I believe this results in a cleaner implementation, separating the concerns of preparing a credential from the ICv2 protocol and its messages and handlers for those messages.

This refactor enables the other major addition in this PR, adding a couple of new endpoints for LDP VC issue and verify, `POST /vc/ldp/issue` and `POST /vc/ldp/verify`. These endpoints are similar to the `/jsonld/sign` and `/jsonld/verify` endpoints. However, the big difference is that the `/jsonld` endpoints did not use the same LDP signing methods used in ICv2 or PPv2. This has caused the two implementations to diverge more and more over time. With this PR, these endpoints are still available but are marked as deprecated. One other significant difference, the inputs for endpoints have changed to be more specific to signing and verifying LDP VCs and not just arbitrary JSON-LD documents.

Fixes #2468.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-05 18:59:39 +0000 UTC
    </div>
</div>

