---
layout: default
title: aries-endorser-service
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-endorser-service
---

# aries-endorser-service <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-endorser-service){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-endorser-service/pull/34" class=".btn">#34</a>
            </td>
            <td>
                <b>
                    Granular configuration of auto-endorsement 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This pull request resolves #32

The endorser service supports auto-endorsing specific types of transaction, however it is not designed to support more fine-grained control mechanisms.

Here we add a new `/allow/` endpoint which can add to, delete from, and get a list of transactions which will be auto-endorsed. There is a list for:
- publishing DIDs
- publishing schema definitions
- publishing credential definitions

When any of these lists are updated all pending transactions will be compared and if a match between one of these lists and the pending transactions is found the transaction will be endorsed.

![2023-09-27_16-39-56](https://github.com/hyperledger/aries-endorser-service/assets/34443260/871415b1-ac51-4758-9abc-d19c61b46dd5)

In addition, a new configuration setting `ENDORSER_REJECT_BY_DEFAULT` has been introduced to control whether transactions that do not match any of the allow lists are rejected, or left pending by default


Currently remaining work to be done:
- [ ] Document how the new allow lists work
- [ ] Integrate RevRegEntry and RevRegDef entries in the creddef configuration
- [ ] Add integration and unit tests
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-28 00:40:58 +0000 UTC
    </div>
</div>

