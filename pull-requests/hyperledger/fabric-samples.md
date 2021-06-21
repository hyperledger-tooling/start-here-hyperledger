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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/451" class=".btn">#451</a>
            </td>
            <td>
                <b>
                    Add process.exit(0) to sample applications
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add process.exit(0) so that sample javascript and typescript
applications exit with success upon completion instead of hanging.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-16 20:23:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/450" class=".btn">#450</a>
            </td>
            <td>
                <b>
                    Test network nano bash - initial commit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Test network Nano bash provides a set of minimal bash scripts
to run a Fabric network on your local machine.
The network is functionally equivalent to the docker-based Test Network,
you can therefore run all the tutorials and samples that target the Test Network.
The Fabric release binaries are utilized rather than using docker containers
to avoid all unnecessary layers. Only the chaincode and chaincode builder
runs in a docker container behind the scenes.
Using the Fabric binaries also makes it simple for Fabric developers
to iteratively and quickly modify Fabric code and test a Fabric network as a user.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-14 11:58:05 +0000 UTC
    </div>
</div>

