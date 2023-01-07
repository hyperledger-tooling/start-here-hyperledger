---
layout: default
title: iroha
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha
---

# iroha <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3049" class=".btn">#3049</a>
            </td>
            <td>
                <b>
                    [ci]: Add regular image tag for Soramitsu registry
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                Signed-off-by: BAStos525 <jungle.vas@yandex.ru>

### Description of the Change
Add one more iroha2 ordinary image tag to be uploaded to Soramitsu images registry.

### Issue
We redeploy some of k8s deployments based on iroha quite often. Free DockerHub account has images pull limit.

### Benefits

By uploading iroha2 stable & lts images with the same tags as iroha2 has on DockerHub, we will get rid of images pull limit and avoid delays with iroha2 deployments (not only Orillion projects).

### Possible Drawbacks

None.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-06 11:13:33 +0000 UTC
    </div>
</div>

