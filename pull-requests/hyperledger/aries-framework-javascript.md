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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1131" class=".btn">#1131</a>
            </td>
            <td>
                <b>
                    feat: Proof Negotiation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Łukasz Przytuła <lprzytula@gmail.com>

Allow proof negotiation by responding to presentation proposal with new presentation request, and responding to presentation request with new presentation proposal
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-29 23:05:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1121" class=".btn">#1121</a>
            </td>
            <td>
                <b>
                    refactor: simplify acceptXXX methods in Issue Credentials V2 JsonLdCredentialFormatService
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR addresses item 1 in issue #1089 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-28 09:44:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1120" class=".btn">#1120</a>
            </td>
            <td>
                <b>
                    fix(problem-report): proper string interpolation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: blu3beri <berend@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-28 09:25:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1119" class=".btn">#1119</a>
            </td>
            <td>
                <b>
                    fix: use custom document loader in jsonld.frame
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We use a custom document loader for tests that use local files instead of downloading them from the web. Inside this custom document loader, we're calling `jsonld.frame()`, but didn't pass the custom document loader. As a result, documents were being fetched from the web during tests, which made the tests fail when there is no internet connection.

This minor fix passes the custom document loader to the `jsonld.frame()` function and makes sure only local files are used.

Fixes #1111 

Signed-off-by: Karim Stekelenburg <karim@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-24 13:50:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1118" class=".btn">#1118</a>
            </td>
            <td>
                <b>
                    feat: add anon-creds package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ledger agnostic anoncreds</span>
            </td>
            <td>
                This PR adds a package that contains a set of interfaces that define unified APIs for AnonCreds related logic.

The goal of adding this package is that we can have two separate implementations, one for `indy-sdk` and another one for the `anoncreds-rs` Rust library that is currently being developed.

> **Note**: the interfaces in this package contain a lot of `todo` comments and `any` statements. The idea is to update these during the implementation of the first package.

Signed-off-by: Karim Stekelenburg <karim@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-24 13:05:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1116" class=".btn">#1116</a>
            </td>
            <td>
                <b>
                    fix(proofs): await shouldAutoRespond to correctly handle the check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We did not await the `shouldAutoRespondTo...` and if we then check if the value is truthy, it is because it is a Promise and not the contained value of `boolean`. 

Abstracting the async function call to a variable above makes an IDE error on the if statement is it will always be truthy if not-awaited.

@TimoGlastra Would it make sense to add a rule that you must mark void/await for async calls? that would've probably avoided this, quite big, bug.

closes #1095 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-23 13:53:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1115" class=".btn">#1115</a>
            </td>
            <td>
                <b>
                    feat: specify httpinboundtransport path
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Allows mediator to have configurable httpinbound endpoint, instead of just '/'

Signed-off-by: Niall Shaw <niall.shaw@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-23 11:34:05 +0000 UTC
    </div>
</div>

