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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/578" class=".btn">#578</a>
            </td>
            <td>
                <b>
                    Refactor/ci workflow
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
        Created At 2022-09-21 16:51:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/577" class=".btn">#577</a>
            </td>
            <td>
                <b>
                    Separate messages module into a crate
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
        Created At 2022-09-21 07:56:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/576" class=".btn">#576</a>
            </td>
            <td>
                <b>
                    Release 0.42.0
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
        Created At 2022-09-19 22:41:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/575" class=".btn">#575</a>
            </td>
            <td>
                <b>
                    Statically link libvcx.so
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Vdr-tools linked as an ordinary Rust crate and does not require any additional installation steps.

Signed-off-by: Artem Mironov <artem.mironov@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-19 15:33:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/574" class=".btn">#574</a>
            </td>
            <td>
                <b>
                    Avoid HTTP request body cloning.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Consume body passed to post_message(body, url) and update callers.

Fold some long lines while I'm here to improve code readability.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-19 09:58:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/573" class=".btn">#573</a>
            </td>
            <td>
                <b>
                    Reuse reqwest::Client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                According to reqwest documentation, is perfectly OK to reuse instance of reqwest::Client. We don't need to wrap it into RwLock because it is already thread and async safe.

Signed-off-by: Artem Mironov <artem.mironov@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-19 07:33:27 +0000 UTC
    </div>
</div>

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

