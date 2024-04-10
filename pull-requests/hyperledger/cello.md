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
                PR <a href="https://github.com/hyperledger/cello/pull/608" class=".btn">#608</a>
            </td>
            <td>
                <b>
                    Resolved the permission issue for uploading chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I got this error when uploading the chaincode: ```[Error 13] Permission denied: '/opt/chaincode'```
I resolved this by changing ```FABRIC_CHAINCODE_STORE = "/opt/chaincode"``` to ```FABRIC_CHAINCODE_STORE = "/opt/cello/chaincode"``` in the ```config.py``` file.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-08 02:13:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/607" class=".btn">#607</a>
            </td>
            <td>
                <b>
                    Connected the chaincode's upload function
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Replace the API URL for uploading the chaincode with the updated URL in the front end.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-06 03:48:21 +0000 UTC
    </div>
</div>

