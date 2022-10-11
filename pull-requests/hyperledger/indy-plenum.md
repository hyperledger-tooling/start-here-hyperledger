---
layout: default
title: indy-plenum
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-plenum
---

# indy-plenum <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-plenum){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-plenum/pull/1615" class=".btn">#1615</a>
            </td>
            <td>
                <b>
                    correctly pass ledger_id to the timestamp state storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes an issue during catch-up that caused all timestamps to get written into the domain_ledger ts storage, ignoring the config_ledger.

Signed-off-by: Christian Bormann <ChristianCarl.Bormann@de.bosch.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-11 15:22:38 +0000 UTC
    </div>
</div>

