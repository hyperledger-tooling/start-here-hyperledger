---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3226" class=".btn">#3226</a>
            </td>
            <td>
                <b>
                    fix: vc-revocation-list-2021 context
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Firas Qutishat <firas.qutishat@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-22 11:50:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3225" class=".btn">#3225</a>
            </td>
            <td>
                <b>
                    chore: add revocation list 2021 context
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Firas Qutishat <firas.qutishat@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-22 10:54:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3224" class=".btn">#3224</a>
            </td>
            <td>
                <b>
                    Port Aries Agent to AWS Lambda
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
Port Aries Agent to AWS Lambda

**Description:**
Port the Agent to run on AWS Lambda, using APIGW and DynamoDB as the supporting infrastructure for transport and storage, respectively.

**Summary:**
The PR includes both a Go application and the Serverless + Serverless Offline framework in order to deploy and run locally for debug purposes. Yarn is used to track the Serverless part of the stack.
The Go application is the agent itself, build to run on AWS Lambda. The main communication with Lambda is handled via github.com/aws/aws-lambda-go/lambda.It uses DynamoDB as both persistent and temporary storage since Lambda runs are ephemeral. The DIDComm transports are handled using APIGW, with WebSockets requiring a bit more dedicated steps. One issue we've identified here is the main app finishing sooner and Lambda terminating the app before auto-approve has had a chance to respond (this only seems to affect the deployed app and does not affect the locally running Serverles Offline app). The temporary hacks we've put in place add a 5 second delay and that seems to work most of the time. This is only a draft for now, as we'd like help on clearing that (perhaps by using WaitGroups or another synchronization mechanism?), and we've left other hacky bits/comments/debugging in place.
We've also noticed issues with custom message endpoints (but we think this is out of scope, for now). The Aries Agent running on AWS Lambda seems like a perfect fit for Mediator purposes, allowing wallets running on the edge to communicate via WebSockets and avoid exposing ports.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 21:35:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3223" class=".btn">#3223</a>
            </td>
            <td>
                <b>
                    refactor: endpoint as object, goal-code with underscore
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Following this DIDcomm V2 spec udpate:
https://github.com/decentralized-identity/didcomm-messaging/pull/352
The endpoint field is now a structure containing a URI, Accept and the RoutingKeys.
and
https://github.com/decentralized-identity/didcomm-messaging/pull/363
goal-code is now goal_code.

Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 15:33:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3222" class=".btn">#3222</a>
            </td>
            <td>
                <b>
                    fix(vcwallet): correct order of test arguments
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jan Christoph Ebersbach <jan-christoph.ebersbach@identinet.io>

Use the following template for your PR (make sure you follow our
[guidelines](CONTRIBUTING.md#pull-request):

**Title:**
Correct order of test arguments.

**Description:**
The order of test arguments is the wrong way around

**Summary:**

The patch swaps the order of arguments.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-19 08:34:56 +0000 UTC
    </div>
</div>

