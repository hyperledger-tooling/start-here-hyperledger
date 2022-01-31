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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/605" class=".btn">#605</a>
            </td>
            <td>
                <b>
                    Run basic-asset-transfer on the Kubernetes Test Network in an Azure CI pipeline 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                DO NOT MERGE 

This PR adds an Azure test suite to run the basic asset transfer sample application on the Kubernetes Test Network.

I am using this branch / PR to troubleshoot / debug the Azure pipeline.  DO NOT MERGE. 

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-28 18:03:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/604" class=".btn">#604</a>
            </td>
            <td>
                <b>
                    Podman nerdctl experiement - DO NOT MERGE
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
        Created At 2022-01-28 16:15:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/601" class=".btn">#601</a>
            </td>
            <td>
                <b>
                    Fix markdown logical structure in asset-transfer-events/README.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fenced code blocks within a list were at the wrong level if indentation and so logically terminated the list.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 17:05:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/600" class=".btn">#600</a>
            </td>
            <td>
                <b>
                    Refactor of asset transfer events Go sample for Fabric Gateway
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Split boiler-plate connection code into a separate file since the basic sample already covers this aspect. The `app.go` file now only presents the main application code, making it much easier for readers to view.

Also changed the event replay code to use a different style of reading from the real-time eventing example, demonstrating the use of timeouts while reading events we expect to arrive quickly, and avoiding any possibility of the main application execution hanging indefinitely.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 12:27:35 +0000 UTC
    </div>
</div>

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

