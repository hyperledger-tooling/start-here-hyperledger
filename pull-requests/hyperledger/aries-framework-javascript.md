---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1037" class=".btn">#1037</a>
            </td>
            <td>
                <b>
                    fix(oob): allow encoding in content type header
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Allows content type header to have encoding in the value. To not break implementations that only use `application/json` it just checks wether the header value starts with `application/json`

The oob RFC describes the content type header with encoding in it: 

> The sender MAY include a Content-Type header specifying application/json; charset=utf-8, and in the case where the agent included an Accept header for the application/json MIME type, the sender MUST include the header. If so, the sender MUST return the invitation in JSON format in the response body with a status_code of 200.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-25 13:44:32 +0000 UTC
    </div>
</div>

