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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/558" class=".btn">#558</a>
            </td>
            <td>
                <b>
                    Ledger comm/validate response
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add validations to ledger responses. Return error if transaction was rejected
- Changed implementation of `revoke_credential` - if local revocations has been performed (eg `get_rev_reg_delta` resolved some unpublished accumulated delta), calling this function will fail, as `prevAccum` in delta returned by `libindy_issuer_revoke_credential` actually refers to state of accumulator AFTER the local revocations, not the state of accumulator on the ledger. Attempt to publish this revocation delta will fail due to mismatch of ledger state of `accum` and value of `prevAccum` in delta returned by `libindy_issuer_revoke_credential`. With old implementation of `revoke_credential`, the delta is lost. That's a problem because, the revocation has changes state of internal accumulator, however the delta was not merged into other accumulated delta. This makes further revocation in this revocation registry, least to say difficult - with current implementation, any attempt to perform further revocations would fail. 
This can be prevented if we always accumulate deltas returned by `libindy_issuer_revoke_credential`, which is what this PR does. Consequently, `revoke_credential` now basically
   - revokes new credential and updates accumulated delta
   - publishes accumualted delta, eg. publishes all accumulated reovcations
which is unexpected behaviour from API standpoint, hence until smarter implementation is created, `revoke_credential` is now deprecated and callers should simply use combination of `revoke_credential_local` and `publish_local_revocations` instead. That way the calling code is more transparent about the fact that ALL local revocations will be published.


- Minor variables/function renames, but particularly removal of "cache" vocabulary for storing revocation deltas. Rev delta storage is not cache, as it does not serve for optimization, but rather storing quite quite important data.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-09 22:04:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/557" class=".btn">#557</a>
            </td>
            <td>
                <b>
                    Fix order of args passed to function publish_local_revocations
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
        Created At 2022-09-09 22:03:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/556" class=".btn">#556</a>
            </td>
            <td>
                <b>
                    Eliminate global state: pool handle
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
        Created At 2022-09-07 13:54:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/555" class=".btn">#555</a>
            </td>
            <td>
                <b>
                    Remove TestAgent trait
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">refactoring</span>
            </td>
            <td>
                Signed-off-by: Miroslav Kovar <miroslav.kovar@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-06 15:02:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/554" class=".btn">#554</a>
            </td>
            <td>
                <b>
                    Eliminate global state: issuer did
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
        Created At 2022-09-06 08:35:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/553" class=".btn">#553</a>
            </td>
            <td>
                <b>
                    Release 0.41.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Miroslav Kovar <miroslav.kovar@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-05 11:42:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/552" class=".btn">#552</a>
            </td>
            <td>
                <b>
                    Add MAINTAINERS.md file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span>
            </td>
            <td>
                Signed-off-by: Miroslav Kovar <miroslav.kovar@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-05 11:06:06 +0000 UTC
    </div>
</div>

