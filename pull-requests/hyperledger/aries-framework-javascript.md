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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/661" class=".btn">#661</a>
            </td>
            <td>
                <b>
                    fix: mediation recipient role for recipient
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Mediation role was being set to `MediationRole.Mediator` instead of `MediationRole.Recipient`. This pr fixes the incorrect role, and adds checks to the methods to make sure we're in the correct context (record.assertRole()).

This is a breaking change, and I'm not sure how to handle this. The record is almost identical between mediator and recipient, so not so sure how to write a migration script for this. As most devices are run inside a specific context (only mediatee or only mediator) the easiest way to update would probably be to update all records to a certain role.

@JamesKEbert heads up on this one. Please let me know how you would like to approach the migration of this. Due to the assertions of the role this is going to cause errors in wallets created before this PR.

Also does some clean up and refactoring

BREAKING CHANGE: for mediation records, the `role` was being set to `MediationRole.Mediator` when acting as a recipient. This is updated to the correct value `MediationRole.Recipient`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-08 11:54:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/660" class=".btn">#660</a>
            </td>
            <td>
                <b>
                    test: minor wallet test changes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Removed '===' prefix to one test name, changed scope of wallet open call to prevent multiple open attempts

Signed-off-by: Niall Shaw <niall.shaw@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-08 11:13:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/657" class=".btn">#657</a>
            </td>
            <td>
                <b>
                    fix(basic-message): assert connection is ready
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim <karim@animo.id>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-03 22:12:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/655" class=".btn">#655</a>
            </td>
            <td>
                <b>
                    feat(core): add OOB record
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There are still some places where it's not so nice because of preserving compatibility with old connection protocol initialization.

I added `protocolCreateRequest` and `protocolProcessRequest` to `ConnectionService` but I want to separate them to`ConnectionProtocol` class later together with other "protocol" methods as `DidExchangeProtocol` class is organized.

We can also add some events around the OOB record, but I also leave it out, for now, to keep it simple.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-03 09:52:14 +0000 UTC
    </div>
</div>

