---
layout: default
title: identus-cloud-agent
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/identus-cloud-agent
---

# identus-cloud-agent <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/identus-cloud-agent){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    Identus Cloud Agent v1.33.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    cloud-agent-v1.33.0
                </span>
            </td>
            <td>
                #### New features
- First iteration of renaming PRISM Agent to Cloud Agent within Identus project
- Use ZIO Failures and Defects effectively + RFC-9457 in connect
- Verification API for Verifiable Credentials
- Support Ed25519 and X25519 key type of managed DID via curve parameter when managing DID using REST interface

#### Bug fixes 
- Check purpose of the keys and fix the fact that issuers DID without purpose "assertionMethod" can issue VC and API does not fail although logs show failure under the hood
- Add shared-crypto module and apollo wrapper for other key types
- Use Apollo for secp256k1 in shared-crypto
- Add missing 'PresentationVerificationFailed' status
- Expose pg_admin port on the localhost interface only
- Remove prism-crypto dependency
- Update Open-api-spec and Generator script to use new Identus naming
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/identus-cloud-agent/releases/tag/cloud-agent-v1.33.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-05-09 04:14:38 +0000 UTC
    </span>
</div>

