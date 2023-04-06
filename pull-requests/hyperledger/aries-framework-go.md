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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3556" class=".btn">#3556</a>
            </td>
            <td>
                <b>
                    ci: complete release 0.2.0 and prepare 0.3.0
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
        Created At 2023-04-05 16:27:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3555" class=".btn">#3555</a>
            </td>
            <td>
                <b>
                    chore: release 0.2.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Set release flag to true
- Add CHANGELOG for 0.2.0
- Add CHANGELOG for 0.1.9 (missed previously) : point to github release page

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-05 14:33:34 +0000 UTC
    </div>
</div>

