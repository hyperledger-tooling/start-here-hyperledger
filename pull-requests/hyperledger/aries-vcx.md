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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/570" class=".btn">#570</a>
            </td>
            <td>
                <b>
                    Reduce size of the release build.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Disable debug in the release profile.
The build on macOS M1, libvcx.a is about 100 Mb, libvcx.dylib is about 20 Mb.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-19 06:32:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/569" class=".btn">#569</a>
            </td>
            <td>
                <b>
                    Make into_did_doc async
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
        Created At 2022-09-16 19:11:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/568" class=".btn">#568</a>
            </td>
            <td>
                <b>
                    Rename SetupLibraryAgencyV2 to SetupPool
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
        Created At 2022-09-16 16:21:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/567" class=".btn">#567</a>
            </td>
            <td>
                <b>
                    Update vdr-tools dependency
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
        Created At 2022-09-16 15:23:39 +0000 UTC
    </div>
</div>

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

