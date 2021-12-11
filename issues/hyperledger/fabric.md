---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/fabric/issues/3014" class=".btn">3014</a>
            </td>
            <td>
                <b>
                    Support docker registry authentication when pulling chaincode builder images and chaincode runtime images
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span>
            </td>
            <td>
                When deploying fabric in enterprise's intranet (without the ability to access internet),  users maybe upload chaincode builder images and chaincode runtime images to a private docker registry which requires authentication when pulling images.
I think fabric can support this scenario by adding configuration in `chaincode` section of core.yaml, such as:
```yaml
chaincode:
    registry:
        authentication:
              user: ****
              password: ****
```

and then uses this configuration for authentication when invoking docker's api .

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 09:19:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/fabric/issues/2916" class=".btn">2916</a>
            </td>
            <td>
                <b>
                    Add Java example to chaincode as external service documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span><span class="chip">good first issue</span>
            </td>
            <td>
                Per stackoverflow post https://stackoverflow.com/questions/69115892/hyperledger-fabric-java-chaincode-timeout-expired-while-starting-chaincode  , it appears Java chaincode is missing from chaincode as an external service doc topic:
https://hyperledger-fabric.readthedocs.io/en/latest/cc_service.html#writing-chaincode-to-run-as-an-external-service

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 15:56:40 +0000 UTC
    </div>
</div>

