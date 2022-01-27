---
layout: default
title: aries-agent-test-harness
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-agent-test-harness
---

# aries-agent-test-harness <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-agent-test-harness){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/422" class=".btn">#422</a>
            </td>
            <td>
                <b>
                    aries-vcx: Fix tails file upload, improve error handling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Miroslav Kovar <miroslavkovar@protonmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 11:38:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/421" class=".btn">#421</a>
            </td>
            <td>
                <b>
                    Changes by create-pull-request action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Automated changes by [create-pull-request](https://github.com/peter-evans/create-pull-request) GitHub action
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 03:52:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/420" class=".btn">#420</a>
            </td>
            <td>
                <b>
                     aries-vcx: Update aries-vcx version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Miroslav Kovar <miroslavkovar@protonmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-26 15:39:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/419" class=".btn">#419</a>
            </td>
            <td>
                <b>
                    docs(api): issue credential and present proof v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds open api definitions for the issue credential and present proof v2 endpoints
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-25 17:58:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/418" class=".btn">#418</a>
            </td>
            <td>
                <b>
                    reversed the if condition for github actions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

Yesterdays if condition was incorrect. logs will now not be copied when running in GitHub. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-25 13:56:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/417" class=".btn">#417</a>
            </td>
            <td>
                <b>
                    refactor: remove backchannel operations csv file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As discussed with @nodlesh, I'd give it a try to remove the backchannel operation matching. The google sheet hasn't been updated for a while and we had to manually edit the CSV. Although this is doable, it doesn't provide the best DX. Only the python based backchannels parsed the CSV file.

I removed the matching of the operations in the python based backchannels and created a `BackchannelCommand` class. This contains everything related to the received command (such as `data`, `record_id`, `topic`, etc..). 

In addition this PR:
- cleans up the backchannels a bit and remove unused code
- Formats the python based backchannels using black (I intend to do a separate PR for the `aries-test-harness` directory)
- Removes all references to the backchannel operations CSV and also updates all documentation referencing it

The recommended approach to document new endpoints are now through the OpenAPI spec located in this repo. 


The following entry in the `backchannel_operations.csv` 

```
0454 Present Proof v2,X,,proof-v2,POST,verify-presentation,Y,,Verify a received proof presentation,presentation_thread_id,,state
```

can be translated to the following entry in the OpenAPI spec. It is a bit more verbose, but basically contains the sae information. The big advantage is that we can now render it nicely (as done here: https://aries-interop.info/api), helping backchannel implementors.

```yaml
  /agent/command/proof-v2/verify-presentation:
    post:
      tags:
        - Present Proof V2
      summary: Verify presentation
      description: >
        Verify the received presentation with specified thread id.
      operationId: PresentProofV2VerifyPresentation
      requestBody:
        required: true
        content:
          application/json:
            schema:
              type: object
              required:
                - id
              properties:
                id:
                  $ref: "#/components/schemas/ThreadId"
      responses:
        200:
          description: Presentation verified
          content:
            application/json:
              schema:
                allOf:
                  - $ref: "#/components/schemas/PresentProofV2OperationResponse"
                  - properties:
                      state:
                        example: done
```

I intend to add all missing endpoints (mostly related to OOB/DIDExchange/V2 Protocols/Revocation) while I work on related aspects of the harness in the coming weeks.

A lot of changes, but the operations file touched a lot of backchannels so it was a bit hard to split up.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-25 10:07:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/416" class=".btn">#416</a>
            </td>
            <td>
                <b>
                    added the case not to copy logs if in GITHUB ACTIONS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

To further diagnose the cancel on the acapy-aries-vcx run, this PR makes copying agent logs conditional on being in GITHUB_ACTIONS. Copying the logs is the next thing that happens at about the point the cancel happens. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-24 23:18:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/415" class=".btn">#415</a>
            </td>
            <td>
                <b>
                    fixed workflow names to match filename
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

This may not clear up the cancelled jobs, but at least we will have a clearer picture of what jobs are being cancelled. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-21 18:49:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/414" class=".btn">#414</a>
            </td>
            <td>
                <b>
                    further separated crons for less parallel execution
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

This may fix the cancelled jobs in the daily interop test runs. If this does work, that means ultimately we need to move to the matrix model so this doesn't happen again. This current submission is just to prove the crons are/were the problem. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-20 13:40:16 +0000 UTC
    </div>
</div>

