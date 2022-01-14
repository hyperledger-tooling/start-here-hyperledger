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
                PR <a href="https://github.com/hyperledger/cello/pull/380" class=".btn">#380</a>
            </td>
            <td>
                <b>
                    [#issue-379] realize the chain code package function
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Realize the chain code package function. In the post request, you need to carry the zip package and MD5 value. After decompressing it to the specified path, call the peer binary tool to perform the package operation

Close #379

Signed-off-by: tianxuanhong1 <523713078@qq.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-11 11:57:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/378" class=".btn">#378</a>
            </td>
            <td>
                <b>
                    [#issue-374]network create failed: The front-end parameters are incon…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …sistent with the back-end parameters

front parames: consensus, db,name,type,version
but backend needs: name, consensus,database
Close #374 
Signed-off-by: fengyang_sy <fengyang.09186@h3c.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-11 02:14:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/375" class=".btn">#375</a>
            </td>
            <td>
                <b>
                    [#issue-373]Modify front-end channel module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1.Modify front end channel list page

2.Modify the response judgment to create channel request

Close #373 

Signed-off-by: fengyang_sy fengyang.09186@h3c.com
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-08 08:40:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/371" class=".btn">#371</a>
            </td>
            <td>
                <b>
                    [#issue-370]Modify front-end login module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Modify the front-end code according to the response information of the new login interface and the verification token interface

Close #370 

Signed-off-by: fengyang_sy <fengyang.09186@h3c.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-08 08:19:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/369" class=".btn">#369</a>
            </td>
            <td>
                <b>
                    [#issue-368] chaincode files upload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The interface of chain code upload is added. Temporarily save the chain code in the / opt / chaincode / {MD5} directory. In the future, consider making the package function in an interface?

and modified dashboard dockerfile of base image node version from 14.2.0 to 14.13.1 , to resolve the dashboard build error: 
error strip-css-comments@5.0.0: The engine "node" is incompatible with this module. Expected version "^12.20.0 || ^14.13.1 || >=16.0.0". Got "14.2.0"
error Found incompatible module.


Close #368

Signed-off-by: tianxuanhong1 <523713078@qq.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-08 00:55:07 +0000 UTC
    </div>
</div>

