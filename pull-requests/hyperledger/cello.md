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
                PR <a href="https://github.com/hyperledger/cello/pull/465" class=".btn">#465</a>
            </td>
            <td>
                <b>
                    Improve observability on node and network creating process
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Add logs for `ResourceNotExists` Error.
* Create a command to remove all node containers.
* Tweak `deep-clean` command so then it can clean HLF nodes as well. 

Signed-off-by: Yuanmao Zhu <yuanmao@ualberta.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-04 17:54:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/464" class=".btn">#464</a>
            </td>
            <td>
                <b>
                    Allow users to update their passwords
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Endpoint: POST `/api/v1/users/:user_id/password`
Request Body:
```
{
	"password": "foo2"
}
```

Signed-off-by: Yuanmao Zhu <yuanmao@ualberta.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-04 02:50:18 +0000 UTC
    </div>
</div>

