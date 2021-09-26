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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/500" class=".btn">#500</a>
            </td>
            <td>
                <b>
                    Remove unused targets
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
        Created At 2021-09-26 08:15:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/499" class=".btn">#499</a>
            </td>
            <td>
                <b>
                    Fix clippy warning on Windows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-25 10:27:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/498" class=".btn">#498</a>
            </td>
            <td>
                <b>
                    Fix resolving relative paths on Windows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                solang ./foo/bar.sol would always fail on Windows

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-25 08:25:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/496" class=".btn">#496</a>
            </td>
            <td>
                <b>
                    Add import mapping to match solc's mapping functionality
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-23 19:20:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/495" class=".btn">#495</a>
            </td>
            <td>
                <b>
                    fix: solana mechanism for return has changed yet again
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                unless am wrong:

```
[
  'Program 3vtWFA1tozq1mfZAMJfAVtQVvRkTjeio8rkyRFzRuTP5 invoke [1]',
  'Program 3vtWFA1tozq1mfZAMJfAVtQVvRkTjeio8rkyRFzRuTP5 consumed 1020 of 200000 compute units',
  'Program return: 3vtWFA1tozq1mfZAMJfAVtQVvRkTjeio8rkyRFzRuTP5 CMN5oAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAgAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABNEbyB0aGUgcmV2ZXJ0IHRoaW5nAAAAAAAAAAAAAAAAAA==',
  'Program 3vtWFA1tozq1mfZAMJfAVtQVvRkTjeio8rkyRFzRuTP5 failed: custom program error: 0x0'
]
```

tested on latest `solanalabs/solana:edge` image.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-22 15:48:09 +0000 UTC
    </div>
</div>

