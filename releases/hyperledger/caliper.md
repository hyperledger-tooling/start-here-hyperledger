---
layout: default
title: caliper
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/caliper
---

# caliper <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/caliper){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v0.6.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.6.0
                </span>
            </td>
            <td>
                # Notable

## Security Fixes
💥Address issue in Prometheus monitor that allowed an abitrary binary to be downloaded and executed on a system running a Caliper worker

## New features
✨ Official support for Node 18 and Node 20 for users and contributors

## Breaking
💥Caliper no longer supports Fisco-BCOS


# Complete list

## What's Changed
* Fix #536 Update error messages for 'caliper-cli' package by @0xt3j4s in https://github.com/hyperledger/caliper/pull/1348
* Port the unit test workflow to GitHub Actions by @CaptainIRS in https://github.com/hyperledger/caliper/pull/1364
* Port the integration test workflow to GitHub Actions by @CaptainIRS in https://github.com/hyperledger/caliper/pull/1376
* Disable unit and integration tests in Azure Pipelines by @CaptainIRS in https://github.com/hyperledger/caliper/pull/1382
* Fix #536 Update error messages for 'caliper-ethereum' package by @0xt3j4s in https://github.com/hyperledger/caliper/pull/1363
* Port the publish workflow to GitHub Actions by @CaptainIRS in https://github.com/hyperledger/caliper/pull/1384
* Pass secrets to CI workflow for publish by @CaptainIRS in https://github.com/hyperledger/caliper/pull/1390
* Fix#1377 Change the generator binding from 2.2 to 1.4 by @0xt3j4s in https://github.com/hyperledger/caliper/pull/1391
* Fix #536: Minor changes in the error messages of 'caliper-fisco-bcos' package by @0xt3j4s in https://github.com/hyperledger/caliper/pull/1383
* Add DCI linting to CI of PRs by @aklenik in https://github.com/hyperledger/caliper/pull/1393
* Updated fabric bindings by @fraVlaca in https://github.com/hyperledger/caliper/pull/1402
* Migrate Fabric integration tests to test network by @CaptainIRS in https://github.com/hyperledger/caliper/pull/1410
* Remove channel and chaincode operations from Fabric v1 connector by @CaptainIRS in https://github.com/hyperledger/caliper/pull/1411
* update fabric bindings by @davidkel in https://github.com/hyperledger/caliper/pull/1412
* Migrate to npm workspaces by @CaptainIRS in https://github.com/hyperledger/caliper/pull/1394
* Migrate generator tests to test network by @CaptainIRS in https://github.com/hyperledger/caliper/pull/1414
* Cache node modules across CI workflows by @CaptainIRS in https://github.com/hyperledger/caliper/pull/1406
* Execute integration tests based on changes by @CaptainIRS in https://github.com/hyperledger/caliper/pull/1421
* Add workflow for gh-pages branch by @CaptainIRS in https://github.com/hyperledger/caliper/pull/1423
* Revert "Add workflow for gh-pages branch" by @CaptainIRS in https://github.com/hyperledger/caliper/pull/1425
* Distinguish different workers in Prometheus PushGateway by @CaptainIRS in https://github.com/hyperledger/caliper/pull/1427
* Add coverage report workflow by @CaptainIRS in https://github.com/hyperledger/caliper/pull/1428
* Upload coverage reports on merge by @CaptainIRS in https://github.com/hyperledger/caliper/pull/1433
* Vscode extension by @eravatee in https://github.com/hyperledger/caliper/pull/1404
* Add Node 18 to CI by @CaptainIRS in https://github.com/hyperledger/caliper/pull/1455
* Fix calculation and doc comment in prometheus observer by @CaptainIRS in https://github.com/hyperledger/caliper/pull/1456
* Revert "Add Node 18 to CI (#1455)" by @CaptainIRS in https://github.com/hyperledger/caliper/pull/1460
* Fix integration test CI trigger by @CaptainIRS in https://github.com/hyperledger/caliper/pull/1458
* Add TxObserver for Prometheus manager by @CaptainIRS in https://github.com/hyperledger/caliper/pull/1448
* Bump moment-timezone from 0.5.34 to 0.5.38 by @dependabot in https://github.com/hyperledger/caliper/pull/1461
* Move inactive maintainers to emeritus status by @ryjones in https://github.com/hyperledger/caliper/pull/1462
* Add CODEOWNERS file by @ryjones in https://github.com/hyperledger/caliper/pull/1463
* Fix npmignore for report html by @CaptainIRS in https://github.com/hyperledger/caliper/pull/1466
* Update cache action by @CaptainIRS in https://github.com/hyperledger/caliper/pull/1469
* Add skeleton for development and proposal docs by @aklenik in https://github.com/hyperledger/caliper/pull/1400
* Use go chaincode in integration tests by @CaptainIRS in https://github.com/hyperledger/caliper/pull/1484
* Update go chaincode dependencies in integration tests by @CaptainIRS in https://github.com/hyperledger/caliper/pull/1485
* docker monitor remote monitoring bugfix in https://github.com/hyperledger/caliper/pull/1499
* Terminate workers if caliper manager is terminated prematurely by @davidkel in https://github.com/hyperledger/caliper/pull/1514
* Remove fisco-bcos by @davidkel in https://github.com/hyperledger/caliper/pull/1515
* test node 18/20, minimum version 18.19.0 by @davidkel in https://github.com/hyperledger/caliper/pull/1517
* Temporarily revert publish to using node 16.x to fix broken publish by @davidkel in https://github.com/hyperledger/caliper/pull/1520
* downgrade npm on publish as temp fix by @davidkel in https://github.com/hyperledger/caliper/pull/1523
* Update the versions of fabric sdks by @davidkel in https://github.com/hyperledger/caliper/pull/1519
* Update PSWG whitepaper link in README #1518 by @vinayakjaas in https://github.com/hyperledger/caliper/pull/1524
* Remove Caliper-gui-server packages and Caliper-gui-dashboard packages  #1538 by @vinayakjaas in https://github.com/hyperledger/caliper/pull/1540
* Remove collection of node gc stats in prometheus by @davidkel in https://github.com/hyperledger/caliper/pull/1545
* Removed unused dependencies by @psankhe28 in https://github.com/hyperledger/caliper/pull/1544

## Special Thanks
* @CaptainIRS For the excellent contributions in in particular to the move to npm workspaces and the Caliper build environment

## New Contributors
* @0xt3j4s made their first contribution in https://github.com/hyperledger/caliper/pull/1348
* @eravatee made their first contribution in https://github.com/hyperledger/caliper/pull/1404
* @dependabot made their first contribution in https://github.com/hyperledger/caliper/pull/1461
* @psankhe28 made their first contribution in https://github.com/hyperledger/caliper/pull/1544

**Full Changelog**: https://github.com/hyperledger/caliper/compare/v0.5.0...v0.6.0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/caliper/releases/tag/v0.6.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-05-01 14:45:49 +0000 UTC
    </span>
</div>

