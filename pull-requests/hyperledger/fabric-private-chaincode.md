---
layout: default
title: fabric-private-chaincode
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-private-chaincode
---

# fabric-private-chaincode <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-private-chaincode){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/681" class=".btn">#681</a>
            </td>
            <td>
                <b>
                    Upgrade ego
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR upgrades ego to v1.0.0. With the new ego bundle command, which
packages the signed enclave binary with the ego runtime, there is no
need for the dedicated `fpc-ccenv-go` image anymore as we can just use
`fpc-ccenv` with the bundled chaincode.

- Upgrade to ego v1.0.0
- Remove fpc-ccenv-go
- Upgrade `go.mod` to go 1.17
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-29 16:05:17 +0000 UTC
    </div>
</div>

