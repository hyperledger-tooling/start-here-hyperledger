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
                PR <a href="https://github.com/hyperledger/caliper/pull/1162" class=".btn">#1162</a>
            </td>
            <td>
                <b>
                    Make fixed load rate controller honor the target duration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--- Provide a general summary of the pull request in the Title above -->

## Checklist
 - ~~A link to the issue/user story that the pull request relates to~~
 - [x]  How to recreate the problem without the fix
 - [x]  Design of the fix
 - [x]  How to prove that the fix works
 - [x]  Automated tests that prove the fix keeps on working
 - ~~Documentation - any JSDoc, website, or Stackoverflow answers?~~


## Issue/User story
<!--- What issue / user story is this for -->
When using the fixed load rate controller we did run into issues where a hanging SUT or a suden drop in the SUT's TPS caused our target duration exceeded by a factor of 50.

## Steps to Reproduce
<!--- Provide a link to a live example, or an unambiguous set of steps to -->
<!--- reproduce this bug include code to reproduce, if relevant -->
Running the benchmarks added in https://github.com/hyperledger/besu/pull/2716 with higher transaction backlogs than used in https://github.com/hyperledger/besu/pull/2716/files#diff-bbce9037b01a9a2ee863e5a760f513e416f2efa57669582a6c316a168044c310 causes this behaviour--e.g. with backlog 300 instead of the used 200. The benchmarks can be executed using `cd benchmark && docker-compose -f docker-compose.yml run caliper`.


## Existing issues
<!-- Have you searched for any existing issues or are their any similar issues that you've found? -->
- [ ] [Stack Overflow issues](http://stackoverflow.com/tags/hyperledger-caliper)
- [ ] [GitHub Issues](https://github.com/hyperledger/caliper/issues)
- [ ] [Rocket Chat history](https://chat.hyperledger.org/channel/caliper)

<!-- please include any links to issues here -->

## Design of the fix
<!-- Focus on why you designed this fix this way, and what was discounted. Do not describe just the code - we can read that! -->
1. The total runtime of a round is bounded by twice the target duration. Exceeding it causes aborting with an exception.
2. The fixed load rate controller is modified to wait indefinitely as long as the target backlog size is exceeded by a factor of more than two.

## Validation of the fix
<!-- Over and above the tests, what has been done to prove this works? -->
- [x] Tested via unit test
- [ ] Tested using the above mentioned besu benchmark suite

## Automated Tests
<!-- Please describe the automated tests that are put in place to stop this recurring -->
Unit tests are adapted and added for the fixed load rate controller.

## What documentation has been provided for this pull request
<!-- JSDocs, WebSite and answers to Stack Overflow questions are possible documentation sources -->
None.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-15 22:59:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1156" class=".btn">#1156</a>
            </td>
            <td>
                <b>
                    allow creating onchain privacy groups during test setup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Taccat Isid <taccatisid@protonmail.com>

<!--- Provide a general summary of the pull request in the Title above -->

## Checklist
 - ~~A link to the issue/user story that the pull request relates to~~
 - [x]  How to recreate the problem without the fix
 - [x]  Design of the fix
 - [x]  How to prove that the fix works
 - [x]  Automated tests that prove the fix keeps on working
 - [ ]  Documentation - any JSDoc, website, or Stackoverflow answers?


## Issue/User story
<!--- What issue / user story is this for -->
When using caliper with onchain privacy the user currently has to create privacy groups outside of caliper and then record the privacyGroupId in the caliper network config. The id itself is created randomly. Having a fixed value in the caliper network config would require to also have a lot of ossified smart contract state the besu genesis file.

## Existing issues
<!-- Have you searched for any existing issues or are their any similar issues that you've found? -->
- [x] [Stack Overflow issues](http://stackoverflow.com/tags/hyperledger-caliper)
- [x] [GitHub Issues](https://github.com/hyperledger/caliper/issues)
- [x] [Rocket Chat history](https://chat.hyperledger.org/channel/caliper)

<!-- please include any links to issues here -->

## Design of the fix
The setup phase of the ethereum connector was extended to allow creation of privacy groups. The generated group ids are injected into the configuration and passed to individual workers via `prepareWorkerArguments` and `getContext`.
<!-- Focus on why you designed this fix this way, and what was discounted. Do not describe just the code - we can read that! -->

## Validation of the fix
<!-- Over and above the tests, what has been done to prove this works? -->
The PR has been tested by using both the existing and the extended (see below) integration tests.

## Automated Tests
<!-- Please describe the automated tests that are put in place to stop this recurring -->
The existing privacy integration tests have been modified to use onchain privacy with dynamically generated groups. It would be preferable to test onchain and legacy privacy groups at the same time. But a single besu instance only supports one or the other and using onchain allows for far more coverage.

## What documentation has been provided for this pull request
<!-- JSDocs, WebSite and answers to Stack Overflow questions are possible documentation sources -->
None so far.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 06:07:27 +0000 UTC
    </div>
</div>

