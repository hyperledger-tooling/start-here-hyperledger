---
layout: default
title: solang
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/552" class=".btn">#552</a>
            </td>
            <td>
                <b>
                    Small fixes
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
        Created At 2021-11-04 22:23:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/550" class=".btn">#550</a>
            </td>
            <td>
                <b>
                    Implement common subexpression elimination
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a draft PR for the common subexpression elimination. Some tests are still missing and there are temporary test files that will be removed when the PR is ready for review.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-04 14:20:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/547" class=".btn">#547</a>
            </td>
            <td>
                <b>
                    Lisbon Release v0.1.9
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added
- Added support for solc import mapppings using `--importmap`
- Added support for Events on Solana
- `msg.data`, `msg.sig`, `msg.value`, `block.number`, and `block.slot` are
  implemented for Solana
- Implemented balance transfers using `.send()` and `.transfer()` on Solana
- Implemented retrieving account balances on Solana
- Verify ed25519 signatures with `signatureVerify()` on Solana
- Added support for Rational numbers
- The address type and value type can changed using `--address-length` and
  `--value-length` command line arguments (for Substrate only)

Changed
- Solana now requires v1.8.1 or later
- On Solana, the return data is now provided in the program log. As a result,
  RPCs are now are now supported.
- On the solang command line, the target must be specified.
- The Solana instruction now includes a 64 bit value field
- Many fixes to the parser and resolver, so solidity compatibility is much
  improved, thanks to [sushi-shi](https://github.com/hyperledger-labs/solang/pulls?q=is%3Apr+author%3Asushi-shi+is%3Aclosed).

Removed
- The Sawtooth Sabre target has been removed.
- The generic target has been removed.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 08:54:11 +0000 UTC
    </div>
</div>

