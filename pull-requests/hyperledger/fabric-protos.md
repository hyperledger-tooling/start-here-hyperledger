---
layout: default
title: fabric-protos
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-protos
---

# fabric-protos

You can clone this repo on <span class="fs-3">[GitHub](https://github.com/hyperledger/fabric-protos){: .btn .mr-4 }</span>


<div class="code-example" markdown="1">
    <table>
        <tr>
            <td>
                PR [#55](https://api.github.com/repos/hyperledger/fabric-protos/pulls/55)
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

