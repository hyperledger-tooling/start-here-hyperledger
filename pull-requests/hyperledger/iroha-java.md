---
layout: default
title: iroha-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-java
---

# iroha-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-java/pull/197" class=".btn">#197</a>
            </td>
            <td>
                <b>
                    Iroha-124 Support other endpoint of the peer (`/configure`, `/health`, `/metrics`) 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The task https://app.zenhub.com/workspaces/iroha-v2-60ddb820813b9100181fc060/issues/hyperledger/iroha-java/124

Change notes:
- added module `admin-client` with additional API for peer's administration and monitoring
- moved `@WithIroha` to separate module `test-tools` to make applicable for both `client` and `admin-client`
- bumped version of Kotlin
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-05 17:42:10 +0000 UTC
    </div>
</div>

