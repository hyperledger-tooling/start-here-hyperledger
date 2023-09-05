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
                PR <a href="https://github.com/hyperledger/iroha-2-docs/pull/390" class=".btn">#390</a>
            </td>
            <td>
                <b>
                    Technical maintenance
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

- Remove Soramitsu UI dependency. The library is undone, and is a heavy dependency without a good reason. I used lighter alternatives (hand-written components, Headless UI).
- Update dependencies (including VitePress to `1.0.0-rc.10`)
- Fix ESLint warning
- Removed PWA plugin; using a simple WebManifest instead
- VitePress has an updated color scheme. It is more accessible than before. I find our current bright-red color is not a good choice for text, and think that we should change it.

### Checklist

- [ ] Return brand colors?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-01 07:20:29 +0000 UTC
    </div>
</div>

