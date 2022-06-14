---
layout: default
title: fabric-sdk-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-go
---

# fabric-sdk-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-go/pull/236" class=".btn">#236</a>
            </td>
            <td>
                <b>
                    Add SubmitInit() to support chaincodes that require init
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Even though the latest recommendation from the Fabric team is to step away from requiring `init`, a lot of customers still use this approach, and the official docs for Fabric chaincode lifecycle still describes the `--init-required` parameter, finally the `fabric-samples` that is used widely by tire-kickers still implements `InitLedger()`.

Added a new `SubmitInit()` instead of modifying the existing signature to allow backward compatibility
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-10 14:19:47 +0000 UTC
    </div>
</div>

