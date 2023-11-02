---
layout: default
title: yui-relayer
parent: Hyperledger Labs
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger-labs/yui-relayer
---

# yui-relayer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/yui-relayer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    reorganize interfaces that comprise the Prover interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.4.17
                </span>
            </td>
            <td>
                introduce the following interfaces

- `FinalityAware`, which provides `GetLatestFinalizedHeader()`
- `FinalityAwareChain`, which is `FinalityAware` + `Chain`
- `ChainLightClient`, which is `Chain` + `LightClient`

delete the following interface

- `ChainICS02QuerierLightClient`

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger-labs/yui-relayer/releases/tag/v0.4.17" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-10-31 01:16:34 +0000 UTC
    </span>
</div>

