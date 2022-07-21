---
layout: default
title: caliper
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/caliper
---

# caliper <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/caliper){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1412" class=".btn">#1412</a>
            </td>
            <td>
                <b>
                    update fabric bindings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - remove fabric-protos as not needed due to removal of fabric operations code
- update to latest 2.2 sdk which addresses discovery bug under load

Signed-off-by: D <d_kelsey@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-21 08:56:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1411" class=".btn">#1411</a>
            </td>
            <td>
                <b>
                    Remove channel and chaincode operations from Fabric v1 connector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In this PR:
* The ability for caliper to be able to create channels, install and instantiate chaincode for fabric is removed.

Closes #1204
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-20 17:16:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1410" class=".btn">#1410</a>
            </td>
            <td>
                <b>
                    Migrate Fabric integration tests to test network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In this PR:
* Fabric integration tests (fabric_tests, fabric_docker_local_tests and fabric_docker_distributed_tests) are migrated to use test network for standing up a Fabric network instead of a custom setup

Closes #1408 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-19 20:57:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1407" class=".btn">#1407</a>
            </td>
            <td>
                <b>
                    Add workflow to test npm packages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In this PR
* A new GitHub Actions workflow is added to test publishing of a package and the functioning of the published package using Verdaccio, with the help of scripts written previously

Closes #1403

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-17 17:51:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1406" class=".btn">#1406</a>
            </td>
            <td>
                <b>
                    Cache node modules across CI workflows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In this PR:
* The integration tests workflow is refactored to be DRY
* The `node_modules` folder is cached across workflows
* The SUT is cached across integration test runs

Closes #1374

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-17 17:50:52 +0000 UTC
    </div>
</div>

