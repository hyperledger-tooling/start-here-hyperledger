---
layout: default
title: fabric-protos
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-protos
---

# fabric-protos <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-protos){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/79" class=".btn">#79</a>
            </td>
            <td>
                <b>
                    Add binding generation for node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds a node module template project and associate code generation

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-21 18:18:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/78" class=".btn">#78</a>
            </td>
            <td>
                <b>
                    Node bindings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add a TypeScript project in bindings/node that can automagically build an npm package containing compiled protobuf and gRPC stubs, along with module indexes to correctly expose the generated stubs from the package.

The change does not implement the packaging (npm pack) or publish of the npm package to the npm registry, which will be delivered later.

The produced npm package has been tested with the Fabric Gateway client API, and passes all unit and scenario tests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-19 17:03:11 +0000 UTC
    </div>
</div>

