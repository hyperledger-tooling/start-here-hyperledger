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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/684" class=".btn">#684</a>
            </td>
            <td>
                <b>
                    Provide clear guidance for running Java chaincode in a debugger - DO NOT MERGE
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

