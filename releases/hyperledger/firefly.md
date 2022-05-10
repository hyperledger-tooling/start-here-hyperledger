---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v1.0.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.0.1
                </span>
            </td>
            <td>
                ## Summary

Fixes for token approvals - previously approvals would intermittently be missed by FireFly or recorded with incorrect details.

## Breaking Changes and Migrations

New versions of the ERC20/ERC721 connector will assume "no data" support if you create a token pool against an older version of the sample smart contracts - see https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/57

## Updated Dependencies

* firefly-tokens-erc1155 [v1.0.2](https://github.com/hyperledger/firefly-tokens-erc1155/releases/tag/v1.0.2)
* firefly-tokens-erc20-erc721 [v1.0.1](https://github.com/hyperledger/firefly-tokens-erc20-erc721/releases/tag/v1.0.1)
* firefly-ui [v1.0.1](https://github.com/hyperledger/firefly-ui/releases/tag/v1.0.1)
* firefly-cli [v1.0.1](https://github.com/hyperledger/firefly-cli/releases/tag/v1.0.1)

## What's Changed
* Backport fixes for 1.0.1 by @awrichar in https://github.com/hyperledger/firefly/pull/803

**Full Changelog**: https://github.com/hyperledger/firefly/compare/v1.0.0...v1.0.1
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/firefly/releases/tag/v1.0.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-05-09 20:45:05 +0000 UTC
    </span>
</div>

