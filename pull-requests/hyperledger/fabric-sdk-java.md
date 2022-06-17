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
                PR <a href="https://github.com/hyperledger/fabric-sdk-java/pull/207" class=".btn">#207</a>
            </td>
            <td>
                <b>
                    Performance improvement for CryptoPrimitives
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Every request required a creation of a new BouncyCastleProvider which is a very expensive operation.

Furthermore, certificates were re-parsed and their chains re-validated on every reques. Again this is a very expensive operation.

Taken together these factors caused excessive delays in interacting with the Fabric block chain.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-17 12:51:08 +0000 UTC
    </div>
</div>

