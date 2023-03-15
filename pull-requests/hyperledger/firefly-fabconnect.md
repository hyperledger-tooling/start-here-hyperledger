---
layout: default
title: firefly-fabconnect
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-fabconnect
---

# firefly-fabconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-fabconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-fabconnect/pull/108" class=".btn">#108</a>
            </td>
            <td>
                <b>
                    Add golangci config file and fix linter issues
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #106 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-08 22:26:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-fabconnect/pull/107" class=".btn">#107</a>
            </td>
            <td>
                <b>
                    Remove double decoding of event payload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                All events emitted from a subscription are processed based on a configurable "payload type" (bytes, string, JSON). However, for events coming out of the block decoder, they are always coerced to JSON upfront before even being passed to the event decoder. This makes the behavior inconsistent for subscriptions based on a particular chaincode vs. channel-wide subscriptions based on the block decoder.

It seems cleaner to leave the payload as bytes in the block decoder, and to only decode it into string or JSON in the event processor.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-08 19:49:37 +0000 UTC
    </div>
</div>

