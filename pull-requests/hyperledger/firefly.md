---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/290" class=".btn">#290</a>
            </td>
            <td>
                <b>
                    Add topic+tag index to messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The intention of the topics field, is that you can create a stream of data that is grouped on a particular ordered business context, and the tag sub-classifies messages within that.

This means that querying by topic and tag is a primary use case, for which index(es) should exist.

This PR proposes a single combined index, on topic then tag, as I believe that's the most likely combination of filter across use cases.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 12:03:27 +0000 UTC
    </div>
</div>

