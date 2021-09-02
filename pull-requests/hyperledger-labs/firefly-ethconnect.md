---
layout: default
title: firefly-ethconnect
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly-ethconnect
---

# firefly-ethconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly-ethconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-ethconnect/pull/143" class=".btn">#143</a>
            </td>
            <td>
                <b>
                    Add synchronization to broadcast when topic list changes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Proposed fix for #142
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-01 22:16:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-ethconnect/pull/141" class=".btn">#141</a>
            </td>
            <td>
                <b>
                    Add fly-transaction param to query transaction details
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Performing a GET to a method endpoint with fly-transaction set to a previously
executed transaction hash will return details on that transaction, including
the decoded input arguments.

I still need to add test coverage, but I wanted to vet that this is a good design.
In particular want to see if we definitely want this on the method REST endpoint,
or if it should be at a higher level somehow.

Note that this branch also includes the enhancement from #140
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-01 19:08:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-ethconnect/pull/140" class=".btn">#140</a>
            </td>
            <td>
                <b>
                    Add getFlyParamBool helper
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-01 14:29:25 +0000 UTC
    </div>
</div>

