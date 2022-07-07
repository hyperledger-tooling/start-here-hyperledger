---
layout: default
title: weaver-dlt-interoperability
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/weaver-dlt-interoperability
---

# weaver-dlt-interoperability <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/weaver-dlt-interoperability){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/291" class=".btn">#291</a>
            </td>
            <td>
                <b>
                    Relay: Event Subscription Endpoints implemented
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Feature:
1. Event subscription endpoints added in relay.
2. Added new service in protos `relay/events` to make event subscription completely async in relay.
3. Added new field in `EventMatcher`: `event_class_id`.
5. Bump Relay version and Protos version to 1.4.0.

Improvements:
1. Moved all committed fabric-network artifacts to separate folder, which will be copied to `shared` folder during network start, and deleted when run `make clean`.
2. Added workflow to test relay using dummy driver and dummy client.

Close #267 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 17:36:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/290" class=".btn">#290</a>
            </td>
            <td>
                <b>
                    Minor Package Upgrades, Code Refactoring, and Bug Fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Upgraded Weaver protos to version `1.3.2`.
Removed `.npmrc` files containing private credentials from Docker container images.
Updated Corda testnet compose files to work with the latest version of docker-compose.
Updated Fabric testnet chaincode deployments to depend on latest and recent versions of Golang.
Bug fixes and output formatting changes in Fabric chaincodes and CLI.
Added more assets in Fabric CLI configuration files to enable more asset exchange test scenarios.
Unlinked publishing of module packages from protos package in github workflows to avoid occasional test failures.
Update instructions in tutorial docs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-05 18:13:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/289" class=".btn">#289</a>
            </td>
            <td>
                <b>
                    Protos for events subscription added
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: sandeep.nishad1 <sandeep.nishad1@ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-04 07:52:15 +0000 UTC
    </div>
</div>

