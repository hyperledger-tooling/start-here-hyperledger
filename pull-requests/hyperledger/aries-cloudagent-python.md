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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2236" class=".btn">#2236</a>
            </td>
            <td>
                <b>
                    Add updated ELK stack for demos.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Remove outdated EFK stack and update documentation.

This is a restore for https://github.com/hyperledger/aries-cloudagent-python/pull/2216. Resetting / merging my repo branch rolled back the commits, so #2216 PR is empty.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-18 17:41:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2235" class=".btn">#2235</a>
            </td>
            <td>
                <b>
                    refactor: Extract verification method ID generation to a separate class
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently, the strategy to generate the verification key IDs only supports an arbitrary set of DID methods, and the IDs are derived from hardcoded strings, which can be too restrictive for some use cases.

For example, if one adds DID methods (such as did:web) using third-party plugins, the current method will always raise an error. Also, one might want to have more advanced ways of deriving the verification key ID, for example when multiple verification methods are used for a given DID and are rotated regularly.

This PR allows for more flexibility by extracting the verification key ID generation to a separate class so that plugins can switch implementations depending on the needs using injection. For example, for the key rotation use-case cited above, the implementation could be switched to one that dynamically returns the correct verkey ID, even if different did methods are used. I believe this solution avoids breaking changes, and keeping the current strategy as the default one allows keeping backward compatibility.

Let me know if you have any comments/suggestions.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-17 15:42:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2234" class=".btn">#2234</a>
            </td>
            <td>
                <b>
                    Allow Log Access at Tenant Level
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve https://github.com/bcgov/DITP/issues/23
- Built on top of #2233
- Allows writing of logs with `logger_alias` [tenant identifier] to a specified file, in addition to console output [same as before]
- It is responsibility of the controller to ingest/consume this logs in ELK stack and then be able to query by tenant identifier.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-16 14:24:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2233" class=".btn">#2233</a>
            </td>
            <td>
                <b>
                    Allow Configuration Settings on a per-tenant basis
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #2209
- Some changes related to getting `BaseLedger` instance from `ledger_id` won't be used right now but will be used soon with some proposed Traction features.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-16 14:05:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2232" class=".btn">#2232</a>
            </td>
            <td>
                <b>
                    Multi-tenant self-managed mediation verkey lookup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes #2231 

There are two ways to setup mediation for multitenancy. One is to have the base wallet mediate for all tenants, and the second is for each tenant to manage their own. In the second case, there was a bug when locating the verkey and packing the outbound message.

This PR checks if the base wallet is mediating and decides which responder to use. If the tenant is managing their own mediation then we need the sub-wallet profile to create the responder NOT the base wallet profile.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-12 18:15:50 +0000 UTC
    </div>
</div>

