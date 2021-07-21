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
3. Deleted commented codes from various makefiles and scripts.
4. Use interopcc `v1.2.1` in testnet.
5. Added mocks folder to `asset-mgmt`, as otherwise using it as go module used to throw error that mocks not found.
6. Simpleasset modified to import `asset-mgmt` as module, currently it imports from my fork, but will later (in a separate PR) modify it to point to hyperledger-labs, since right now I can't generate `go.sum` entry.

Tested all 6 Interop calls, and local unit tests, and end to end asset-exchange after these changes, and it works fine for me.
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/114" class=".btn">#114</a>
            </td>
            <td>
                <b>
                    protos and protos-go updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change-set does the following:
- It updates the go_package to specify the full path
- It updates the proto package to remove the dots
- It modify the proto go build process to split the compilation in multiple calls to protoc, one for each folder
This way, the protos that can be compiled the same version of protoc used for Fabric
- Update the go module for the protos-go

Signed-off-by: Angelo De Caro <adc@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-18 05:08:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/112" class=".btn">#112</a>
            </td>
            <td>
                <b>
                    Modules via Github Packages - PR-2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Changes: 
1. Interoperation Cordapp package name changed to `com.weaver.corda.app.interop` and added steps to publish to github packages.
2. Modified all apps to use modules in github packages when not using `-local` in make commands. (Retained the functionality of make commands with `-local` suffix).
3. Modified go chaincodes to use previously published `protos-go`.
4. Interop-cc now being fetched as go module from github to install on testnet.

Close #111 .

Fixes:
1. Resolved #110 : Now compiled grpc go files are also created.
2. Resolved #109 : Added go.sum.

Comments before testing:
1. To start testnet there are two options:

- Fetch local copy: Uncomment line 45 and comment line 46 in `tests/network-setups/fabric/dev/Makefile`.
- Fetch remotely from my fork: Replace `hyperledger-labs` with `sanvenDev` in `line 7` and with `sanven\!dev` in `line 17`
in file: `tests/network-setups/fabric/dev/scripts/setupCC.sh`.

2. Replace `hyperledger-labs` with `sanvenDev` in `url` field in all `artifactory.properties`. (Currently I've published apps to my fork for testing, once approved I'll publish those in hyperledger-labs)

(Once this PR is merged, these steps won't be required)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-15 13:35:33 +0000 UTC
    </div>
</div>

