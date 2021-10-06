---
layout: default
title: fabric-protos
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-protos
---

# fabric-protos <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-protos){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/66" class=".btn">#66</a>
            </td>
            <td>
                <b>
                    Change EndpointError to ErrorDetail
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This name gets surfaced in the SDKs,  not as an error itself, but as extra information within an error/exception.  The name, ending in Error, is misleading in Java and Node.  This commit changes it to more appropriate name.

contributes to https://github.com/hyperledger/fabric/issues/2971

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-06 14:33:28 +0000 UTC
    </div>
</div>

