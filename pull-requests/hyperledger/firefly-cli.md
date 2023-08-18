---
layout: default
title: firefly-cli
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-cli
---

# firefly-cli <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-cli){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/252" class=".btn">#252</a>
            </td>
            <td>
                <b>
                    Fix checking result of queryInstalled()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                the `label` property has the value that is a combination of the chaincode name version. for instance if the chaincode name is `basic`, and version is `v2.0`, then the label is returned as `basic_v2.0`, using the convention `_` to concatenate the two parts:

```
{
	"installed_chaincodes": [
		{
			"package_id": "firefly_1.0:b8e754685421dd03e40251b9ef2dd811e49659453cd489ca7bd27585d9be06b4",
			"label": "firefly_1.0",
			"references": {
				"firefly": {
					"chaincodes": [
						{
							"name": "firefly",
							"version": "1.0"
						}
					]
				}
			}
		},
		{
			"package_id": "basic_v1.0:351b39eb21c6a1d42f65d21398bf747880404c322a8883f2fb61fe1a3bb0d68d",
			"label": "basic_v1.0"
		}
	]
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-17 19:30:39 +0000 UTC
    </div>
</div>

