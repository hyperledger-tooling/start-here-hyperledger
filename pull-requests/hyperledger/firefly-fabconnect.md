---
layout: default
title: firefly-fabconnect
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-fabconnect
---

# firefly-fabconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-fabconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-fabconnect/pull/61" class=".btn">#61</a>
            </td>
            <td>
                <b>
                    Improve responses for enroll/register endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These caught me out a bit using the API:
- No feedback on what's wrong with the input if you specify fields that shouldn't be there
- You always get `"name": ""` in the response, because `username` comes from the URL
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-02 21:57:34 +0000 UTC
    </div>
</div>

