---
layout: default
title: indy-node-monitor
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/indy-node-monitor
---

# indy-node-monitor <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-node-monitor){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v0.4.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.4.0
                </span>
            </td>
            <td>
                ## What's Changed
* Added a way to not use the -it mode for docker easily by setting the CM env variable on run #13 by @swcurran in https://github.com/hyperledger/indy-node-monitor/pull/15
* Detect connection issues between nodes by @WadeBarnes in https://github.com/hyperledger/indy-node-monitor/pull/16
* Detect pending upgrade and display in `--status` summary by @WadeBarnes in https://github.com/hyperledger/indy-node-monitor/pull/17
* Add `--alerts` filter by @WadeBarnes in https://github.com/hyperledger/indy-node-monitor/pull/19
* Add validator client and node public addresses by @WadeBarnes in https://github.com/hyperledger/indy-node-monitor/pull/22
* Added URL work around for linux. by @mrkaurelius in https://github.com/hyperledger/indy-node-monitor/pull/23
* Initial implementation of plugin architecture. by @KoleBarnes in https://github.com/hyperledger/indy-node-monitor/pull/26
* Fixed Bug where network_name was not set when using genesis_url. by @KoleBarnes in https://github.com/hyperledger/indy-node-monitor/pull/30
* Added Indicio networks to networks.json by @GavinBendixsen in https://github.com/hyperledger/indy-node-monitor/pull/32
* Fix pipe to file issue on Windows by @WadeBarnes in https://github.com/hyperledger/indy-node-monitor/pull/33
* Fix for fetch_status container build issues. by @WadeBarnes in https://github.com/hyperledger/indy-node-monitor/pull/34
* Add support for running as an API server. by @KoleBarnes in https://github.com/hyperledger/indy-node-monitor/pull/35

## New Contributors
* @mrkaurelius made their first contribution in https://github.com/hyperledger/indy-node-monitor/pull/23
* @KoleBarnes made their first contribution in https://github.com/hyperledger/indy-node-monitor/pull/26
* @GavinBendixsen made their first contribution in https://github.com/hyperledger/indy-node-monitor/pull/32

**Full Changelog**: https://github.com/hyperledger/indy-node-monitor/commits/v0.6.0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/indy-node-monitor/releases/tag/v0.4.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-12-24 19:04:46 +0000 UTC
    </span>
</div>

