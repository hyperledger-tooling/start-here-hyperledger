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
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/324" class=".btn">#324</a>
            </td>
            <td>
                <b>
                    IIN Agent Auto Sync Bug and Deploy Workflow improvement
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * IIN Agent auto sync bug fixed. Now works as expected.
* Added more config instructions in README of IIN Agent
* Deploy workflows now will pass if package to be published already exists.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-13 09:31:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/322" class=".btn">#322</a>
            </td>
            <td>
                <b>
                    IIN Agent Implementation of endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                IIN Agent:
1. Added implementation for endpoints `syncExternalState`, `requestIdentityConfiguration`, `sendIdentityConfiguration`, and `sendAttestation`.
2. Added utility functions in common/utils.
3. Added Config files (along with templates): dnsconfig, and security-domain-config.
4. Added env variables as required.
5. Added dockerfile and docker-compose for iin agent.
6. Added sample testnet envs for  iin agent.

SDK:
1. Added MembershipManager, to record local memberships and also perform manual sync of membership through iin-agent.

Fabric-CLI:
1. Removed generation of membership from all places.
2. Removed IINAgent user registration from cli.
3. Using SDK to record local membership.
4. Added function to sync membership manually via iin-agent (using SDK).

Driver:
1. Error Log fixes
2. Implemented function to restart event listeners from database when driver is restarted.
3. Allow TLSCACert for client to be empty.
4. Improved and slimmed docker image for fabric driver.

Workflows:
1. Updated workflows to use iin-agent for fabric membership sync.
2. Modified existing (different) workflow(s) to build, test and publish iin-agent docker image.
3. (EDIT) Added testcase for locally built docker based test net setup in data sharing workflow.

Update:
Updated all node applications to node version 16.17.1.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-07 21:09:58 +0000 UTC
    </div>
</div>

