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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/108" class=".btn">#108</a>
            </td>
            <td>
                <b>
                    Modules via Github Packages PR-1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Created modules for protos for javascript, go, and java/kotlin, along with steps to publish it in github packages.
2. Created NodeJS module in github packages for interop-node-sdk with name changed to `@hyperledger-labs/weaver-fabric-interop-sdk`.
3. Modified interop-node-sdk, fabric-driver, fabric-cli to use weaver modules from github packages.
4. Created docker images for relay and fabric-driver and pushed in github registry.
5. Modified docs in order to be consistent with above changes.

Changes remaining for modularization will be in next PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-12 09:19:53 +0000 UTC
    </div>
</div>

