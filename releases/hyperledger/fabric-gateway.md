---
layout: default
title: fabric-gateway
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/fabric-gateway
---

# fabric-gateway <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-gateway){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v1.3.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.3.0
                </span>
            </td>
            <td>
                ## What's Changed
* Use @noble/curves for Node signing by @bestbeforetoday in https://github.com/hyperledger/fabric-gateway/pull/565
* Add implementations for all hashes supported by Fabric v2.5 by @bestbeforetoday in https://github.com/hyperledger/fabric-gateway/pull/580
* Require at least Node 16 and Go 1.19 by @bestbeforetoday in https://github.com/hyperledger/fabric-gateway/pull/584
* Remove Netty dependency from Java package by @bestbeforetoday in https://github.com/hyperledger/fabric-gateway/pull/587
* Ed25519 signer implementations by @bestbeforetoday in https://github.com/hyperledger/fabric-gateway/pull/596

## Migration considerations

Java applications are now _required_ to have an explicit dependency on a suitable gRPC channel service provider. Earlier versions of the [org.hyperledger.fabric/fabric-gateway](https://central.sonatype.com/artifact/org.hyperledger.fabric/fabric-gateway) Java package included [io.grpc/grpc-netty-shaded](https://central.sonatype.com/artifact/io.grpc/grpc-netty-shaded) as a dependency. This dependency has been removed, which allows client applications the flexibility to select a gRPC channel service provider most suitable to their runtime environment when creating a gRPC connection. See the [gRPC security documentation](https://github.com/grpc/grpc-java/blob/master/SECURITY.md#transport-security-tls) for details of the available providers.

**Full Changelog**: https://github.com/hyperledger/fabric-gateway/compare/v1.2.2...v1.3.0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/fabric-gateway/releases/tag/v1.3.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-06-19 08:28:18 +0000 UTC
    </span>
</div>

