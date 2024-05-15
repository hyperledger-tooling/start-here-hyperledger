---
layout: default
title: iroha-2-docs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-2-docs
---

# iroha-2-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-2-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-2-docs/pull/485" class=".btn">#485</a>
            </td>
            <td>
                <b>
                    Update the data model reference to the latest iroha dev revision
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR does three things:
- support for bitmaps in schema (introduced in https://github.com/hyperledger/iroha/pull/4381)
- "fixes" paths to referenced config files
- updates torii reference to be in line with https://github.com/hyperledger/iroha/pull/4544

While the inclusion of toml templates in place of old json files makes the config documentation "wrong", this allows writing new documentation with references to a more up-to-date `schema.json`.

In the end I think the #397 will in the end remove the toml templates altogether, I consider this just a way to unblock my updates to the torii reference for https://github.com/hyperledger/iroha/pull/4544

@0x009922 Do you think it's a good approach? Or should we try somehow to keep the old `json`'s in place while the new config reference is not yet complete?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-14 14:01:33 +0000 UTC
    </div>
</div>

