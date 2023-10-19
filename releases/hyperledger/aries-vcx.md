---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    Release 0.60.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.60.0
                </span>
            </td>
            <td>
                # Headlines
- This release marks a milestone where we dropped vdrtools(indysdk fork) based anoncreds implementation in favor of credx library. 
Migration of wallet from `vdrtools -> credx` has been stabilized and provided in release `0.59.1`.

# What's changed
### Refactoring
* Refactor/test by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/995
* Refactor/remove mocks by @bobozaur in https://github.com/hyperledger/aries-vcx/pull/1005
* Replace trait objects in libvcx_core with generics/concrete types by @bobozaur in https://github.com/hyperledger/aries-vcx/pull/1011

### Changes
* Use credx anoncreds in napi wrapper by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/927
* Purge vdrtools by @bobozaur in https://github.com/hyperledger/aries-vcx/pull/1013

### CI
* Release 0.60.0 by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/1015


**Full Changelog**: https://github.com/hyperledger/aries-vcx/compare/0.59.1...0.60.0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-vcx/releases/tag/0.60.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-10-12 15:04:12 +0000 UTC
    </span>
</div>

