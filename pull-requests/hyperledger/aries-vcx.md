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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/579" class=".btn">#579</a>
            </td>
            <td>
                <b>
                    Proof presentation/always ack
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">hotfix</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-23 10:44:26 +0000 UTC
    </div>
</div>

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
                <span class="chip">refactoring</span><span class="chip">ci</span>
            </td>
            <td>
                Depends on #575 

Target: run all Rust tests under 30 mins.
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
                <span class="chip">changelog-excluded</span>
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
                <span class="chip">ci</span><span class="chip">dependencies</span>
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
                <span class="chip">refactoring</span>
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
                <span class="chip">refactoring</span>
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
                <span class="chip">hotfix</span><span class="chip">ci</span>
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

