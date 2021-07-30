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
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/121" class=".btn">#121</a>
            </td>
            <td>
                <b>
                    Update Expired fabric crypto materials.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-30 06:16:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/120" class=".btn">#120</a>
            </td>
            <td>
                <b>
                    Corda Interop App Improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Fix java package names in protos to include `com.weaver.protos` prefix.
2. Fix `interop-contracts` to work with SpringBoot framework (a requirement from Marcopolo demo application).
3. Use full version in corda modules for weaver dependencies, and upgrade versions to `1.2.3`.
4. Combined corda-client two gradle build files `build.gradle.local` and `build.gradle.remote` into one `build.gradle`, which decides local or remote based on presence of `artifactory.properties`.

**NOTE:** To test these changes, kindly change `url` in all `artifactory.properties`, replace `hyperledger-labs` with `sanvenDev`. Currently these modules are published on my fork.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-28 12:43:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/119" class=".btn">#119</a>
            </td>
            <td>
                <b>
                    new app to demonstrate use of assetexchange cc package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Changes made:
- Added new application `assetexchangeandinterop` to demonstrate the use of `assetexchange` chaincode package
- Updated interop-cc to refer to published `assetexchange` chaincode package
 
Signed-off-by: Krishnasuri Narayanam <knaraya3@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-27 10:19:16 +0000 UTC
    </div>
</div>

