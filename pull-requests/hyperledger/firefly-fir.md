---
layout: default
title: firefly-fir
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-fir
---

# firefly-fir <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-fir){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-fir/pull/9" class=".btn">#9</a>
            </td>
            <td>
                <b>
                    Enhanced Identity API - custom identities and DID support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR from @jimthematrix and @peterbroadhurst proposes the next step that was discussed in https://github.com/hyperledger/firefly/issues/187

Summary of value (more detail in FIR itself):

1. Make identity extensible by applications, allowing broadcast of granular application-specific identities in a tree under an organization
2. Allow multiple signing keys to be registered by a single identity, for key rotation scenarios, and multiple key types/uses
3. Allow minimum viable DID documents to be obtained for FireFly backed identities
4. Provide a model that is designed for future extensibility to externally verifiable DID backed identities (implementation out of scope for this FIR)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-03 00:37:28 +0000 UTC
    </div>
</div>

