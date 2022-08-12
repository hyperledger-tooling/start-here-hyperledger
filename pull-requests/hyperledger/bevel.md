---
layout: default
title: bevel
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/bevel
---

# bevel <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/bevel){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2004" class=".btn">#2004</a>
            </td>
            <td>
                <b>
                    [chore] doorman build fix on kotlin v1.6.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**
- Add fix for kotlin v1.6.0 fix doorman build
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-11 08:26:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2003" class=".btn">#2003</a>
            </td>
            <td>
                <b>
                    [quorum] ansible decoupling raft crypto creation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: manikanta-darsi <manikanta.darsi@accenture.com>

**Changelog**
- Add ansible decoupling raft crypto creation

 

**Reviewed by**
@sownak @suvajit-sarkar @jagpreetsinghsasan 

 

**Linked issue**
#1835 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-10 11:43:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2002" class=".btn">#2002</a>
            </td>
            <td>
                <b>
                    fix(security):Cross Site Scripting Attack (XSS)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Unsanitized input from `req.body.trackingID` flows `trackingID` into `res.send`, where it is used to render an HTML page returned to the user. This may result in a Cross-Site Scripting attack (XSS).

Signed-off-by: Bhaskar Ram <bhaskarvilles@duck.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-07 07:04:21 +0000 UTC
    </div>
</div>

