---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/432" class=".btn">#432</a>
            </td>
            <td>
                <b>
                    Update tokio and libc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">update</span>
            </td>
            <td>
                Signed-off-by: Miroslav Kovar <miroslavkovar@protonmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-25 21:52:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/431" class=".btn">#431</a>
            </td>
            <td>
                <b>
                    Release 0.29.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">changelog-excluded</span>
            </td>
            <td>
                Signed-off-by: Miroslav Kovar <miroslavkovar@protonmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-25 16:14:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/429" class=".btn">#429</a>
            </td>
            <td>
                <b>
                    Refactor credential definition code, separate rotation and publishing…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">refactoring</span><span class="chip">breaking</span>
            </td>
            <td>
                - Separates credential registry rotation from its publishing. If you call `credential_def::rotate_rev_reg`, you need to additionally call `credential_def::publish_revocation_primitives`. Previously these both stages were happening as part of `credential_def::rotate_rev_reg`
- Adds tracking whether and which revocation primitives (revocation registry definition, initial revocation registry delta) were published on ledger so we prevent attempts to publish already published data on ledger.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 12:01:11 +0000 UTC
    </div>
</div>

