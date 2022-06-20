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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/855" class=".btn">#855</a>
            </td>
            <td>
                <b>
                    fix(credentials): proposal preview attribute 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In the v2 preview `credential_proposal` should be `credential_preview`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 08:06:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/849" class=".btn">#849</a>
            </td>
            <td>
                <b>
                    feat(indy): add choice for taa mechanism
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                todos:
* tests
* ensure this is complete and correct

Signed-off-by: Moriarty <moritz@animo.id>

BREAKING CHANGE: the transaction author agreement acceptance mechanism was previously automatically the first acceptance mechanism from the acceptance mechanism list. With this addition, the framework never automatically selects the acceptance mechanism anymore and it needs to be specified in the `transactionAuthorAgreement` in the `indyLedgers` agent config array.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-13 11:26:11 +0000 UTC
    </div>
</div>

