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
                PR <a href="https://github.com/hyperledger/cello/pull/468" class=".btn">#468</a>
            </td>
            <td>
                <b>
                    Revert "Fix (security) : Path Traversal Bug"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Revert #443 

Signed-off-by: Yuanmao Zhu [yuanmao@ualberta.ca](mailto:yuanmao@ualberta.ca)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-11 01:25:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/467" class=".btn">#467</a>
            </td>
            <td>
                <b>
                    Revert "Fix : (Security) Migitate Path Traversal Bug"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Reverts hyperledger/cello#455

Signed-off-by: Yuanmao Zhu [yuanmao@ualberta.ca](mailto:yuanmao@ualberta.ca)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-11 00:58:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/466" class=".btn">#466</a>
            </td>
            <td>
                <b>
                    [#issue-460]Switch Docker Compose to v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Switch all Docker Compose commands to v2.
Update setup doc for the version change.

Close #460 

Signed-off-by: xichen1 <xichen.pan@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-07 07:47:17 +0000 UTC
    </div>
</div>

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

