---
layout: default
title: open-enterprise-agent
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/open-enterprise-agent
---

# open-enterprise-agent <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/open-enterprise-agent){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/961" class=".btn">#961</a>
            </td>
            <td>
                <b>
                    feat: Signature, Not Before, Expiration, Schema Verification API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span>
            </td>
            <td>
                https://input-output.atlassian.net/browse/ATL-6788
https://input-output.atlassian.net/browse/ATL-6780
https://input-output.atlassian.net/browse/ATL-6774
https://input-output.atlassian.net/browse/ATL-6781
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-09 02:50:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/960" class=".btn">#960</a>
            </td>
            <td>
                <b>
                    ci: update the release commit message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">build</span>
            </td>
            <td>
                The signer is changed from Anton to Allain

### Description: 
Summarize the changes you're submitting in a few sentences, including Jira ticket ATL-xxxx if applicable.
Link to any discussion, related issues and bug reports to give the context to help the reviewer understand the PR.

### Alternatives Considered (optional): 
Link to existing ADR (Architecture Decision Record), if any. If relevant, describe other approaches explored and the selected approach. Documenting why the methods were not selected will create a knowledge base for future reference, helping prevent others from revisiting less optimal ideas.

### Checklist: 
- [ ] My PR follows the [contribution guidelines](https://github.com/hyperledger-labs/open-enterprise-agent/blob/main/CONTRIBUTING.md) of this project
- [ ] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [ ] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-08 14:21:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/959" class=".btn">#959</a>
            </td>
            <td>
                <b>
                    feat: VC Verification Abstraction
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">prism-agent</span>
            </td>
            <td>
                ### Description: 
https://input-output.atlassian.net/browse/ATL-6447
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-08 03:55:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/958" class=".btn">#958</a>
            </td>
            <td>
                <b>
                    fix: add shared-crypto module and apollo wrapper for other key types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">prism-agent</span><span class="chip">build</span><span class="chip">shared</span><span class="chip">castor</span><span class="chip">connect</span>
            </td>
            <td>
                ### Description: 
!!! DO NOT MERGE YET !!! -  need apollo version bump

- Move original `prism-crypto` wrapper from `wallet-api` to `shared-crypto`
- Add wrapper for x25519 and ed25519 key
- Simplify some crypto operation error to align with error handling ADR
- Reorganize `shared-*` into a single directory

### Alternatives Considered (optional): 
Link to existing ADR (Architecture Decision Record), if any. If relevant, describe other approaches explored and the selected approach. Documenting why the methods were not selected will create a knowledge base for future reference, helping prevent others from revisiting less optimal ideas.

### Checklist: 
- [ ] My PR follows the [contribution guidelines](https://github.com/hyperledger-labs/open-enterprise-agent/blob/main/CONTRIBUTING.md) of this project
- [ ] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [ ] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-03 13:33:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/957" class=".btn">#957</a>
            </td>
            <td>
                <b>
                    Update docker-compose.yml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">infra</span>
            </td>
            <td>
                Restricting postgres and pgadmin to local interface by default seems to be a better option since there is no reason to expose these ports to the public internet. Anyone following the local deployment guide on a publicly accesible web server it's a high risk of having the container hijacked by malware bots when the ports are exposed on every interface.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-02 18:21:45 +0000 UTC
    </div>
</div>

