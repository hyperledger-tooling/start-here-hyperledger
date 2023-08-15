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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3618" class=".btn">#3618</a>
            </td>
            <td>
                <b>
                    feat: Improvements to ECDSA2019 DI API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The existing API required an interface that defines many more methods than what are actually required, which forces consumers of the API to implement many methods that won't ever be called. The API has now been changed to make use of two minimal interfaces instead, making it easier to use and understand. Note that implementations of the larger crypto interface can still be used since the minimal interface method signatures match.

To avoid potential confusion with the new interface names, two existing constructors were renamed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-14 21:29:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3617" class=".btn">#3617</a>
            </td>
            <td>
                <b>
                    feat: SDJWT V5 (#33)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
SD JWT V5 Support

**Description:**
https://www.ietf.org/archive/id/draft-ietf-oauth-selective-disclosure-jwt-02.html
https://www.ietf.org/archive/id/draft-ietf-oauth-selective-disclosure-jwt-05.html

**Summary:**
1. Changes in issuance, holder and verifier logic.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-09 12:23:41 +0000 UTC
    </div>
</div>

