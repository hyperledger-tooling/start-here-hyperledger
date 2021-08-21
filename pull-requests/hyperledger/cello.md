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
                PR <a href="https://github.com/hyperledger/cello/pull/301" class=".btn">#301</a>
            </td>
            <td>
                <b>
                    [#issue-300]Modify registration, login, and user roles
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. When registering a user, change the user name to email
2. When logging in, change the user name to email and remove the organization name
3. Modify the user role judgment and only retain two roles: "admin" and "member"

Signed-off-by: fengyang_sy <fengyang.09186@h3c.com>
Close #300 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-21 02:17:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/299" class=".btn">#299</a>
            </td>
            <td>
                <b>
                    Optimize network module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                *Optimize return format.
*Optimize list, create function.

Signed-off-by: XuHugo <xq-310@163.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-20 16:19:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/298" class=".btn">#298</a>
            </td>
            <td>
                <b>
                    [#issue-297]Modify page display and mock data
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1.Modify the organization's mock according to the new interface
2.Modify the method of extracting organization data from agent page according to the new interface
3.Modify the organization page and extract the organization list according to the returned information of the new interface
4.Modify the user's mock login interface address

Signed-off-by: fengyang_sy <fengyang.09186@h3c.com>
fix #issue-297
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-20 13:34:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/296" class=".btn">#296</a>
            </td>
            <td>
                <b>
                    Fix #290 Can not get JWT token from obtain_jwt_token view
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Solved by using email as the login usernames, and add an email field to
registration API endpoint.

Close #290

Signed-off-by: Yuanmao Zhu <zhu.yuanmao18@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-18 02:18:51 +0000 UTC
    </div>
</div>

