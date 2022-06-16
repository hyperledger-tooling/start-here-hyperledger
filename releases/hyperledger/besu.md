---
layout: default
title: besu
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    22.4.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    22.4.3
                </span>
            </td>
            <td>
                ### Additions and Improvements
- \[EXPERIMENTAL\] Add checkpoint sync `--sync-mode="X_CHECKPOINT"` [#3849](https://github.com/hyperledger/besu/pull/3849)
- Support `finalized` and `safe` as tags for the block parameter in RPC APIs [#3950](https://github.com/hyperledger/besu/pull/3950)
- Added verification of payload attributes in ForkchoiceUpdated [#3837](https://github.com/hyperledger/besu/pull/3837)
- Add support for Gray Glacier hardfork [#3961](https://github.com/hyperledger/besu/issues/3961)

### Bug Fixes
- alias engine-rpc-port parameter with the former rpc param name [#3958](https://github.com/hyperledger/besu/pull/3958)

As we develop new and required functionality for the Merge, the team has discovered some regressions. For transparency for our production users and testers, we have provided the following known issues below.

### Known Issues:

- Under certain circumstances your node may encounter a state root mismatch, a resync is required to fix this. We are actively looking at fixes. [#3891](https://github.com/hyperledger/besu/issues/3891)
- On certain machines, RocksDB may cause an out of memory error. We are in the process of finalizing configuration changes to address these memory challenges. [#3963](https://github.com/hyperledger/besu/pull/3963)
- Related to the peering issue, sometimes a SnapSync may fail to complete or hang. If your node appears stuck, a restart of the node will fix this issue and should continue the sync. We are looking at both fixes and improvements to the logs to help users understand what is happening during a sync. [#3746](https://github.com/hyperledger/besu/issues/3746)

Most of the above issues can be solved with a restart, and are not specific to 22.4.3. If you are a tester and encounter these bugs and would like to help provide feedback, please reach out on Discord with your configuration and details. This may help us. As always, Hyperledger Besu is an open-source project and we are always looking for direct contributions. Thank you for your patience and support!

https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.4.3/besu-22.4.3.tar.gz
sha256: `f263e82c8dbe9aa23ac2863f82aea62a11b71d3deb9a415432e0fa604ff4a77c`
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.4.3/besu-22.4.3.zip
sha256: `144f4c407193cb66897ac5999b215507333df6b418c84d607bd68e16a179ab64`
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/22.4.3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-06-16 18:04:18 +0000 UTC
    </span>
</div>

