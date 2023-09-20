---
layout: default
title: fabric-chaincode-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-chaincode-go
---

# fabric-chaincode-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-chaincode-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/84" class=".btn">#84</a>
            </td>
            <td>
                <b>
                    Draft: Resolves #80, Bumped fabric-proto-go to fabric-protos-go-apiv2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Draft: This is a working change on bumping the fabric-chaincode-go to use fabric-protos-go-apiv2 and the new protobufs lib. This commits includes changes to fuction signatures, return values, interface definition and type definition to type "ChaincodeMessage" and "pb.Response".

 It is a breaking change.
 
 Here is a repository with a branch that house the state of the codebase after resolving the imports with fabric-protos-go-apiV2 lib, this does not breaks anything yet and it is intended to showcase to the maintainers the complaint of the `go vet` . The `go vet ./...` command should be run at the root of the project.

 https://github.com/tobigiwa/fabric-chaincode-go/tree/fix

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-17 08:15:38 +0000 UTC
    </div>
</div>

