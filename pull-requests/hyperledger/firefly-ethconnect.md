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
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/199" class=".btn">#199</a>
            </td>
            <td>
                <b>
                    Protect misconfiguring catchupModeBlockGap < catchupModePageSize and fix catchup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See #198 for the 🤕 behavior you can get if we don't protect against this.

The logic here has an implicit assumption of this rule, so that when we read a page it's never going to extend past the `blockNumber` of the header of the chain at the point we query.

Otherwise, we think:
- Gap to head 1234 is > 250 - so we're in catchup
- Read 5000 (page size) - cool we've read 5000 blocks ... but actually there were only 1234 to read!!!
- ok, now we're not in catchup any more - start reading from where we left off - but that's now skipped a whole bunch of blocks.

https://github.com/hyperledger/firefly-ethconnect/blob/f6c7fe5499d111a25d2301b84efdb8a13db988e2/internal/events/subscription.go#L223-L248
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-04 04:29:11 +0000 UTC
    </div>
</div>

