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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/566" class=".btn">#566</a>
            </td>
            <td>
                <b>
                    Docs/update
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
        Created At 2022-09-15 00:24:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/565" class=".btn">#565</a>
            </td>
            <td>
                <b>
                    Remove function to revoke+publish individual credential
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                After changes done on https://github.com/hyperledger/aries-vcx/pull/558 it became clear that `vcx_revoke_credential` is problematic function as:
- before #558 it could cause entering problematic state after losing revocation delta
- changes in #558 prevent problematic behaviour, but causes `vcx_revoke_credential` to have side effects - if other credentials in same revocation registry has been revoked locally before and their deltas are accumulated, it would publish revocation for those credential as well. 
The pre #558 approach in unacceptable, the post #558 approach is not transparent. The right way is to revoke credential locally, then published the delta, accounting for the fact that can lead to actually publishing merged revocation delta of multiple local revocations.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-14 21:39:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/564" class=".btn">#564</a>
            </td>
            <td>
                <b>
                    Cleanup nodejs test function naming, remove duplicated test
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
        Created At 2022-09-14 21:38:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/563" class=".btn">#563</a>
            </td>
            <td>
                <b>
                    Reformat, use secrets.GITHUB_TOKEN everywhere in CI
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
        Created At 2022-09-14 17:35:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/562" class=".btn">#562</a>
            </td>
            <td>
                <b>
                    Enhance node agent CLI to support url formatted invitations
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
        Created At 2022-09-14 17:31:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/561" class=".btn">#561</a>
            </td>
            <td>
                <b>
                    Refactor building problem reports, add logging
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
        Created At 2022-09-14 13:23:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/560" class=".btn">#560</a>
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
                iOS Wrapper abstraction: Some information, such as handler types (u32, i32) or callback definitions, is only useful within vcx and the client code that uses them doesn't need to know the details. Hiding them from the client code will improve maintainability.

Signed-off-by: kukgini <kukgini@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-14 09:17:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/559" class=".btn">#559</a>
            </td>
            <td>
                <b>
                    Statically link libindy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - use left-arm form of vdr-tools

- simplify some code and remove unused dependencies
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-13 12:30:00 +0000 UTC
    </div>
</div>

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
- Update `publish_local_revocations` implementation to assure that accumulated deltas are deleted only if publishing to ledger has been successful. 
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

