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
                PR <a href="https://github.com/hyperledger-labs/firefly-ethconnect/pull/148" class=".btn">#148</a>
            </td>
            <td>
                <b>
                    Use mockery for contractregistry and sarama mocks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This makes mocks a lot clearer and more explicit about the expected calls.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 14:35:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-ethconnect/pull/147" class=".btn">#147</a>
            </td>
            <td>
                <b>
                    Allow including method inputs with subscribed events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Passing {"inputs": true} when initializing an event stream will cause each
event to include two new fields - inputMethod will be the name of the method
that emitted the event, and inputArgs will be a map of the args passed in
when the method was called.

This can be reviewed in parallel with #141, although they share one commit
containing some generic helpers for decoding transaction info.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-13 16:17:53 +0000 UTC
    </div>
</div>

