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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/699" class=".btn">#699</a>
            </td>
            <td>
                <b>
                    Fix Linting: Add in a `-not -path` option to find 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix errors like this that occur from time to time..
```
Linting ./.git/refs/remotes/origin/dependabot/npm_and_yarn/asset-transfer-basic/rest-api-typescript
~/work/1/s/.git/refs/remotes/origin/dependabot/npm_and_yarn/asset-transfer-basic/rest-api-typescript ~/work/1/s
```




Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-01 09:13:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/697" class=".btn">#697</a>
            </td>
            <td>
                <b>
                    Updates the README and documentation guide for the Kube test network's usage of Nginx ingress
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is a documentation update associated with a fix for Issue #685 

The updates associated with this doc update are described in PR #692 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-31 18:21:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/696" class=".btn">#696</a>
            </td>
            <td>
                <b>
                    CORS Enablement
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                After feedback from the community, this PR adds CORS support in, but as an option
to enable.

Along with warnings that the default wildcard origin might not be applicable
in a production use case

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-31 16:55:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/694" class=".btn">#694</a>
            </td>
            <td>
                <b>
                    fix chaincode breakage in asset-transfer-basic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                only broken in main branch, not in release-2.2

Signed-off-by: D <d_kelsey@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 16:36:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/693" class=".btn">#693</a>
            </td>
            <td>
                <b>
                    [release-2.2] Missing await in asset-transfer-basic chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Missing an `await` on the asset-transfer-basic javascript chaincode.

This has been fixed in the main branch but needs to be fixed in the
release-2.2 branch

Signed-off-by: D <d_kelsey@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 14:38:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/692" class=".btn">#692</a>
            </td>
            <td>
                <b>
                    test-network-k8s : Connect to Fabric services via Nginx Ingress - READY FOR MERGE
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
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

