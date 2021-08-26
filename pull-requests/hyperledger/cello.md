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
                PR <a href="https://github.com/hyperledger/cello/pull/304" class=".btn">#304</a>
            </td>
            <td>
                <b>
                    [#issue-302]add fabric cmdline lib
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The command line lib library is added to help cello use the binary file of fabric to execute channel created and other methods to operate the fabric network.
This issue will build the channel class and implement the methods of creating and querying channels

Signed-off-by: tianxuanhong <523713078@qq.com>

Close #302 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-26 01:07:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/303" class=".btn">#303</a>
            </td>
            <td>
                <b>
                    fix login
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                *The user name and email should be consistent; Role setting admin

Signed-off-by: XuHugo <xq-310@163.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-25 16:05:06 +0000 UTC
    </div>
</div>

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

