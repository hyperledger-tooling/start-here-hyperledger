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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/804" class=".btn">#804</a>
            </td>
            <td>
                <b>
                    docs: add ios ledger troubleshooting information
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These docs address issues found with multiple ledgers in iOS release environments found in #647. The solutions present in the docs have been tested in Bifold [PR #336](https://github.com/hyperledger/aries-mobile-agent-react-native/pull/336).


Other contributors who assisted: @reflectivedevelopment, @TheTreek, @amanji
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-26 19:35:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/803" class=".btn">#803</a>
            </td>
            <td>
                <b>
                    fix: Async ledger connection issues on iOS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change `connectToPools` function to sequentially connect to pools. Previously there were [issues on iOS](https://github.com/hyperledger/aries-framework-javascript/issues/647) because of too many open sockets on this function.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-26 19:25:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/801" class=".btn">#801</a>
            </td>
            <td>
                <b>
                    refactor: move signatures suites to vc module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This moves the signature suites, the jsonld util and other files to the vc module. This will help with the separation of credential formats we're going to look at soon. It also fixes an issue with type files being places outside of the src directory causing build issues. We didn't catch this because CI was not enabled on the 0.3.0 branch. CI is now enabled which gives us more assurance when merging PRs.

This doesn't change anything about the functionality. It's just relocation, and fixing of type issues.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-26 09:51:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/799" class=".btn">#799</a>
            </td>
            <td>
                <b>
                    ci: run ci on -pre branches
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Run ci on pre branches so we also have this enabled for the 0.3.0-pre (and others in the future) branches
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-25 14:18:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/798" class=".btn">#798</a>
            </td>
            <td>
                <b>
                    fix(credentials): add missing issue credential v1 proposal attributes
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
        Created At 2022-05-25 12:58:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/797" class=".btn">#797</a>
            </td>
            <td>
                <b>
                    refactor(credentials): minor refactor of CredentialMessageBuilder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Mainly to make it more consistent with the rest of AFJ
- Cleaned up the `CredentialMesssageBuilder` a small bit
- Mainly removed unnecessary types and checks for undefined values
- Not completely done (will continue later in other PRs) 

Signed-off-by: Berend Sliedrecht <berend@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-25 12:50:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/796" class=".btn">#796</a>
            </td>
            <td>
                <b>
                    fix(core): expose CredentialPreviewAttribute
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - file rename from `CredentialPreviewAttributes` to `CredentialPreviewAttribute`
- export `CredentialPreviewAttribute` to the framework user for building a credential offer

Signed-off-by: Berend Sliedrecht <berend@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-25 12:18:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/795" class=".btn">#795</a>
            </td>
            <td>
                <b>
                    feat: Issue Credentials V2: W3C/ jsonld credentials
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Merge of jsonld-credentials -> 0.3.0-pre
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-25 11:48:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/790" class=".btn">#790</a>
            </td>
            <td>
                <b>
                    fix: extract indy did from peer did in indy credential request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Amit-Padmani <amit.padmani@ontario.ca>

- Fetch publicKeyBase58 from did document,  generate the indy did and use for createRequest

Issue - [alpha76] Accept Offer Credential v1 not working [#780](https://github.com/hyperledger/aries-framework-javascript/issues/780)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-23 15:02:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/789" class=".btn">#789</a>
            </td>
            <td>
                <b>
                    fix: add BBS context to DidDoc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                BBS context was missing in the DidDocumentBuilder, resulting in some value being dropped during frameing. This PR adds the context.

Signed-off-by: Karim <karim@animo.id>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-23 12:09:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/787" class=".btn">#787</a>
            </td>
            <td>
                <b>
                    fix(routing): sending of trustping in pickup v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There was a bug discovered that would cause the first message in the pick up queue to be delivered when the trust ping was sent to create the web socket connection. This PR addresses that by only sending the trust ping when the request status receives a status of zero, then indicating to the mediator that we are ready to actively receive messages. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-20 16:36:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/786" class=".btn">#786</a>
            </td>
            <td>
                <b>
                    fix: invalid injection symbols in W3cCredService
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixed invalid injection symbols for Wallet and Logger in the W3cCredentialService.

Signed-off-by: Karim <karim@animo.id>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-20 12:58:36 +0000 UTC
    </div>
</div>

