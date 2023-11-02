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

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    Fix the logging function TimeTrack to take variadic arguments
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.4.16
                </span>
            </td>
            <td>
                Add `otherArgs` argument to `TimeTrack`
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger-labs/yui-relayer/releases/tag/v0.4.16" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-10-26 10:51:35 +0000 UTC
    </span>
</div>

