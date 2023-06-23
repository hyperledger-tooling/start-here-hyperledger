---
layout: default
title: firefly-fabconnect
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-fabconnect
---

# firefly-fabconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-fabconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-fabconnect/pull/111" class=".btn">#111</a>
            </td>
            <td>
                <b>
                    Fix panic in un-register
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Seen in testing:
```
[2023-06-19T01:42:33.888Z] ERROR Listening ended with: http: Server closed
panic: runtime error: invalid memory address or nil pointer dereference
[signal SIGSEGV: segmentation violation code=0x1 addr=0x10 pc=0xb9831d]

goroutine 2358 [running]:
github.com/hyperledger/firefly-fabconnect/internal/fabric/client.(*txSubmitAndListenHandler).Handle(0xc0010ba1e0, 0xc000351680, 0xc001885800)
	/fabconnect/internal/fabric/client/invokehandler.go:58 +0x33d
github.com/hyperledger/fabric-sdk-go/pkg/client/channel/invoke.(*SignatureValidationHandler).Handle(0xc00177bf10, 0xc000351680, 0x2)
	/go/pkg/mod/github.com/hyperledger/fabric-sdk-go@v1.0.1-0.20220617091732-e170b98fa821/pkg/client/channel/invoke/signature.go:37 +0x75
github.com/hyperledger/fabric-sdk-go/pkg/client/channel/invoke.(*EndorsementValidationHandler).Handle(0xc00177bf20, 0xc000351680, 0x2b)
	/go/pkg/mod/github.com/hyperledger/fabric-sdk-go@v1.0.1-0.20220617091732-e170b98fa821/pkg/client/channel/invoke/txnhandler.go:161 +0x6d
github.com/hyperledger/fabric-sdk-go/pkg/client/channel/invoke.(*SelectAndEndorseHandler).Handle(0xc001755920, 0xc000351680, 0xc001885800)
	/go/pkg/mod/github.com/hyperledger/fabric-sdk-go@v1.0.1-0.20220617091732-e170b98fa821/pkg/client/channel/invoke/selectendorsehandler.go:90 +0x522
github.com/hyperledger/fabric-sdk-go/pkg/client/channel.(*Client).InvokeHandler.func2.1()
	/go/pkg/mod/github.com/hyperledger/fabric-sdk-go@v1.0.1-0.20220617091732-e170b98fa821/pkg/client/channel/chclient.go:182 +0x2f
github.com/hyperledger/fabric-sdk-go/pkg/common/errors/retry.(*RetryableInvoker).Invoke(0xc001827d40, 0xc000327fa8)
	/go/pkg/mod/github.com/hyperledger/fabric-sdk-go@v1.0.1-0.20220617091732-e170b98fa821/pkg/common/errors/retry/invoker.go:63 +0x16d
github.com/hyperledger/fabric-sdk-go/pkg/client/channel.(*Client).InvokeHandler.func2()
	/go/pkg/mod/github.com/hyperledger/fabric-sdk-go@v1.0.1-0.20220617091732-e170b98fa821/pkg/client/channel/chclient.go:180 +0x7a
created by github.com/hyperledger/fabric-sdk-go/pkg/client/channel.(*Client).InvokeHandler
	/go/pkg/mod/github.com/hyperledger/fabric-sdk-go@v1.0.1-0.20220617091732-e170b98fa821/pkg/client/channel/chclient.go:179 +0x471
rpc error: code = Unknown desc = Error: No such container: 8168efe9b5f15559cfcd382ff31843c3aa6434e8d0c6edac0b76030c8b757a9d
```

Reading the Fabric docs, the channel is closed on `Unregister` - so a `nil` result should be tolerated:
https://github.com/hyperledger/firefly-fabconnect/blob/b46951bb6613a2981b89c3ea2e69048441ec41ed/internal/fabric/client/invokehandler.go#L58
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-19 02:07:07 +0000 UTC
    </div>
</div>

