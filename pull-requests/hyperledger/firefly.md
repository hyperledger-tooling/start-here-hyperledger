---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1176" class=".btn">#1176</a>
            </td>
            <td>
                <b>
                    Update to docker/build-push-action@v4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of #1174
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-02 20:20:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1175" class=".btn">#1175</a>
            </td>
            <td>
                <b>
                    Include signing key in batch processor identifier
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Messages from the same identity but different signing keys must be processed into different batches. If the signing key of the message does not match the signing key of the batch, the message will be rejected.

Fixes #1173
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-01 22:58:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1174" class=".btn">#1174</a>
            </td>
            <td>
                <b>
                    Update to docker/build-push-action@v4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Due to a recent change in the docker/build-push-action GitHub Action https://github.com/docker/build-push-action/issues/778 our images stopped having their manifests published properly. This PR updates our GitHub Actions to use a newer version of the Action, and restores the previously working behavior. I was able to test this on my own fork and created https://github.com/nguyer/firefly/pkgs/container/firefly/67526987 which has a good manifest in it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-01 21:40:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1172" class=".btn">#1172</a>
            </td>
            <td>
                <b>
                    Add stack type to nightly integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-01 01:35:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1171" class=".btn">#1171</a>
            </td>
            <td>
                <b>
                    Update dependencies for v1.2.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-31 21:16:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1169" class=".btn">#1169</a>
            </td>
            <td>
                <b>
                    Fix coverage gap in webhooks test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-30 21:40:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1168" class=".btn">#1168</a>
            </td>
            <td>
                <b>
                    Update dependencies for v1.2.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-30 20:20:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1164" class=".btn">#1164</a>
            </td>
            <td>
                <b>
                    Keep Docker state between builds
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Greatly reduces incremental build time for "make docker".
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-27 15:42:16 +0000 UTC
    </div>
</div>

