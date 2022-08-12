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
                PR <a href="https://github.com/hyperledger/caliper/pull/1438" class=".btn">#1438</a>
            </td>
            <td>
                <b>
                    Collect Prometheus metrics in manager using messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Alternative implementation that works for both local and remote workers.
(This is just a draft implementation, discussions are ongoing in Discord)

## Checklist
 - [x]  A link to the issue/user story that the pull request relates to
 - [ ]  How to recreate the problem without the fix
 - [ ]  Design of the fix
 - [ ]  How to prove that the fix works
 - [ ]  Automated tests that prove the fix keeps on working
 - [ ]  Documentation - any JSDoc, website, or Stackoverflow answers?


## Issue/User story
#1353

## Design of the fix
WIP

## Validation of the fix
|Approach|Results|
|:--:|:--:|
|PushGateway with local workers and mqtt communication|![image](https://user-images.githubusercontent.com/36656347/183692152-be68eb1f-a34c-4b09-aeac-50ab29bfc03e.png)|
|This PR (metrics communicated using messages) with local workers and mqtt communication|![image](https://user-images.githubusercontent.com/36656347/183691928-b704009f-f7dc-4dd6-8bbb-f0206ce0790a.png)|
|PR #1434 (metrics communicated using IPC) with local workers and mqtt communication|![image](https://user-images.githubusercontent.com/36656347/183694509-08504e92-0584-46f2-a5e5-e220187cf6f7.png)|

## Automated Tests
WIP

## What documentation has been provided for this pull request
WIP

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-09 15:38:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1435" class=".btn">#1435</a>
            </td>
            <td>
                <b>
                    Terminate Caliper workers on interrupting Caliper manager
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In this PR:
* The SIGINT signal is handled in the manager to cleanly terminate workers when user tries to terminate Caliper manager.

Fixes #1361
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-06 13:24:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1434" class=".btn">#1434</a>
            </td>
            <td>
                <b>
                    Add Prometheus scrape target server to Caliper manager
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                (This is just a draft implementation, discussions are ongoing in Discord)

## Checklist
 - [x]  A link to the issue/user story that the pull request relates to
 - [ ]  How to recreate the problem without the fix
 - [ ]  Design of the fix
 - [ ]  How to prove that the fix works
 - [ ]  Automated tests that prove the fix keeps on working
 - [ ]  Documentation - any JSDoc, website, or Stackoverflow answers?


## Issue/User story
#1353

## Design of the fix
WIP

## Validation of the fix
![image](https://user-images.githubusercontent.com/36656347/183242780-81800421-ebb2-444d-95a6-fa139a8a6666.png)

## Automated Tests
WIP

## What documentation has been provided for this pull request
WIP

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-06 09:46:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1433" class=".btn">#1433</a>
            </td>
            <td>
                <b>
                    Upload coverage reports on merge
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In this PR:
* The coverage report workflow is run on merge as well so that the coverage of the main branch can be obtained and used as a basis for comparing the coverage of PRs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-05 19:07:56 +0000 UTC
    </div>
</div>

