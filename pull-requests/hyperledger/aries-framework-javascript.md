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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1437" class=".btn">#1437</a>
            </td>
            <td>
                <b>
                    chore: export askar types
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
        Created At 2023-04-19 08:05:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1436" class=".btn">#1436</a>
            </td>
            <td>
                <b>
                    chore(ci): switch to dedicated Aries runners
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
        Created At 2023-04-19 00:31:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1435" class=".btn">#1435</a>
            </td>
            <td>
                <b>
                    feat: Add cheqd demo and localnet for tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds the required Readme files and integrates cheqd modules in the demo

Also included a setup-cheqd in ./.github/actions which starts a localnet for the tests to be run
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-17 12:33:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1434" class=".btn">#1434</a>
            </td>
            <td>
                <b>
                    fix(indy-vdr): do not force indy-vdr version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I'm not sure if @hyperledger/indy-vdr-shared and @hyperledger/indy-vdr-nodejs versions are fixed to a particular version on purpose, but tests seem to work fine on the latest 0.1.0-dev.14.

This is mainly to fix https://github.com/hyperledger/aries-agent-test-harness/issues/669. If the version should be fixed to dev.13, another possibility is to fix it in the AATH backchannel.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-16 14:56:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1433" class=".btn">#1433</a>
            </td>
            <td>
                <b>
                    fix(connections): store imageUrl when using DIDExchange
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It was already fixed for Connection protocol in https://github.com/hyperledger/aries-framework-javascript/pull/896 but missing for DID Exchange.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-14 18:46:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1431" class=".btn">#1431</a>
            </td>
            <td>
                <b>
                    fix: issuance with unqualified identifiers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bigger PR than anticipated, but this fixes the issuance of credentials with unqualified identifiers. You can now issue with both unqulaiifed and did indy identifiers interchangeably, but only for the issuance side. the other sides don't work interchangeably yet. 

I hope this is one of the last big tasks before releasing 0.4.0?

Lot of code is moving around stuff and removing some of the duplicated code. We now have indy specific identifier code in the anoncreds package, but it's needed for the unqualified handling. As it's part of the spec, and it can provide the easiest migration path, that is okay by me. (it's not much, just some identifier parsing etc..)

Hope this doesn't clash too much with your Revocation pr @genaris 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 18:57:20 +0000 UTC
    </div>
</div>

