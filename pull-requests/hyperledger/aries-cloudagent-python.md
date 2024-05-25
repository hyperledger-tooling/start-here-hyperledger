---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2968" class=".btn">#2968</a>
            </td>
            <td>
                <b>
                    Sonarcloud with code coverage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is used to get code coverage for our sonarcloud integration on PR's and when code is pushed to main. 

The complication comes with using the sonarcloud token from forked repos. I have tested using two github accounts and forking my fork. 

This works by saving the test report from the `PR Tests` workflow as an artifact and also the pr number. Then when the `PR Tests` workflow completes successfully a workflow will begin for sonarcloud witch gets information about the forked repo, and fetches the code for the scan. The code coverage is downloaded from the artifact, updated and then upload to sonarcloud.

Another workflow runs the tests on merge to main, runs the scan and uploads results. I thought about doing this as one workflow but decided separate workflows was actually much simpler.

I changed the workflow `Tests` to an action and adjusted the other workflows that used it. When calling from the push to main workflow it was having trouble as a workflow.

Requires disabling `Automatic Analysis` in the sonarcloud admin console. You can't use automatic and manage it from CI at the same time. Also won't exist until the workflows have been merged to main.

Main branch:

![image](https://github.com/hyperledger/aries-cloudagent-python/assets/31809382/028b59c9-6977-4402-a26b-5d693305b3a3)

PR (Failing):

The required coverage can be adjusted in sonarcloud console.

![image](https://github.com/hyperledger/aries-cloudagent-python/assets/31809382/4b30d724-da76-4187-ae6b-619e8c839568)

![image](https://github.com/hyperledger/aries-cloudagent-python/assets/31809382/ee0efd1a-d5fb-4ffe-8c2b-5c6a0b2f0890)

![image](https://github.com/hyperledger/aries-cloudagent-python/assets/31809382/a6ec57c1-ac31-4802-b93d-4cdddc4ada9d)

PR (Passing):

![image](https://github.com/hyperledger/aries-cloudagent-python/assets/31809382/ff860d3b-5746-4248-8c30-b69f1334d79e)


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-24 19:51:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2967" class=".btn">#2967</a>
            </td>
            <td>
                <b>
                    Add support for revocable credentials in vc_di handler
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
        Created At 2024-05-24 11:15:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2961" class=".btn">#2961</a>
            </td>
            <td>
                <b>
                    Fix Snyk sarif file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes the issue with Snyk sarif file. Replace any "null" security severity values with 0. The null value is used in the case of license-related findings, which do not do not indicate a security vulnerability.

See https://github.com/github/codeql-action/issues/2187 for more context.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-21 19:27:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2960" class=".btn">#2960</a>
            </td>
            <td>
                <b>
                    feat: VC DI proof request
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
        Created At 2024-05-21 18:09:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2959" class=".btn">#2959</a>
            </td>
            <td>
                <b>
                    DIDComm V2 Initial Implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The purpose of this PR is to add basic DIDComm V2 support to ACA-Py. It is our intention to add support gradually with small PRs, rather than one massive PR. To that end, at present, here's what we've added:

- Added `--experimental-didcomm-v2` flag to enable the DIDComm V2 code
- Added the ability to decrypt/unpack V2 messages
- When a message is received, we respond back with a DIDComm V1 problem report (there-by, providing a foundation to rely upon when adding protocols) and pack it the same way that we'd pack a DIDComm V2 message
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-21 14:50:00 +0000 UTC
    </div>
</div>

