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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/927" class=".btn">#927</a>
            </td>
            <td>
                <b>
                    Avoid explicit import of grpc-js or fabric-protos in TypeScript apps
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Rely on the dependencies of @hyperledger/fabric-gateway making these packages transitively available. Having explicit dependency versions in the application can cause type conflicts due to private member changes in the gRPC Client class across versions.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-10 14:21:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/926" class=".btn">#926</a>
            </td>
            <td>
                <b>
                    Fix an npm dependency error that was breaking the FSAT app compilation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-10 10:30:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/924" class=".btn">#924</a>
            </td>
            <td>
                <b>
                    Move fabric-kube-test-network from Hyperledgendary -> samples
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Configure a test-network on a local Kubernetes cluster, highlighting the enrollment, distribution, and exchange of channel MSP certificates in a production-style, multi-org environment.  The use of CA, ingress, and Fabric CLIs is illustrated through simplistic bash scripting and clear definitions of the org / MSP context.

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-09 17:33:48 +0000 UTC
    </div>
</div>

