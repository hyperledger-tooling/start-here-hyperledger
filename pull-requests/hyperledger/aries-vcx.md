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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/614" class=".btn">#614</a>
            </td>
            <td>
                <b>
                    Allow obtaining cred rev id from the wallet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">feature</span>
            </td>
            <td>
                This will eventually allow checking revocation status against ledger and finding the corresponding `Holder` based on received revocation notification.

Signed-off-by: Miroslav Kovar <miroslav.kovar@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-24 12:00:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/613" class=".btn">#613</a>
            </td>
            <td>
                <b>
                    Ci/improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">skip-ios</span><span class="chip">skip-android</span>
            </td>
            <td>
                - Fix CI warnings (usage of set-output)
- As `build-image` action was trying to pull images from `docker.pkg.github.com`, it never worked because that's not docker registry we are logged into - so we didn't reuse previously built docker layer
- Generalized `construct-run-info` to refer to on `$MAIN_BRANCH` instead of hardcoding `main`
- Added action template for detecting skip PR tags (currently supports opt-in PR tags `skip-android` and `skip-ios`)
- Fixed information passing into `azure/docker-login@v1`
- Fixed publishing jobs - images are published under tag`$PUBLISH_VERSION` 
- Modified `build-image` such that it publishes image `<docker-img>:<branch>` to docker registry for caching purposes
- Adjusted publish-image more robust so it doesn't try to load image from cache if it already exist in local docker repo

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-22 22:04:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/612" class=".btn">#612</a>
            </td>
            <td>
                <b>
                    Use a macro for message fetching functions in agent
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
        Created At 2022-10-22 18:24:45 +0000 UTC
    </div>
</div>

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

