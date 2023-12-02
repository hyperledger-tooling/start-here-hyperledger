---
layout: default
title: fabric-gateway
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-gateway
---

# fabric-gateway <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-gateway){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/661" class=".btn">#661</a>
            </td>
            <td>
                <b>
                    Update dependencies to mitigate CVE-2023-44487
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This vulnerability can be exploited in gRPC servers (not clients) so should not directly impact the Fabric Gateway client API. However, updates to gRPC Java dependencies enables compatibility with Netty version 4.1.101.Final, which contains mitigations to this vulnerability and supports client applications that also expose gRPC services.

See:

- https://github.com/grpc/grpc-java/releases/tag/v1.59.1
- https://github.com/grpc/grpc-java/issues/10617

Also:

- Update dependency-check-maven to avoid use of sunset NVD data-feed.
- Update Go dependencies.
- Update Node dev-dependencies.
- Use GitHub actions/setup-java@v4.
- Fix deadlock in Java 8 / 11 scenario tests.

Closes #659
Closes #660
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-02 14:45:09 +0000 UTC
    </div>
</div>

