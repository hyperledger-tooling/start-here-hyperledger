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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/531" class=".btn">#531</a>
            </td>
            <td>
                <b>
                    Update application-gateway-typescript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The fabric-gateway node module has been renamed to @hyperledger/fabric-gateway

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 12:21:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/529" class=".btn">#529</a>
            </td>
            <td>
                <b>
                    Fix type error when using the latest sort-keys-recursive
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Descriptions
The latest version (2.1.2) of sort-keys-recursive adds TypeScript typing, which includes export default function.
This change has caused the TS2349 type error.

This patch modifies the import form in assetTransfer.ts to fix the error.

## Related information

The example of error logs is:
```javascript
github.com/fabric-samples/asset-transfer-basic/chaincode-typescript (main *)$ npm run build

> asset-transfer-basic@1.0.0 build /home/ubuntu/workspace/src/github.com/fabric-samples/asset-transfer-basic/chaincode-typescript
> tsc

src/assetTransfer.ts:66:69 - error TS2349: This expression is not callable.
  Type 'typeof import("sort-keys-recursive")' has no call signatures.

66             await ctx.stub.putState(asset.ID, Buffer.from(stringify(sortKeysRecursive(asset))));
                                                                       ~~~~~~~~~~~~~~~~~

src/assetTransfer.ts:87:59 - error TS2349: This expression is not callable.
  Type 'typeof import("sort-keys-recursive")' has no call signatures.

87         await ctx.stub.putState(id, Buffer.from(stringify(sortKeysRecursive(asset))));
                                                             ~~~~~~~~~~~~~~~~~

src/assetTransfer.ts:117:60 - error TS2349: This expression is not callable.
  Type 'typeof import("sort-keys-recursive")' has no call signatures.

117         return ctx.stub.putState(id, Buffer.from(stringify(sortKeysRecursive(updatedAsset))));
                                                               ~~~~~~~~~~~~~~~~~

src/assetTransfer.ts:145:59 - error TS2349: This expression is not callable.
  Type 'typeof import("sort-keys-recursive")' has no call signatures.

145         await ctx.stub.putState(id, Buffer.from(stringify(sortKeysRecursive(asset))));
                                                              ~~~~~~~~~~~~~~~~~


Found 4 errors.

npm ERR! code ELIFECYCLE
npm ERR! errno 2
npm ERR! asset-transfer-basic@1.0.0 build: `tsc`
npm ERR! Exit status 2
npm ERR! 
npm ERR! Failed at the asset-transfer-basic@1.0.0 build script.
npm ERR! This is probably not a problem with npm. There is likely additional logging output above.

npm ERR! A complete log of this run can be found in:
npm ERR!     /home/ubuntu/.npm/_logs/2021-11-05T06_16_41_781Z-debug.log
```

Related update is:
https://github.com/Kikobeats/sort-keys-recursive/commit/41858bd2745ead6fcb38e281cc7c4eb00705c523

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-05 07:21:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/528" class=".btn">#528</a>
            </td>
            <td>
                <b>
                    Add an option to stage docker images locally to KIND
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR addresses a compromise for development workflows requiring different patterns for loading images into the KIND / kubernetes cluster. 

- For casual / default usage, the docker images are loaded from the public container registries (docker.io and ghcr.io)

- For developers with network issues connecting to public registries, this PR allows for an offline "pull" and stage to the KIND control plane: 
```
export TEST_NETWORK_STAGE_DOCKER_IMAGES=true
./network kind     # << this will pull from the public repos, and run kind load docker-image ...  

./network up 
```

- For test/development of the CI latest build outputs, the container registry and revision can be overridden: 
```
export TEST_NETWORK_FABRIC_VERSION=amd64-latest 
export TEST_NETWORK_FABRIC_CA_VERSION=amd64-latest 
export TEST_NETWORK_FABRIC_CONTAINER_REGISTRY=hyperledger-fabric.jfrog.io

./network up 
```

- For active development of core Fabric images (e.g. peer, orderer), the KIND control plane can be directly loaded with local builds: 
```
make docker # (in fabric) 

export TEST_NETWORK_FABRIC_VERSION=2.4.0 

./network load-images 
./network up 
``` 


@mbwhite and @SamYuan1990 can you please give this PR a test run to double-check that it meets your target use cases?   Matthew I had some difficulty testing out PR #507 and the `candidate-use-builtin-ccs-builder` branch with the mainline network scripts.  I think this is a better fit for that workflow. 


Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 20:57:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/527" class=".btn">#527</a>
            </td>
            <td>
                <b>
                    Use built-in Peer chaincode-as-a-server builder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Using the variant of the peer's docker container from https://github.com/hyperledger/fabric/pull/2990  this PR adapts the K8S deployment to use this inbuilt chaincode builder.

- creates two deployments of the chaincode for each peer
- uses the builders ability to template the fields in the connection.json

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 10:08:54 +0000 UTC
    </div>
</div>

