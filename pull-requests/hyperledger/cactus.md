---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2075" class=".btn">#2075</a>
            </td>
            <td>
                <b>
                    fix: fixed 2 lint errors that were the any type error for Typescript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixed 2 lint errors that were the any type error for Typescript and removed Node

Signed-off-by: Alec Phong <alecphong@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-13 19:01:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2072" class=".btn">#2072</a>
            </td>
            <td>
                <b>
                    docs(build): add text build steps for Linux, Mac and Windows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Issue: #1963

Signed-off-by: Abhinav Srivastava (abhinavmir#1898 on Discord)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-10 02:13:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2071" class=".btn">#2071</a>
            </td>
            <td>
                <b>
                    feat(fabric-socketio-connector): sending transactions signed on the client-side
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                - Add functions to support entire process of sending transaction to the ledger without sharing
  any private key with the connector.
- Add test cases to check the new functionalities.
- Adjust asset-trade sample app to use new logic that doesn't send the private key to the connector.
- Move fabric signing utils to a separate file.
- Add fabric protobuf serializers and deserializers, so they can be send back and forth
  between connector and BLP without loosing type information.
- Add an option to FabricTestLedgerV1 to allow attaching to already running ledger container.
  This can speed up test development/troubleshoot process.
- Improve fabric-all-in-one ledger healthcheck, so that it waits for basic chaincode intialization.
  This is not strictly needed by current tests, but may be expected by future tests.
- Refactor duplicated logic in fabric-connector.
- Fix fabric-socketio module entry points (minor fix).

Closes: #2070

Depends on #2047

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

-------------

As always, please review only the last commit. Remaining ones are just dependencies, that will be squashed before an actual merge.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-07 15:48:30 +0000 UTC
    </div>
</div>

