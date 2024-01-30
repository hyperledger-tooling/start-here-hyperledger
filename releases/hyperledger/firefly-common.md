---
layout: default
title: firefly-common
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/firefly-common
---

# firefly-common <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-common){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v1.4.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.4.5
                </span>
            </td>
            <td>
                ## Migration consideration

Further to the embedding API changes to `eventstreams` in [v1.4.4](https://github.com/hyperledger/firefly-common/releases/tag/v1.4.4), there is an externals change to the JSON configuration of the `webhooks` type of event stream in this release:
- The duplicate top-level `headers` field is removed.

## What's Changed
* fix: delete stream with name by @EnriqueL8 in https://github.com/hyperledger/firefly-common/pull/121
* Remove WebhookConfig.Headers in favour of WebhookConfig.HTTP.HTTPHeaders by @chrisbygrave in https://github.com/hyperledger/firefly-common/pull/122


**Full Changelog**: https://github.com/hyperledger/firefly-common/compare/v1.4.4...v1.4.5
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/firefly-common/releases/tag/v1.4.5" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-01-24 13:14:57 +0000 UTC
    </span>
</div>

