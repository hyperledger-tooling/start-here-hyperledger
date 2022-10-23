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
                
            </td>
            <td>
                - as `build-image` action was trying to pull images from `docker.pkg.github.com`, it never worked because that's not docker registry we are logged into - so we didn't reuse previously built docker layer
- generalized `construct-run-info` to rely on `$MAIN_BRANCH` instead of hardcoding `main`
- added action template for detecting skip PR tags
- fixed information passing into `azure/docker-login@v1`
- fixed publishing jobs - publish built images under both tags `$PUBLISH_VERSION` and also  `$BRANCH_NAME` (to cache layers) 
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

