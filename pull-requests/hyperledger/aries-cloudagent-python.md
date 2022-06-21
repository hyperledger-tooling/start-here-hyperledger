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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1827" class=".btn">#1827</a>
            </td>
            <td>
                <b>
                    Fix IssuerCredRevRecord state update on revocation publish
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1823 broken in #1804

Ran against integration tests T002-TAA and T003-TAA which were previously failing.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 22:16:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1824" class=".btn">#1824</a>
            </td>
            <td>
                <b>
                    Update POST /present-proof/send-request to POST /present-proof-2.0/send-request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                

I got error messages when following the instructions and tried the updated version, which worked.

Signed-off-by: lineko <36633510+lineko@users.noreply.github.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-19 17:58:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1820" class=".btn">#1820</a>
            </td>
            <td>
                <b>
                    Fix: Present Proof v2 - check_proof_vs_proposal update to support proof request with restrictions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.7.4</span>
            </td>
            <td>
                - resolve #1755 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-17 14:10:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1818" class=".btn">#1818</a>
            </td>
            <td>
                <b>
                    Add troubleshooting document, include initial examples - ledger connection, out-of-sync RevReg
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
        Created At 2022-06-16 18:56:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1817" class=".btn">#1817</a>
            </td>
            <td>
                <b>
                    Changelog, version and ReadTheDocs updates for 0.7.4-rc3 release
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
        Created At 2022-06-16 16:47:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1816" class=".btn">#1816</a>
            </td>
            <td>
                <b>
                    Fix missing webhook handler
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 13:44:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1813" class=".btn">#1813</a>
            </td>
            <td>
                <b>
                    Refactoring of revocation registry creation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updates the revocation registry initialization process.

Previously, an event was fired using `profile.notify`, which led to an `IssuerRevRegRecord` being created and the associated revocation registry being generated. Now, the `IssuerRevRegRecord` is created first, and then the event is fired, which leads to the registry generation. This allows the detection of a registry in progress and helps to avoid multiple revocation registries being created in parallel for the same credential definition.

Also, the tails file is now uploaded after the registry definition is posted and before the first entry is posted, instead of after the first entry is posted. This ensures that the registry doesn't enter the ACTIVE state until after the tails file is publicly available.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 03:26:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1812" class=".btn">#1812</a>
            </td>
            <td>
                <b>
                    Fix external Outbound Transport loading code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.7.4</span>
            </td>
            <td>
                As the code currently stands, only internal outbound transports are able to be loaded. With these changes, it should be possible to load a new outbound transport via a plugin.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 02:13:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1811" class=".btn">#1811</a>
            </td>
            <td>
                <b>
                    Fix: present-proof v1 send-proposal flow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.7.4</span>
            </td>
            <td>
                - resolve #1809 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 17:41:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1808" class=".btn">#1808</a>
            </td>
            <td>
                <b>
                    Fix put_file when the server returns a redirect
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.7.4</span>
            </td>
            <td>
                I believe this fix only applies to tails file uploads at the moment. Previously, aiohttp would encounter an error because it closed the tails file after the first attempt.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 00:40:53 +0000 UTC
    </div>
</div>

