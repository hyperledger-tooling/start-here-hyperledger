---
layout: default
title: fabric-chaincode-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-chaincode-java
---

# fabric-chaincode-java

You can clone this repo on <span class="fs-3">[GitHub](https://github.com/hyperledger/fabric-chaincode-java){: .btn .mr-4 }</span>


<div class="code-example" markdown="1">
    <table>
        <tr>
            <td>
                PR [#175](https://api.github.com/repos/hyperledger/fabric-chaincode-java/pulls/175)
            </td>
            <td>
                <b>
                    NettyGrpcServer -- configure ALPN to enable TLS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Without ALPN configured, the following exception is thrown when one tries to instantiate NettyChaincodeServer with TLS enabled:

```
java.lang.IllegalArgumentException: ALPN must be enabled and list HTTP/2 as a supported protocol.
	at com.google.common.base.Preconditions.checkArgument(Preconditions.java:142)
	at io.grpc.netty.shaded.io.grpc.netty.GrpcSslContexts.ensureAlpnAndH2Enabled(GrpcSslContexts.java:260)
	at io.grpc.netty.shaded.io.grpc.netty.NettyServerBuilder.sslContext(NettyServerBuilder.java:300)
	at org.hyperledger.fabric.shim.NettyGrpcServer.<init>(NettyGrpcServer.java:60)
	at org.hyperledger.fabric.shim.NettyChaincodeServer.<init>(NettyChaincodeServer.java:27)
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-22 14:52:01 +0000 UTC
    </div>
</div>

