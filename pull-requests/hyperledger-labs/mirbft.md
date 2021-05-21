---
layout: default
title: mirbft
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/mirbft
---

# mirbft <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/mirbft){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/mirbft/pull/24" class=".btn">#24</a>
            </td>
            <td>
                <b>
                    Make Node orchestrate processing Actions / Events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is the first step towards cleaning up the top-level structure.
The Node now mostly deals with modules and orchestrates the flow of
Actions and events between them.

The interface for submitting client request is simplified and becomes
a single method `SubmitRequest` of the Node.

Signed-off-by: Matej Pavlovic <mpa@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 21:02:53 +0000 UTC
    </div>
</div>

