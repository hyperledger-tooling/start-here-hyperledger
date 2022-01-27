---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/599" class=".btn">#599</a>
            </td>
            <td>
                <b>
                    fix a bug in function [getBlockByNumber]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This bug can lead to users can't change target peer to send query operations.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 11:45:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/598" class=".btn">#598</a>
            </td>
            <td>
                <b>
                    Fix CHAINCODE_AS_A_SERVICE_TUTORIAL.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes several typos and more importantly add an instruction to
set FABRIC_CFG_PATH without which the peer command fails.

Signed-off-by: Arnaud J Le Hors <lehors@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 07:45:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/597" class=".btn">#597</a>
            </td>
            <td>
                <b>
                    Asset transfer events Go sample for Fabric Gateway
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-26 19:37:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/596" class=".btn">#596</a>
            </td>
            <td>
                <b>
                    Experimental Support for using podman with the test-network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Podman support
_Note: currently experimental, only 2 org currently modified_

A copy of the `install_fabric.sh` script is in the `test-network` directory. This has been enhanced to support a `podman` argument; if used it will use `podman` to pull down images and tag them rather than docker. The images are the same, but need to pulled differently.

The `network.sh` script has been enhanced so that it can use `podman` and `podman-compose` instead of docker. Ensure that `CONTAINER_CLI` is set as below when running anet `network.sh` script. 

```bash
CONTAINER_CLI=podman ./network.sh up
````

As there is no Docker-Daemon in this context, only Chaincode-as-a-service is supported.

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-26 09:54:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/595" class=".btn">#595</a>
            </td>
            <td>
                <b>
                    ERC20 Java chaincode implementation exmaple.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: renjithkn@gmail.com <renjithkn@gmail.com>

This is an example of ERC20 token standard Java chaincode implementation.  The functionality is the same as the existing go and nodejs ERC20 chaincode.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-24 16:56:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/589" class=".btn">#589</a>
            </td>
            <td>
                <b>
                    Remove JCenter as a Gradle package repository
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                JCenter is deprecated, can no longer be published to, and is scheduled for removal. It is now causing build failures. Replace with Maven Central.

Also remove mavenLocal() as this is not recommended practice:
    
https://docs.gradle.org/current/userguide/declaring_repositories.html#sec:case-for-maven-local

Note that Jitpack still needs to be included as a package repository for Java chaincode since it has dependencies on an old version of com.github.everit-org.json-schema:org.everit.json.schema that is only published there.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-21 09:20:34 +0000 UTC
    </div>
</div>

