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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/475" class=".btn">#475</a>
            </td>
            <td>
                <b>
                    Catch inconsistency if chaincode name does not match
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Problem

I'm testing asset-transfer-basic/chaincode-java.

If I accidently changed rootProject.name in settings.gradle to something else, but still use 

```
 ./network.sh deployCC -ccn basic -ccp ../asset-transfer-basic/chaincode-java -ccl java 
```

for deploying the chaincode, the tool compiles the source code into  ../asset-transfer-basic/chaincode-java/build/install/newName, but deploys the outdated ../asset-transfer-basic/chaincode-java/build/install/basic to the chain.


This behavior is very likely to cause confusions for beginners when they made changes to the source code but didn't see effects on the chain because network.sh is deploying the old copy named basic while the user is changing a project named newName.

## Solution

In this PR, for a Java project, network.sh is revised to remove the install folder to clean up the residues. If the root project name does not match with `-ccn`, users will see an error so that they know there is something wrong.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-24 08:58:19 +0000 UTC
    </div>
</div>

