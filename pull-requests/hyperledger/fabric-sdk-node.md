---
layout: default
title: fabric-sdk-node
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-node
---

# fabric-sdk-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/683" class=".btn">#683</a>
            </td>
            <td>
                <b>
                    Use require to import long
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Explicit require provides better TypeScript compatibility regardless of esModuleInterop setting.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-07 22:25:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/682" class=".btn">#682</a>
            </td>
            <td>
                <b>
                    Fixes required by changes to typing in dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Scheduled build began failing last week, with the typing / import errors related to the version of the `long` package inherited from the protobuf packages. Add explicit dependencies on the `long` package and adjust imports accordingly.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-03 17:13:44 +0000 UTC
    </div>
</div>

