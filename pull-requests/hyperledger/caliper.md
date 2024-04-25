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
                PR <a href="https://github.com/hyperledger/caliper/pull/1553" class=".btn">#1553</a>
            </td>
            <td>
                <b>
                    Update docs around fabric-gateway and 0.5.1 release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - prepare vNext to represent a 0.5.1 release
- move all references of fabric to now demonstrate the `fabric-gateway`

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-23 14:56:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1552" class=".btn">#1552</a>
            </td>
            <td>
                <b>
                    remove bit.ly link as it could have been hacked
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
        Created At 2024-04-23 08:44:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1551" class=".btn">#1551</a>
            </td>
            <td>
                <b>
                    Update versions of node in docs
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
        Created At 2024-04-23 08:32:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1545" class=".btn">#1545</a>
            </td>
            <td>
                <b>
                    Remove collection of node gc stats in prometheus
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                reasons for this

1. we have never documented the metrics
2. not sure how much use it is anyway
3. was using an old version of gc-stats which is now unmaintained and has security issues
4. replacement version of gc-stats is maintained by a single person who controls the binary builds available so is a dangerous thing to rely on
5. it has no pure javascript fallback therefore requires caliper to pull down or build a binary module (meaning you need python and compilers installed) which will also be dependent on the version of node being used.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-22 10:22:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1544" class=".btn">#1544</a>
            </td>
            <td>
                <b>
                    Removed unused dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--- Provide a general summary of the pull request in the Title above -->

## Checklist
 - [x]  A link to the issue/user story that the pull request relates to
 - [ ]  How to recreate the problem without the fix
 - [ ]  Design of the fix
 - [ ]  How to prove that the fix works
 - [ ]  Automated tests that prove the fix keeps on working
 - [ ]  Documentation - any JSDoc, website, or Stackoverflow answers?


## Issue/User story
#1365 

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
        Created At 2024-04-20 07:26:39 +0000 UTC
    </div>
</div>

