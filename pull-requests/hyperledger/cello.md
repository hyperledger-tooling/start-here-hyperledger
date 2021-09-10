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
                PR <a href="https://github.com/hyperledger/cello/pull/328" class=".btn">#328</a>
            </td>
            <td>
                <b>
                    Implemented channel creating operation with peer channel cli.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Create a channel for the current user, and then add all peer nodes from
the org to the channel. Finally, set the first peer node as the anchor
peer.

Signed-off-by: Yuanmao Zhu <zhu.yuanmao18@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-10 05:09:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/327" class=".btn">#327</a>
            </td>
            <td>
                <b>
                    [#issue-326] cmdlinelib feature of approveformyorg && queryapproved f…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …unctions

implement the cmdlinelib feature of approveformyorg && queryapproved functions

Close #issue-326

Signed-off-by: tianxuanhong <523713078@qq.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 00:41:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/325" class=".btn">#325</a>
            </td>
            <td>
                <b>
                    create channel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                *first,update configtx.yaml.
*then,create channel.tx.

Signed-off-by: XuHugo <xq-310@163.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-08 15:04:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/324" class=".btn">#324</a>
            </td>
            <td>
                <b>
                    [#issue-319] There is a risk of obtaining expired information
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If the file has already been created. Then an exception occurs, at which point the file is not deleted, and the next time the function is called, the information continues to be written to the file, causing the user to get an exception.

Perhaps using files is not a good method;

Close #issue-319

Signed-off-by: zhaoshihong <523713078@qq.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-06 12:22:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/323" class=".btn">#323</a>
            </td>
            <td>
                <b>
                    [#issue-322]Modify the agent,network and node list to display abnorma…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …l problems

Modify the agent,network and node list to display abnormal problems

Signed-off-by: fengyang_sy <fengyang.09186@h3c.com>

Close #322 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-05 00:44:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/321" class=".btn">#321</a>
            </td>
            <td>
                <b>
                    [#issue-320] lifecycle_query_installed&lifecycle_get_installed_package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                lifecycle_query_installed will get all chaincode information installed in peer. lifecycle_get_installed_package will get all chaincode files installed in peer,
it's input is packid_id.

Close #issue-320

Signed-off-by: zhaoshihong<523713078@qq.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-04 08:52:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/318" class=".btn">#318</a>
            </td>
            <td>
                <b>
                    [#issue-317] cmdLineLib of chaincode operation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Construct the chaincode class and implement the methods of chaincode package and chaincode install

Close #issue-317

Signed-off-by: zhaoshihong <523713078@qq.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-04 06:58:58 +0000 UTC
    </div>
</div>

