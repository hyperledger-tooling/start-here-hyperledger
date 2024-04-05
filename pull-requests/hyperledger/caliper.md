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
                PR <a href="https://github.com/hyperledger/caliper/pull/1526" class=".btn">#1526</a>
            </td>
            <td>
                <b>
                    Resolve issue with documentation rendering locally #1525
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
 - [x]  How to recreate the problem without the fix
 - [x]  Design of the fix
 - [x]  How to prove that the fix works
 - [x]  Automated tests that prove the fix keeps on working
 - [ ]  Documentation - any JSDoc, website, or Stackoverflow answers?

## Issue/User story
<!--- What issue / user story is this for -->
Link to the issue: #1525 

## Steps to Reproduce
<!--- Provide a link to a live example, or an unambiguous set of steps to -->
<!--- reproduce this bug include code to reproduce, if relevant -->
1. Navigate to the documentation section.
2. Attempt to run the documentation locally using the previous configuration.
3. Observe the error related to loading 'rexml/parsers/baseparser' file.

## Design of the fix
<!-- Focus on why you designed this fix this way, and what was discounted. Do not describe just the code - we can read that! -->
The fix involved updating the Gemfile to use newer versions of dependencies, specifically targeting the issue related to loading 'rexml/parsers/baseparser' file. This approach was chosen to address the root cause of the error and ensure compatibility with the latest dependencies.

## Validation of the fix
<!-- Over and above the tests, what has been done to prove this works? -->
After implementing the fix, I tested it locally by running the documentation server. The error related to loading 'rexml/parsers/baseparser' file no longer occurred, confirming that the fix resolves the issue.

## Automated Tests
<!-- Please describe the automated tests that are put in place to stop this recurring -->
Automated tests were not applicable for this fix.

## What documentation has been provided for this pull request
<!-- JSDocs, WebSite and answers to Stack Overflow questions are possible documentation sources -->
Documentation update is pending.

## Screenshots
<!-- Include screenshots here to visually demonstrate the fix -->
![Screenshot 1]
![Screenshot 2024-04-04 233610](https://github.com/hyperledger/caliper/assets/96948435/fe78130d-91dc-47f0-8d3f-bc94a7cc9d89)


![Screenshot 2](
![Screenshot 2024-04-04 233701](https://github.com/hyperledger/caliper/assets/96948435/a6aaa8e8-02b3-4af5-8a6b-f00a932914e2)


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-04 18:25:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1524" class=".btn">#1524</a>
            </td>
            <td>
                <b>
                    Update PSWG whitepaper link in README #1518
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
 - [x]  How to recreate the problem without the fix
 - [x]  Design of the fix
 - [x]  How to prove that the fix works
 - [x]  Automated tests that prove the fix keeps on working
 - [ ]  Documentation - any JSDoc, website, or Stackoverflow answers?

## Issue/User story
<!--- What issue / user story is this for -->
Fixes #1518

## Steps to Reproduce
1.Open the README.md file.
2.Click on the PSWG whitepaper link

## Design of the fix
<!-- Focus on why you designed this fix this way, and what was discounted. Do not describe just the code - we can read that! -->
The fix updates the PSWG white paper link in the README file to the correct URL: https://www.hyperledger.org/learn/publications/blockchain-performance-metrics. 

## Screenshots
![Screenshot 1] Before Correction
![image](https://github.com/hyperledger/caliper/assets/96948435/56ba1eae-f579-42fa-bc2a-28fb132db6aa)

![Screenshot 2] After Correction
![image](https://github.com/hyperledger/caliper/assets/96948435/0e11acc4-7627-4a23-94ce-6bd8baac89fe)



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-02 15:19:32 +0000 UTC
    </div>
</div>

