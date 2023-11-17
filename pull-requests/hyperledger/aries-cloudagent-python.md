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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2611" class=".btn">#2611</a>
            </td>
            <td>
                <b>
                    feat: support resolving did:peer:1 received in did exchange
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an experimental implementation of supporting did:peer:1 resolution. This enables ACA-Py to correctly handle DID Exchange requests from AFJ (AFJ now fails to process our responses since we're not passing back a did:peer, still the unqualified values).

Notably, this does not support creating or sending did:peer:1, just storing and resolving.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-17 04:24:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2609" class=".btn">#2609</a>
            </td>
            <td>
                <b>
                    fix: more resilient checks in verify signed attachments
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2608.

This PR makes the signed attachment verification a bit more resilient. According to [RFC 7515](https://datatracker.ietf.org/doc/html/rfc7515), there's no reason for us to strictly expect a `kid` to be present in the `jwk` and we can verify that the jwk corresponds to the kid in the header trivially. In short, the previous rigidity was unnecessary. This corrects that.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-17 02:37:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2607" class=".btn">#2607</a>
            </td>
            <td>
                <b>
                    Anoncreds rs sync updates from Main
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
        Created At 2023-11-15 18:57:47 +0000 UTC
    </div>
</div>

