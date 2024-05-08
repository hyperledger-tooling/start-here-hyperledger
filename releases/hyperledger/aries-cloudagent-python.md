---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    0.11.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.11.1
                </span>
            </td>
            <td>
                A patch release to update the `aiohttp` library such that a reported serious vulnerability is addressed such that a crafted payload delivered to `aiohttp` can put it in an infinite loop, which can be used for a low cost denial of service attack. [CVE-2024-30251] describes the issue.

[CVE-2024-30251]: https://github.com/advisories/GHSA-5m98-qgg9-wh84

### 0.11.1 Breaking Changes

There are no breaking changes in this release. The only changed is the updated `aiohttp` dependency.

## What's Changed
* 0.11.1 and aiohttp dependency update by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2936
* 0.11.1 ChangeLog fixes by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2937


**Full Changelog**: https://github.com/hyperledger/aries-cloudagent-python/compare/0.11.0...0.11.1
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/0.11.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-05-07 19:35:18 +0000 UTC
    </span>
</div>

