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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/692" class=".btn">#692</a>
            </td>
            <td>
                <b>
                    test-network-k8s : Connect to Fabric services via Nginx Ingress - DO NOT MERGE
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                DRAFT PR - DO NOT MERGE 

This PR updates the Kube test network to access Fabric services via an Ingress controller.  This allows for easy access to the CAs, peers, orderers, and load-balanced Gateway Peer via the nginx bound to localhost:443.

In previous iterations, any administration of the network involved a remote exec to execute commands on an "admin CLI pod" running in the cluster.  In addition, any time files needed to get to/from the volume mounts in Kubernetes, an overly complicated sequence of arcane `exec tar --.... ` commands was necessary.

With this PR, the network is instantiated, exposing core services at the *.vcap.me (wildcard match to 127.0.0.1) DNS domain.  Fabric binaries are run directly on the host, and certificate enrollments are managed locally as if they were maintained in a local wallet storage.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-29 15:14:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/689" class=".btn">#689</a>
            </td>
            <td>
                <b>
                    Update the REST Example
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. For development purposes CORS can hinder testing examples. Therefore enable CORS if needed, default off
2. The default chaincode use Capitalized JSON Names, whereas for new asset the REST validation didn't.. Adjusted
so it matches the chaincode

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-28 12:25:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/684" class=".btn">#684</a>
            </td>
            <td>
                <b>
                    Provide clear guidance for running Java chaincode as a service
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **DRAFT PR - DO NOT MERGE** 

This PR addresses the need for a simple, clear example that illustrates the use of Chaincode-as-a-Service to build and run Java chaincode on a local development environment.

In addition, the README includes a section that describes how users may employ a Docker loopback interface to connect from a remote Peer binary to a local port on the host OS.  In this manner, chaincode may be run locally while attached to a debugger, with the peer running on a remote pod in Kubernetes.

Items in this PR that need additional focus / review / input: 

- The PR introduces a new "ccpackage/" folder, with the expectation that all of the ccaas-enabled samples will follow this convention.  In ccpackage/, the sample includes the metadata, connection, and new "ccaas.json" descriptors.  This is not an ideal approach, but we need some way for each of the samples to declare the target chaincode image to build and deploy in k8s.

- Additional testing on the `host.docker.internal` DNS alias is required (e.g. Win, Linux, revs of Docker, etc.) 

-  The doc sets up a flow with three installations of the same chaincode, but does not delete the chaincode between steps.  (How does one _delete_ a chaincode, btw?) 

-  file-based arguments must all be absolute paths.  This can be fixed either in this PR or a follow-on. 



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-23 14:40:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/683" class=".btn">#683</a>
            </td>
            <td>
                <b>
                    Fix typo
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
        Created At 2022-03-23 07:16:59 +0000 UTC
    </div>
</div>

