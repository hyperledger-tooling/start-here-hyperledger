---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3557" class=".btn">#3557</a>
            </td>
            <td>
                <b>
                    feat: refactor logs and kms+crypto into separate components
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - component/log: Logging API implementation.
- component/kmscrypto: KMS, Crypto, and some JWK APIs, and their
  implementations.

For refactored APIs, the original APIs have been left in their
original locations, transparently referencing/wrapping
the new APIs, to minimize breaking changes for consumers of
these APIs. Exceptions are:
- KMS protobufs for key data don't have wrappers in their original
  locations. Imports need to be amended to component/kmscrypto.

Once further refactoring is complete, these original APIs will be
deprecated and callers advised to use the refactored APIs instead.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-06 16:43:16 +0000 UTC
    </div>
</div>

