---
layout: default
title: aries-framework-dotnet
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-dotnet
---

# aries-framework-dotnet <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-dotnet){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-dotnet/pull/210" class=".btn">#210</a>
            </td>
            <td>
                <b>
                    did:key Transformation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Short description of what this resolves:
This PR adds the ability to transform did:key into verkeys and verkeys into their did:key representation as described in [RFC-0360](https://github.com/hyperledger/aries-rfcs/tree/b3a3942ef052039e73cd23d847f42947f8287da2/features/0360-use-did-key).

#### Changes proposed in this pull request:

- Added method in DidUtils to transform verkey into did:key
- Enable did:key usage in connection invitation and service decorators
- Added integration tests for connectionless presentation and issuance

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-10 12:51:27 +0000 UTC
    </div>
</div>

