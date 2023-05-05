---
layout: default
title: fabric-sdk-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-java
---

# fabric-sdk-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-java/pull/280" class=".btn">#280</a>
            </td>
            <td>
                <b>
                    Remove netty-tcnative-boringssl-static dependency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Not required since tcnative with BoringSSL is already included in grpc-netty-shaded dependency.
    
Also update Bouncy Castle dependency to implementations for Java 1.8 and later only.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-05 14:03:40 +0000 UTC
    </div>
</div>

