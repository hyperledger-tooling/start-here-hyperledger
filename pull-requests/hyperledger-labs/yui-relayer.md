---
layout: default
title: yui-relayer
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/yui-relayer
---

# yui-relayer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/yui-relayer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-relayer/pull/120" class=".btn">#120</a>
            </td>
            <td>
                <b>
                    fix height flag type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                height flag should be specified as uint64, but int64 is used
- https://github.com/hyperledger-labs/yui-relayer/blob/main/cmd/query.go#L52
- https://github.com/hyperledger-labs/yui-relayer/blob/main/cmd/query.go#L89
- https://github.com/hyperledger-labs/yui-relayer/blob/main/cmd/query.go#L122
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-31 14:23:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-relayer/pull/119" class=".btn">#119</a>
            </td>
            <td>
                <b>
                    reorganize interfaces that makes up the Prover interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                introduce the following interfaces
- `FinalityAware`
- `FinalityAwareChain`
- `ChainLightClient`

delete the following interface
- `ChainICS02QuerierLightClient`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-30 08:43:59 +0000 UTC
    </div>
</div>

