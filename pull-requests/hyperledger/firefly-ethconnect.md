---
layout: default
title: firefly-ethconnect
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-ethconnect
---

# firefly-ethconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-ethconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/239" class=".btn">#239</a>
            </td>
            <td>
                <b>
                    [subscriptions] Fix for Validating URLs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We've observed a webhook subscription can be configured with URL which resolves an empty address (without throwing earlier errors):
```
panic: runtime error: index out of range [0] with length 0

goroutine 66 [running]:
github.com/hyperledger/firefly-ethconnect/internal/events.(*eventStream).isAddressUnsafe(0x11c4458, 0x1217e18)
	/kaleido-io/ethconnect/internal/events/eventstream.go:767 +0xd4
```

This is meant to treat this edge case then as an "unsafe address" so Ethconnect does not 1) panic and 2) the URL / hostname will be bubbled up as an error.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-09 12:54:00 +0000 UTC
    </div>
</div>

