---
layout: default
title: cello
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cello
---

# cello <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cello){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/490" class=".btn">#490</a>
            </td>
            <td>
                <b>
                    Add a new org to the channel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Allow users to append an MSP config to the channel config. Currently, we upload the MSP data via the request body, and will implement uploading via file format. 

Endpoint: 

`PUT  http://127.0.0.1:8080/api/v1/channels/:channel_id` 
Request body:
```
{
    "msp_id": "<Org MSP ID>",
    "config": {
      ...msp_config
    }
 
}
```

Signed-off-by: Yuanmao Zhu [yuanmao@ualberta.ca](mailto:yuanmao@ualberta.ca)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-23 22:19:51 +0000 UTC
    </div>
</div>

