---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1090" class=".btn">#1090</a>
            </td>
            <td>
                <b>
                    Fix typo in multiparty_features.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Chengxuan Xing <chengxuan.xing@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-17 22:31:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1089" class=".btn">#1089</a>
            </td>
            <td>
                <b>
                    Set firstEvent default using string
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `viper.GetString` does not return a value, if the default was set to a type that wraps string.

So the fact we were setting the default for `firstEvent` as `core.SubOptsFirstEventOldest`, meant the default did not work.

This is a significant bug, as it changes the default in v1.1 to listen from the current block (the EthConnect/FabConnect/EVMConnect default for an unset value), rather than the beginning of the blockchain (as we did in v1.0).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-14 19:28:53 +0000 UTC
    </div>
</div>

