---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2406" class=".btn">#2406</a>
            </td>
            <td>
                <b>
                    refactor(weaver): prefix cacti to all weaver packages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Set publish target to cacti

- Update relay, drivers, iin-agent image registry to hyperledger/cacti
- Update npm packages (protos-js and sdks) registry to cacti
- Update maven packages registry to cacti
- Rename sdks/besu/interoperation-node-sdk to sdks/besu/node
- Rename modules with following convention `<module-type>-<dlt-platform>`:
    - For SDKs: `sdk.corda`, `sdk-fabric`, `sdk-besu`
    - For drivers: `driver-corda`, `driver-fabric`
    - For interoperation modules: `imodule.corda`
- Change all packages version to v2.0.0-alpha-prerelease
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-26 06:30:55 +0000 UTC
    </div>
</div>

