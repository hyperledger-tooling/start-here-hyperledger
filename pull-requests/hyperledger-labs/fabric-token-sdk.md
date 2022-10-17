---
layout: default
title: fabric-token-sdk
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-token-sdk
---

# fabric-token-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-token-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/408" class=".btn">#408</a>
            </td>
            <td>
                <b>
                    Move inactive maintainers to emeritus status
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The TSC approved a requirement that maintainers
that have not been active in over three to six
months be move to emeritus status.

These maintainers have not been active in over
one year.

https://github.com/hyperledger/toc/issues/32
Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-16 18:40:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/407" class=".btn">#407</a>
            </td>
            <td>
                <b>
                    Export `SetStatus` function on OnwerDBs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                Signed-off-by: Angelo De Caro <adc@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-12 06:24:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/406" class=".btn">#406</a>
            </td>
            <td>
                <b>
                    enhancements/bug fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">enhancement</span>
            </td>
            <td>
                This PR brings in the following enhancements/bug fixes:
- CI: expand `fungible` and `inteop` tests to run them in parallel
- Fungible Tests: Introduce a view that check the consistency of the transaction dbs with the ledger and the vault
- Interop Tests: Introduce balance view to check the amount of unspent tokens, locked tokens, and locked by expired tokens.
- Wallets: Introduce Iterators
- Owner and Audit DB (derivates of the TTXDB): Restore status listeners when rebooting
- HTLC Wallet: functions to return locked tokens, locked and expired tokens (with support to iterators)
- TransactionInfoProvider: to load metadata of a transaction
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-11 13:20:41 +0000 UTC
    </div>
</div>

