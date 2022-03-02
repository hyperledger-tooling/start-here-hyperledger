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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/454" class=".btn">#454</a>
            </td>
            <td>
                <b>
                    Expose update state with message in node wrapper
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">wrappers</span>
            </td>
            <td>
                Signed-off-by: Miroslav Kovar <miroslav.kovar@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-01 12:08:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/453" class=".btn">#453</a>
            </td>
            <td>
                <b>
                    Expose decline offer in node API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">wrappers</span>
            </td>
            <td>
                Signed-off-by: Miroslav Kovar <miroslav.kovar@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-28 15:44:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/452" class=".btn">#452</a>
            </td>
            <td>
                <b>
                    Change issuer's implementation of is_revokable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">breaking</span>
            </td>
            <td>
                Changes issuer's implementation of `is_revokable` from returning `true` iff the credential was issued under revokable credential definition to returning `true` iff attempt to revoke is expected to succeed, i.e. the credential was issued under revokable credential definition and it was created and saved to the wallet (and potentially sent).

Holder's implementation still returns `true` iff the credential was issued under revokable credential definition.

Signed-off-by: Miroslav Kovar <miroslav.kovar@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-28 11:20:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/448" class=".btn">#448</a>
            </td>
            <td>
                <b>
                    Wait for ack
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                Signed-off-by: Miroslav Kovar <miroslav.kovar@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-24 11:36:33 +0000 UTC
    </div>
</div>

