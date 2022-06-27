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
                PR <a href="https://github.com/hyperledger/caliper/pull/1391" class=".btn">#1391</a>
            </td>
            <td>
                <b>
                    Fix#1377 Change the generator binding from 2.2 to 1.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Tezas-6174 <jamdade.2@iitj.ac.in>

- Fixes #1377.
- Changed the generator binding from 2.2 to 1.4 in ``run.sh`` in generator-tests of ``caliper-test-integration`` package.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-26 15:19:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1390" class=".btn">#1390</a>
            </td>
            <td>
                <b>
                    Pass secrets to CI workflow for publish
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In this PR:
* Secrets are passed on from the parent workflow to the publish workflow as described in the GitHub Actions documentation

Fixes #1389

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-26 11:16:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1387" class=".btn">#1387</a>
            </td>
            <td>
                <b>
                    Cache node modules across CI workflows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In this PR:
* The `node_modules` folder is cached across workflows using a method inspired by the workflow in [jupyterlab/extension-examples](https://github.com/jupyterlab/extension-examples/blob/master/.github/workflows/main.yml)

Closes #1374

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 17:42:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1385" class=".btn">#1385</a>
            </td>
            <td>
                <b>
                    Fix: When selecting v0.4.2 in the caliper docs the dropdown switches to 0.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes #1381

Signed-off-by: Shreesh Kulkarni <sgkul2000@gmail.com>

<!--- Provide a general summary of the pull request in the Title above -->

## Checklist
 - [ x ]  A link to the issue/user story that the pull request relates to
 - [ x ]  How to recreate the problem without the fix
 - [ x ]  Design of the fix
 - [ x ]  How to prove that the fix works
 - [ ]  Automated tests that prove the fix keeps on working
 - [ ]  Documentation - any JSDoc, website, or Stackoverflow answers?


## Issue/User story
#1381 

## Steps to Reproduce
 1. go to caliper docs
 2. select v0.4.2 under versions


## Design of the fix
the fix adds "selected" to the appropriate option to make it the selected option by default

## Validation of the fix
manual testing proves that the fix works

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-21 20:24:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1384" class=".btn">#1384</a>
            </td>
            <td>
                <b>
                    Port the publish workflow to GitHub Actions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In this PR:
* The publish workflow is ported from Azure Pipelines to GitHub Actions as it is. Optimizations would be done in later PRs
* The publish action currently runs after unit and integration tests on committing to the main branch

Closes #1369

This also closes the epic issue for migration.
Closes #1360
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-21 20:14:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1383" class=".btn">#1383</a>
            </td>
            <td>
                <b>
                    Fix #536: Minor changes in the error messages of 'caliper-fisco-bcos' package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Partially fixes # 536. 
- This PR contains very minor changes; including them as mentioned in the error logging issue to check the error messages of every package.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-21 19:19:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1382" class=".btn">#1382</a>
            </td>
            <td>
                <b>
                    Disable unit and integration tests in Azure Pipelines
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In this PR:
* The unit and integration test jobs in Azure pipelines are removed as they were migrated to GitHub Actions

Closes #1367 
Closes #1368 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-21 16:04:35 +0000 UTC
    </div>
</div>

