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
                PR <a href="https://github.com/hyperledger/cello/pull/504" class=".btn">#504</a>
            </td>
            <td>
                <b>
                    Add token and user feilds to the response in token-verify endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Example response 
```
{
    "data": {
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiZXhwIjoxNjcwNjk5Njg0LCJpYXQiOjE2NzA2OTkzODQsImp0aSI6ImY1ZDc1MjUyMWJjNzQyMTVhOTQ5OTY0NWRhOTY3MmE0IiwidXNlcl9pZCI6ImEzODc4MDQwLTQ2MDItNDdlMy05YWE1LTYyYjI2OWMzN2VkOCJ9.W3dsf987YfX6c6yhaVssQF6MHxoBc6vF4HCNn8nS3Rw",
        "user": {
            "id": "a3878040-4602-47e3-9aa5-62b269c37ed8",
            "username": "foo2@email.com",
            "role": "admin",
            "organization": {
                "id": "142fb71a-ed52-4972-94ff-9c6b87f729d1",
                "name": "org2.cello.com"
            }
        }
    },
    "msg": null,
    "status": "successful"
}
```




Signed-off-by: Yuanmao Zhu <yuanmao@ualberta.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-10 19:11:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/503" class=".btn">#503</a>
            </td>
            <td>
                <b>
                    Bump up python version to 3.8 in github workflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Bump up python version to 3.8 in github workflow
* Add token-verify endpoint back
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-10 01:48:55 +0000 UTC
    </div>
</div>

