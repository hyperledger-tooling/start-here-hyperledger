---
layout: default
title: fabric-chaincode-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-chaincode-java
---

# fabric-chaincode-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-chaincode-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/330" class=".btn">#330</a>
            </td>
            <td>
                <b>
                    Upgrade Gradle version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Include build of the Docker image in tests run on a pull request to ensure the Docker image at least builds cleanly.

The integration tests use builders baked into Microfab rather than real Fabric builders and the chaincode Docker images. This means the bare-gradle test chaincode is built using the Gradle version supplied by Microfab, not the version included in the Java chaincode Docker images, and has to be left with outdated plugin versions and build.gradle content.

Closes #326
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-25 17:52:02 +0000 UTC
    </div>
</div>

