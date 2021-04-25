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
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/55" class=".btn">#55</a>
            </td>
            <td>
                <b>
                    FABGW-19: Secure Gateway CommitStatus service
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Include calling identity in CommitStatusRequest
- SignedCommitStatusRequest wraps a serialized CommitStatusRequest and digital signature
- CommitStatus service received a SignedCommitStatusRequest instead of CommitStatusRequest

Allows the server to:

- Ensure the request message was created by the expected client identity by verifying the signature
- Check that the calling identity has read permission for the channel
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-22 13:05:55 +0000 UTC
    </div>
</div>

