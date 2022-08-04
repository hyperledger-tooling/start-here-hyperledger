---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/971" class=".btn">#971</a>
            </td>
            <td>
                <b>
                    feat(ledger): Add ledgerService interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: DaevMithran <daevmithran1999@gmail.com>

Question
- instead of indyLedgers. Can we change it to ledgers : { indy: [ ], cosmos: [ ] } .etc
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-29 14:07:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/967" class=".btn">#967</a>
            </td>
            <td>
                <b>
                    feat(ledger): handle REQNACK response for write request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I'm not sure if the check for REQNACK response was omitted in the write request method on purpose, but `registerSchema` is throwing a confusing error.

Previously:
```
TypeError: Cannot read property 'txnMetadata' of undefined
```

After the update:
```
Ledger 'pool-localhost' rejected write transaction request: client request invalid: could not authenticate, verkey for 9gFCquotxSS7ctKG1GJatU cannot be found
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-28 07:46:46 +0000 UTC
    </div>
</div>

