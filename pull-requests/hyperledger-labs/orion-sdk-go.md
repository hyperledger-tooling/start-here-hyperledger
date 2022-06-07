---
layout: default
title: orion-sdk-go
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/orion-sdk-go
---

# orion-sdk-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/orion-sdk-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-sdk-go/pull/134" class=".btn">#134</a>
            </td>
            <td>
                <b>
                    group reads/writes provenance response by db
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                For GetValuesReadBy() and GetValuesWritten() APIs,
we have to group keys by databases. In the past, there
was a bug at the server which did not group keys by databases.
As now the bug has been fixed at the server side, we are
updating the client APIs in this commit.

Signed-off-by: senthil <cendhu@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-07 04:37:34 +0000 UTC
    </div>
</div>

