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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/405" class=".btn">#405</a>
            </td>
            <td>
                <b>
                    fix libzmq build error with disable some features
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix libzmq build error with disable some features (perf and curve-keygen)

Signed-off-by: kukgini <kukgini@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-01 15:10:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/404" class=".btn">#404</a>
            </td>
            <td>
                <b>
                    Release 0.24.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">changelog-excluded</span>
            </td>
            <td>
                Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-30 10:15:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/403" class=".btn">#403</a>
            </td>
            <td>
                <b>
                    Revert reqwest, futures, tokio upgrade (revision 5502176e6)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pre-release</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-29 16:09:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/402" class=".btn">#402</a>
            </td>
            <td>
                <b>
                    Pass request data to Verifier::create_from_request via struct
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">refactoring</span>
            </td>
            <td>
                Signed-off-by: Miroslav Kovar <miroslavkovar@protonmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-29 14:38:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/400" class=".btn">#400</a>
            </td>
            <td>
                <b>
                    Send presentation ack
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                Signed-off-by: Miroslav Kovar <miroslavkovar@protonmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-29 11:52:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/398" class=".btn">#398</a>
            </td>
            <td>
                <b>
                    iOS Wrapper abstraction
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Some information, such as handler types (u32, i32) or callback definitions, is only useful within vcx and the client code that uses them doesn't need to know the specifics. So I think hiding it from the client code will improve maintainability.

Signed-off-by: kukgini <kukgini@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-27 02:00:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/397" class=".btn">#397</a>
            </td>
            <td>
                <b>
                    Do not serialize None Filter fields
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">hotfix</span>
            </td>
            <td>
                Serialized `null` values in the `Filter` were throwing acapy off.

Signed-off-by: Miroslav Kovar <miroslavkovar@protonmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-26 20:51:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/396" class=".btn">#396</a>
            </td>
            <td>
                <b>
                    Upgrade reqwest to 0.9.19
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-26 15:36:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/393" class=".btn">#393</a>
            </td>
            <td>
                <b>
                    Update readme, delete unmaintained changelog.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-25 14:48:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/392" class=".btn">#392</a>
            </td>
            <td>
                <b>
                    Release retry/0.24.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pre-release</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-25 13:39:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/391" class=".btn">#391</a>
            </td>
            <td>
                <b>
                    Release 0.24.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pre-release</span>
            </td>
            <td>
                Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-25 11:49:21 +0000 UTC
    </div>
</div>

