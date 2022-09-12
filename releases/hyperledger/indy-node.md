---
layout: default
title: indy-node
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/indy-node
---

# indy-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v1.13.2-rc2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.13.2-rc2
                </span>
            </td>
            <td>
                [v1.13.2-rc2] 

## What's Changed
* Add flag for sorting algorithm switching by @c2bo in https://github.com/hyperledger/indy-node/pull/1775
  * The default value ensures net new Ubuntu 20.04 based networks use sorted ordering for revocation transactions.  The `REV_STRATEGY_USE_COMPAT_ORDERING` flag should be set to `True` when adding a Ubuntu 20.04 based node to an existing network so it uses compatibility ordering.
* [v1.13.2-rc2] - Update Version Number for Release by @sovbot in https://github.com/hyperledger/indy-node/pull/1776

## New Contributors
* @c2bo made their first contribution in https://github.com/hyperledger/indy-node/pull/1775

**Full Changelog**: https://github.com/hyperledger/indy-node/compare/v1.13.2-rc1...v1.13.2-rc2
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/indy-node/releases/tag/v1.13.2-rc2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-09-12 19:31:22 +0000 UTC
    </span>
</div>

