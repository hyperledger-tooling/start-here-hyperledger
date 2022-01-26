---
layout: default
title: fabric-private-chaincode
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/fabric-private-chaincode
---

# fabric-private-chaincode <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-private-chaincode){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    FPC v1.0 RC3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.0.0-rc3
                </span>
            </td>
            <td>
                This is the third release candidate of Fabric Private Chaincode (FPC) v1.0.0

The release focuses on the integration with [Fabric Smart Client](https://github.com/hyperledger-labs/fabric-smart-client). Additionally, the release comes with several improvements and bug fixes. More details see `CHANGELOG.md`.

## What's Changed
* Fixed the version of fabric-ccenv to 2.3.0 by @ikegawa-koshi in https://github.com/hyperledger/fabric-private-chaincode/pull/629
* Updated helloworld readme by @ricc-zappoli in https://github.com/hyperledger/fabric-private-chaincode/pull/631
* Upgrade go and fabric by @mbrandenburger in https://github.com/hyperledger/fabric-private-chaincode/pull/633
* Demo FSC integration using the IRB demo by @mbrandenburger in https://github.com/hyperledger/fabric-private-chaincode/pull/635
* Fix sgx device location for dcap machines by @bvavala in https://github.com/hyperledger/fabric-private-chaincode/pull/639
* Extend FPC Shim support by @mbrandenburger in https://github.com/hyperledger/fabric-private-chaincode/pull/637
* Upgrade parson by @mbrandenburger in https://github.com/hyperledger/fabric-private-chaincode/pull/642
* Add stress test for many invocations and fix memory leak by @mbrandenburger in https://github.com/hyperledger/fabric-private-chaincode/pull/641
* Add del_state support by @mbrandenburger in https://github.com/hyperledger/fabric-private-chaincode/pull/640
* Link existing FSC examples by @mbrandenburger in https://github.com/hyperledger/fabric-private-chaincode/pull/648
* Update IRB readme by @mbrandenburger in https://github.com/hyperledger/fabric-private-chaincode/pull/647

## New Contributors
* @ricc-zappoli made their first contribution in https://github.com/hyperledger/fabric-private-chaincode/pull/631

**Full Changelog**: https://github.com/hyperledger/fabric-private-chaincode/compare/v1.0.0-rc2...v1.0.0-rc3
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/fabric-private-chaincode/releases/tag/v1.0.0-rc3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-01-26 17:15:05 +0000 UTC
    </span>
</div>

