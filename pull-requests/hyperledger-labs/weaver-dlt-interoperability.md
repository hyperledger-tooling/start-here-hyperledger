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
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/118" class=".btn">#118</a>
            </td>
            <td>
                <b>
                    changing asset exchange interop cc as package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Below changes are made via this PR:
1. Created `assetexchange` library/package inside core/network/fabric-interop-cc/libs
2. Called functions from this library/package in the asset exchange chaincode core/network/fabric-interop-cc/contracts/interop/manage_assets.go

Signed-off-by: Krishnasuri Narayanam <knaraya3@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-23 16:04:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/117" class=".btn">#117</a>
            </td>
            <td>
                <b>
                    Clean Up following use of modules, fix Asset-Mgmt module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Deleted `protos-go` and `protos-js` directories.
2. Deleted scripts in various places which is used to copy protos and build manually, (since this is being done in common folder, use that if you want to build locally).
3. Deleted commented codes from various makefiles and scripts (If want to use local protos, point to folders in `/common`)
4. Use interopcc `v1.2.1` in testnet.
5. Added mocks folder to `asset-mgmt`, as otherwise using it as go module used to throw error that mocks not found.
6. Simpleasset modified to import `asset-mgmt` as module. To test it, manually copy folder `core/network/fabric-interop-cc/interfaces/asset-mgmt` from my fork to your path: `$GOPATH/pkg/mod/github.com/hyperledger-labs/weaver-dlt-interoperability/core/network/fabric-interop-cc/interfaces/asset-mgmt@v1.2.1`.

Tested all 6 Interop calls, and local unit tests, and end to end asset-exchange after these changes, and it works fine for me.

Update:
1.  Included GRPC protos in protos-go compilation. 
2. Fixed `go_packages` in protos.
3. Using scripts to fetch corda interop modules instead of using build.gradle (apparently this seems to be better option)
4. Docs: removed all local build steps, fixed typos.
5. Removed unused dependencies from `interoperation-node-sdk` and `fabric-driver`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-21 07:09:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/116" class=".btn">#116</a>
            </td>
            <td>
                <b>
                    go-sdk for performing asset exchange
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
        Created At 2021-07-19 19:04:04 +0000 UTC
    </div>
</div>

