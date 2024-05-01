---
layout: default
title: caliper
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/caliper
---

# caliper <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/caliper){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1559" class=".btn">#1559</a>
            </td>
            <td>
                <b>
                    `caliper-ethereum` : Add new tests for packages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--- Provide a general summary of the pull request in the Title above -->
# Adding Test Cases for Ethereum Connector

This pull request introduces a set of test cases for the Ethereum Connector. These tests are currently contradictory in nature, as they are designed to cover various edge cases and potential error conditions, that is, varying results when called from `packages/caliper-ethereum/lib/connectorFactory.js` v/s that from `packages/caliper-ethereum/lib/ethereum-connector.js`

Given the complexity of these scenarios, this PR is opened as a draft. The intention is to invite feedback and discussion on the test cases and their expected outcomes. Once the testing has been completed thoroughly and all issues have been addressed, this PR will be marked ready for review.

## Checklist
 - [x]  A link to the issue/user story that the pull request relates to~ #1556 
 - [ ]  How to recreate the problem without the fix
 - [ ]  Design of the fix
 - [ ]  How to prove that the fix works
 - [ ]  Automated tests that prove the fix keeps on working
 - [ ]  Documentation - any JSDoc, website, or Stackoverflow answers?


## Issue/User story
<!--- What issue / user story is this for -->


## Steps to Reproduce
<!--- Provide a link to a live example, or an unambiguous set of steps to -->
<!--- reproduce this bug include code to reproduce, if relevant -->
1. `cd packages/caliper-ethereum && npm i && npm run dev`
2.
3.
4.


## Existing issues
<!-- Have you searched for any existing issues or are their any similar issues that you've found? -->
- [ ] [Stack Overflow issues](http://stackoverflow.com/tags/hyperledger-caliper)
- [x] [GitHub Issues](https://github.com/hyperledger/caliper/issues)
- [ ] [Discord history](https://discord.com/channels/905194001349627914/941417677778473031)

<!-- please include any links to issues here -->

## Design of the fix
<!-- Focus on why you designed this fix this way, and what was discounted. Do not describe just the code - we can read that! -->

## Validation of the fix
<!-- Over and above the tests, what has been done to prove this works? -->

## Automated Tests
<!-- Please describe the automated tests that are put in place to stop this recurring -->

## What documentation has been provided for this pull request
<!-- JSDocs, WebSite and answers to Stack Overflow questions are possible documentation sources -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-30 21:19:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1558" class=".btn">#1558</a>
            </td>
            <td>
                <b>
                    `caliper-core`: add tests for `assignedMessage`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Checklist
 - [X]  A link to the issue/user story that the pull request relates to
 - [ ]  How to recreate the problem without the fix
 - [ ]  Design of the fix
 - [ ]  How to prove that the fix works
 - [X]  Automated tests that prove the fix keeps on working
 - [ ]  Documentation - any JSDoc, website, or Stackoverflow answers?


## Issue/User story
Fixes part of #1557 

## Steps to Reproduce
<!--- Provide a link to a live example, or an unambiguous set of steps to -->
<!--- reproduce this bug include code to reproduce, if relevant -->
1.
2.
3.
4.


## Existing issues
<!-- Have you searched for any existing issues or are their any similar issues that you've found? -->
- [ ] [Stack Overflow issues](http://stackoverflow.com/tags/hyperledger-caliper)
- [ ] [GitHub Issues](https://github.com/hyperledger/caliper/issues)
- [ ] [Discord history](https://discord.com/channels/905194001349627914/941417677778473031)

<!-- please include any links to issues here -->

## Design of the fix
<!-- Focus on why you designed this fix this way, and what was discounted. Do not describe just the code - we can read that! -->

## Validation of the fix
<!-- Over and above the tests, what has been done to prove this works? -->

## Automated Tests
<!-- Please describe the automated tests that are put in place to stop this recurring -->

## What documentation has been provided for this pull request
<!-- JSDocs, WebSite and answers to Stack Overflow questions are possible documentation sources -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-25 18:48:57 +0000 UTC
    </div>
</div>

