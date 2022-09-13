---
layout: default
title: fabric-operations-console
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-operations-console
---

# fabric-operations-console <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-operations-console){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/303" class=".btn">#303</a>
            </td>
            <td>
                <b>
                    Join channel better error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nikhil Modem [nikhil.modem@ibm.com](mailto:nikhil.modem@ibm.com)

#### Type of change

- Bug fix
- Improvement (improvement to code, performance, etc)

#### Description
- When entering a non-existent channel name when adding a peer to a channel, the error message was not caught and formatted well.
- Now checks the grpc status and formats the error message properly 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-13 07:52:53 +0000 UTC
    </div>
</div>

