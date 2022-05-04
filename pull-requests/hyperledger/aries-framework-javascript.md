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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/736" class=".btn">#736</a>
            </td>
            <td>
                <b>
                    fix: mediation record checks for pickup v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds checks in the mediation recipient service for mediation record state and role. Also splits up the sending of the status request message to be more in line with separation of service/module in the rest of the framework. 

Finally, this updates the processing of the message to be using the event emitter. We also use this approach for pickup v1 and it was causing issues in the oob branch due to circular dependencies.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-02 22:03:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/735" class=".btn">#735</a>
            </td>
            <td>
                <b>
                    ci: add node 18 to test matrix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds node v18 to the test matrix. Once this is merged we can look at removing support for node 12 (https://github.com/hyperledger/aries-framework-javascript/issues/734).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-02 12:07:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/733" class=".btn">#733</a>
            </td>
            <td>
                <b>
                    fix: always encode keys according to RFCs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">OOB - DidExchange</span>
            </td>
            <td>
                Keys were not encoded in services according to the RFCs. This is quite complex TBH as there's three different service types with three different encodings.... 

The biggest problem was the encoding of the `did-communciation` used in did documents, those should use did references local to the did, not did:key dids and not raw public keys. 

This PR updates a lot of places to pass around keys so we have a consistent format to pass around keys in the framework, which made it a lot easier to work with the different formats (we never know which of the three encodings recipientKey of type string means).

A lot more changes than I initially anticipated, but this is an important fix to adhere to the RFCs.

Dependant on #717. We can merge that PR first or merge this PR into #717 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-01 16:15:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/732" class=".btn">#732</a>
            </td>
            <td>
                <b>
                    refactor: unify connection record state and role
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">OOB - DidExchange</span>
            </td>
            <td>
                Unify connection record state and role by only levering did exchange states and roles. The did exchange states are more explicit so I thought we use that. Also added an `rfc0160State` getter to the connection record for convenience.

Can be merged into #717 or merged into main after that PR is merged

Migration script is addressed in #731 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-30 19:36:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/731" class=".btn">#731</a>
            </td>
            <td>
                <b>
                    feat: 0.2.0 connection migration script
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">OOB - DidExchange</span>
            </td>
            <td>
                Adds migration script for the breaking changes introduced in 0.2.0 with the addition of out of band protocol and `did:peer` dids.

This should be merged after #717 is merged ( I will update the target to main then ), as it depends on those Changes. Keeping it as separate PR to not make the PR  bigger.

I think there's some issues with the transformation of the invitations and did documents that we should address, but that can be address separately. This PR just leans on the methods for transformation already provided in PR #717

There's one FIXME left because I wasn't 100% sure on how it worked. @jakubkoci maybe you can help me answer. When creating an oob record that is reusable, is it correct that all connections will have the same oob id? If that's true I need to make some small tweaks to the script.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-30 14:30:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/726" class=".btn">#726</a>
            </td>
            <td>
                <b>
                    fix: optional fields in did document
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">OOB - DidExchange</span>
            </td>
            <td>
                This changes the logic for the did document to not set default values for the did document. This seemed convenient to me at first, but in the end it causes problems when you need to get the original form of the did document.

This PR also removes the `DidPeer` class. I thought this would be convenient (and it was for a part), but it added way to much complexity. Especially as I tried to fix the issue with `did:peer:1` method and needing the raw json bytes (to consistently calculate the hash). I now replaced it with simple methods such as `keyToNumAlgo0DidDocument` or `didDocumentJsonToNumAlgo1Did`.

@jakubkoci this affects your PR because you can't use the `DidPeer` class anymore. Please take a look at `peer-did.test.ts` on how to use it without `DidPeer`. I didn't want to add more work, but the consistent hashing is quite important for interop with other agents down the line. You should make sure that when parsing a num algo 1 (`did:peer:1`) that is received from another agent we parse the json variant of the did document (`didDocumentJsonToNumAlgo1Did`) as the transformation to the `DidDocument` class can make the resulting document structure different.

BREAKING CHANGE: The `DidDocument` class doesn't set empty array values anymore for optional fields. This means you now have to check the value exists before being able to use it. This would mean that e.g. `didDocument.authentication.map()` would become `didDocument.authentication?.map()` to deal with the optionality of the field. This change was introduced to keep the class representation of a did document more in line with the actual representation of a did document.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-28 21:10:06 +0000 UTC
    </div>
</div>

