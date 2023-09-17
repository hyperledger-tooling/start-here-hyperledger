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
                    Resolves #80, Bumped fabric-proto-go to fabric-protos-go-apiv2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves #80, this commit contains dependency update from fabric-protos-go to fabric-protos-go-apiv2 and "github.com/golang/protobuf"(deprecated) to "google.golang.org/protobuf

Bumped google.golang.org/protobuf to v1.31.0 from v1.5.2

It can be noticed that the package "github.com/golang/protobuf" is still an indirect dependency used by google.golang.org/grpc/credentials v1.53.0, even the latest update v1.58.0 still does.

Made sure all tests passed.

CHANGES INCLUDE:

	SOURCE CODE
The "AssertProtoEqual" was borrowed from: // https://github.com/hyperledger/fabric-gateway/blob/cd1bc1f3fcf007bd97244120d9a8d112153322cd/pkg/internal/test/transaction.go#L20-L22 which is more apt to test the Protobufs of google.golang.org/protobuf/ implementation. It replaced assertEqual.

now := ptypes.TimestampNow() --> now := timestamp.Now()

IMPORTS
All Import aliases are kept.
"github.com/golang/protobuf/proto" --> "google.golang.org/protobuf/proto"

pb "github.com/hyperledger/fabric-protos-go/peer" --> pb "github.com/hyperledger/fabric-protos-go-apiv2/peer"

"github.com/golang/protobuf/ptypes/timestamp" --> timestamp "google.golang.org/protobuf/types/known/timestamppb"

"github.com/hyperledger/fabric-protos-go/ledger/queryresult" --> "github.com/hyperledger/fabric-protos-go-apiv2/ledger/queryresult"

"github.com/hyperledger/fabric-protos-go/ledger/msp" → "github.com/hyperledger/fabric-protos-go-apiv2/ledger/msp" "github.com/hyperledger/fabric-protos-go/common" --> "github.com/hyperledger/fabric-protos-go-apiv2/common"
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-17 08:15:38 +0000 UTC
    </div>
</div>

