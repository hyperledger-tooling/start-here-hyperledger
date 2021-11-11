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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/535" class=".btn">#535</a>
            </td>
            <td>
                <b>
                    Retire dormant maintainers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Several fabric-samples maintainers have moved on to other projects.
See maintainer policies at
https://hyperledger-fabric.readthedocs.io/en/latest/CONTRIBUTING.html#becoming-a-maintainer

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-10 16:13:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/534" class=".btn">#534</a>
            </td>
            <td>
                <b>
                    Update node version in CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Several Fabric projects have updated their supported node versions and 16.x is the active LTS version

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-10 16:07:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/533" class=".btn">#533</a>
            </td>
            <td>
                <b>
                    Address Issue #511 with docs and better error handling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The chaincode installation script had an error that was masking the lack of `shasum` on an end-user's machine.  This made it really hard to pick out the root cause of a downstream error.

This PR addresses the first part / root cause of Issue #511, which can be closed after this PR lands. 

This snippet will not crash with error.  $? is set to the return value of the `local` command.  
```
set -o errexit 

local foo=$(broken-command | tr -s ' ' | cut -d ' ' -f 1)
```

This snippet will error when `broken-command` terminates with a nonzero exit code: 
```
set -o errexit 

foo=$(broken-command | ...)
```


Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-10 15:20:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/532" class=".btn">#532</a>
            </td>
            <td>
                <b>
                    Setup basic HA features for the Peers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add a new label to each peer to mark which org it is in
- Create new service per org, that matches this label - so the service can pick from one of multiple pods
- Update the kubeproxy to give more choice of ha stratergies
- Update the application configmaps and samples to refer to this new service rather than specific peers

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-10 10:57:57 +0000 UTC
    </div>
</div>

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

