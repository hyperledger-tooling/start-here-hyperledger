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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/727" class=".btn">#727</a>
            </td>
            <td>
                <b>
                    add js cc for the private data
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I was testing the private data concept, I noticed that the chaincode is only written with go and java then I decided to take this initiative and implement it with js, the cc was tested with the application I hope that would help js developers understand private data and use nodejs sdk easily.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-29 15:33:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/726" class=".btn">#726</a>
            </td>
            <td>
                <b>
                    Enable engine-strict checks for TypeScript Gateway samples
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Use an .npmrc to enable engine-strict checks so that `npm install` will fail for projects when an incompatible Node version is used, rather than confusing errors about unsupported language features occuring at runtime.

Signed-off-by: Mark S. Lewis <mark_lewis@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-29 13:30:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/725" class=".btn">#725</a>
            </td>
            <td>
                <b>
                    Allow custom peer images for test-network-k8s
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The Hyperledger provided Fabric peer images are only a sample so it would be good to make the k8s test network peer image configurable, for example to include a custom builder

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 14:55:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/724" class=".btn">#724</a>
            </td>
            <td>
                <b>
                    Provide clear guidance for debugging Java chaincode as a service #684
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **READY FOR MERGE** 

(This PR replaces PR #684, which lingered for too long in a DRAFT / review status, spanned multiple approaches, and had merge conflicts with the mainline.)



This PR addresses the need for a simple, clear example that illustrates the use of Chaincode-as-a-Service to build and run Java chaincode on a local development environment.

In addition, the README includes a section that describes how users may employ a Docker loopback interface to connect from a remote Peer binary to a local port on the host OS.  In this manner, chaincode may be run locally while attached to a debugger, with the peer running on a remote pod in Kubernetes.

In the first iteration of this PR, we introduced a new `ccpackage/*` folder to hold descriptive files that would be used to generate the chaincode-as-a-service package, AND help with the deployment to k8s: 

- ccpackage/metadata.json     (defines the package label)
- ccpackage/connection.json  (defines the CC service URL for gRPC access by the peer) 
- ccpackage/ccaas.json           (describes the CC name, used to construct the CC pods in k8s, and CC IMAGE) 

After community review, the PR has been reflected to *remove* the /ccpackage/ folder, opting to dynamically construct the cc package based on conventions and additional CLI arguments.  This has the benefit of applying directly to most (if not all) of the current sample code base, without introducing the crufty "ccaas" deployment descriptors for yet-another-deployment-technique-for-fabric.

A multi-phase Azure pipeline has been included to verify the overall approach for both golang and Java CCaaS asset transfer chaincode samples.

Some additional / loose ends that may warrant future PRs and improvements: 

- Additional testing on the `host.docker.internal` DNS alias is required (e.g. Win, Linux, revs of Docker, etc.) 

-  The doc sets up a flow with three installations of the same chaincode, but does not delete the chaincode between steps.  (How does one _delete_ a chaincode, btw?) 

-  file-based arguments must all be absolute paths. 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 13:10:16 +0000 UTC
    </div>
</div>

