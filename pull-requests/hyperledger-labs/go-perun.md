---
layout: default
title: go-perun
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/go-perun
---

# go-perun <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/go-perun){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/337" class=".btn">#337</a>
            </td>
            <td>
                <b>
                    Multi ledger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Enables multi-ledger channels.

The following changes are applied:
- Implement special Asset type that contains `LedgerID`.
- Implement multi funder (adjudicator) that contain a set of funders (adjudicators) which are called depending on which assets a channel has.
- Revise watcher: The watcher ensures that in case of a multi-ledger channel, all watched ledgers are kept synchronized.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-29 13:29:18 +0000 UTC
    </div>
</div>

