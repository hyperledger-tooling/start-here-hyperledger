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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/611" class=".btn">#611</a>
            </td>
            <td>
                <b>
                    Refactor verifier / prover SMs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">refactoring</span>
            </td>
            <td>
                Addressing #583, based on #610.

Signed-off-by: Miroslav Kovar <miroslav.kovar@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-21 13:49:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/610" class=".btn">#610</a>
            </td>
            <td>
                <b>
                    Refactor issuer / holder SMs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">refactoring</span>
            </td>
            <td>
                Holder handler calls specific SM methods instead of relying on a step function. This way, if an explicit "action" is performed in an invalid state, an error is returned, instead of a noop.

Addresses #583 .

Signed-off-by: Miroslav Kovar <miroslav.kovar@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-21 07:31:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/608" class=".btn">#608</a>
            </td>
            <td>
                <b>
                    Revocation notification
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">feature</span>
            </td>
            <td>
                https://github.com/hyperledger/aries-rfcs/tree/main/features/0721-revocation-notification-v2

Signed-off-by: Miroslav Kovar <miroslav.kovar@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-20 07:56:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/607" class=".btn">#607</a>
            </td>
            <td>
                <b>
                    Fix agent build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">hotfix</span>
            </td>
            <td>
                Signed-off-by: Miroslav Kovar <miroslav.kovar@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-19 19:47:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/605" class=".btn">#605</a>
            </td>
            <td>
                <b>
                    Backchannel-related refactoring
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">refactoring</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-16 16:58:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/604" class=".btn">#604</a>
            </td>
            <td>
                <b>
                    Rust aries agent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">feature</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-16 16:57:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/603" class=".btn">#603</a>
            </td>
            <td>
                <b>
                    Refactor CI using composite actions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ci</span>
            </td>
            <td>
                - Extract number of composite actions
- Technical details such us caching directory / file location, concept of cache-key hidden behind simpler composite-action interface
- In case of cache miss, significantly improved build times by reusing docker layers from previous branch build / master branch build 
- CI workflow file shorter by ~500 lines :-) 

Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-16 10:46:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/602" class=".btn">#602</a>
            </td>
            <td>
                <b>
                    Update Rust toolchain to 1.64.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">update</span>
            </td>
            <td>
                Signed-off-by: Miroslav Kovar <miroslav.kovar@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-15 19:12:39 +0000 UTC
    </div>
</div>

