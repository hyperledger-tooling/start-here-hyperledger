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
                PR <a href="https://github.com/hyperledger/fabric-sdk-go/pull/177" class=".btn">#177</a>
            </td>
            <td>
                <b>
                    Fixed a bug in proposal matcher when querying committed chaincodes. P…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes an error in the proposal matcher with an unexpected order of committed chaincodes returned from a peer. The matcher uses `proto.Equal` which fails to compare the values of slices that are in a different order.   
Two peers return the same list of the chaincodes in a slice instead of a map, that's why the order can't be guaranteed https://github.com/hyperledger/fabric/blob/main/core/chaincode/lifecycle/scc.go#L620.

Signed-off-by: Vladyslav Kopaihorodskyi <vlad.kopaygorodsky@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 15:50:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-go/pull/176" class=".btn">#176</a>
            </td>
            <td>
                <b>
                    add HSM Identity proposal
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Hello, we are trying to use HSM with the GO SDK, our objective is to use it with a wallet, some kind of identityprovider, we are creating this PR to interact with you, so you can guide us further:

- Is this the right approach for this project?
- Using Cryptosuite with PKCS11 interface is not as clear as we wanted it to be.
- Using identitymanager or using the mspwallet to create a manager is not explained thoroughly

We want to do something like this(inspired by the node SDK): https://github.com/hyperledger/fabric-sdk-node/blob/main/fabric-network/src/impl/wallet/hsmx509identity.ts 

We have some of the possible interfaces and some of the functions, but when we think how to link everything with a wallet, we just don't know if the path we are following is correct

Hope you can guide us, thanks a lot!
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-25 14:48:45 +0000 UTC
    </div>
</div>

