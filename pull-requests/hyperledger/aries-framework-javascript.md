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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/872" class=".btn">#872</a>
            </td>
            <td>
                <b>
                    docs: accessing rust logs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Niall Shaw <niall.shaw@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 12:09:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/871" class=".btn">#871</a>
            </td>
            <td>
                <b>
                    docs: update developer readme
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                adds some hints for debugging running tests

Signed-off-by: Moriarty <moritz@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 10:24:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/870" class=".btn">#870</a>
            </td>
            <td>
                <b>
                    feat: delete associated didCommMessages when deleting credential records
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Moriarty <moritz@animo.id>

closes #728 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 10:15:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/869" class=".btn">#869</a>
            </td>
            <td>
                <b>
                    Mjrmergemain ppv2
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
        Created At 2022-06-16 07:42:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/864" class=".btn">#864</a>
            </td>
            <td>
                <b>
                    fix(credentials): store revocation identifiers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #863 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 13:37:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/862" class=".btn">#862</a>
            </td>
            <td>
                <b>
                    fix(credentials): indy cred attachment format
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 10:43:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/861" class=".btn">#861</a>
            </td>
            <td>
                <b>
                    fix(credentials): parse and validate preview @type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 10:25:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/857" class=".btn">#857</a>
            </td>
            <td>
                <b>
                    fix(node): only send 500 if no headers sent yet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If an error occurred after a message has been sent in response in the http inbound transport it would error out because we can't return a response twice in http. This just checks if the response is already sent
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 08:56:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/856" class=".btn">#856</a>
            </td>
            <td>
                <b>
                    fix(credentials): use interface in module api
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                My previous PR to generalize the crdentials module undid some of the changes to only allow interfaces.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 08:45:57 +0000 UTC
    </div>
</div>

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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/848" class=".btn">#848</a>
            </td>
            <td>
                <b>
                    fix(proofs): allow duplicates in proof attributes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a partial fix for https://github.com/hyperledger/aries-framework-javascript/issues/837
The check is limited to duplicates between predicates and attributes only. Duplicit attributes should be allowed as they don't cause any error during proof creation.
Still todo: Either
* parse and validate based on `restrictions`, whether the items collide or not
or
* completely rethink the check and validate only at the point of `ProofsModule.acceptRequest` (which is the actual problem)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-10 13:58:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/847" class=".btn">#847</a>
            </td>
            <td>
                <b>
                    docs(samples): fix extension module sample
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-10 10:51:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/846" class=".btn">#846</a>
            </td>
            <td>
                <b>
                    docs: remove signed off by lines from changelog
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-10 09:36:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/845" class=".btn">#845</a>
            </td>
            <td>
                <b>
                    refactor: adds custom rxjs operator to filter record events by record type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds custom rxjs operator to filter record events by record type. To be used in hooks extension.

Signed-off-by: Akiff Manji <akiff.manji@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-09 21:52:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/844" class=".btn">#844</a>
            </td>
            <td>
                <b>
                    chore(migration): add credentials migration script
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds migration script for updating credential records to 0.2.0 structure. 

Fixes #738
Supersedes #843 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-09 20:56:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/842" class=".btn">#842</a>
            </td>
            <td>
                <b>
                    feat(core): generic repository events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #723 

Added generic `RecordSavedEvent`, `RecordUpdatedEvent`, and `RecordDeletedEvent` emitted from `Repository`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-09 15:03:31 +0000 UTC
    </div>
</div>

