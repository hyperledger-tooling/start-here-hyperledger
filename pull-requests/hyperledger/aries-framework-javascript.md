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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1544" class=".btn">#1544</a>
            </td>
            <td>
                <b>
                    fix: add OOB id to auto-created connection
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When a connection is auto-created after receiving first DIDComm v2 message, the OOB record that generated the invitation is not associated to it. So it becomes difficult to find it it afterwards. 

This happened to Faber in the demo, and may happen to you as well!
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-14 23:10:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1543" class=".btn">#1543</a>
            </td>
            <td>
                <b>
                    test: DidCommV2 compatibility with Aries GO
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added test and note regarding the compatibility of DidCommV2 message packing with AFGo.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-14 06:16:10 +0000 UTC
    </div>
</div>

