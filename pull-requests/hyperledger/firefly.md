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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1088" class=".btn">#1088</a>
            </td>
            <td>
                <b>
                    Allow listening for go debug on all interfaces, not just localhost
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It's difficult using the go pprof debug utility when running in a container since the network interface it binds to defaults to localhost. This PR makes 2 changes:

1. Make the interface address configurable
2. Change the default interface to "*"

It still requires changes to the docker run command or docker compose overrides file to get a route through to the debug listener, but doesn't require you to rebuild firefly. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-11 12:31:37 +0000 UTC
    </div>
</div>

