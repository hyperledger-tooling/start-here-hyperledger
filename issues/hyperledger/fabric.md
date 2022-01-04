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
                Issue <a href="https://github.com/hyperledger/fabric/issues/3101" class=".btn">3101</a>
            </td>
            <td>
                <b>
                    Unclear empty critical section
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span>
            </td>
            <td>
                https://github.com/hyperledger/fabric/blob/516bc8bab548a484e2e62fee24b0f4fed5bf6873/core/ledger/kvledger/kv_ledger.go#L542-L547

I'm not sure why this is not implemented the same way as other methods in the same file. If a special case is indeed needed here, some comments would be appreciated
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-07 09:16:06 +0000 UTC
    </div>
</div>

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

