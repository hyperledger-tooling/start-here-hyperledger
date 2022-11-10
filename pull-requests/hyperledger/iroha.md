---
layout: default
title: iroha
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha
---

# iroha <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2939" class=".btn">#2939</a>
            </td>
            <td>
                <b>
                    [feature] #2885: Define `TriggerExecuted` event
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span><span class="chip">api-changes</span>
            </td>
            <td>
                <!-- [feature] #2885: Define `TriggerExecuted` event -->
### Description of the Change
- Add `TriggerExecuted` as a variant of `Event`
  - Not a variant of `PipelineEvent` because trigger executions does not seem to fit `PipelineEvent` structure

### Issue
- Partial solution to #2885

### Benefits
- Data structure for notification of triggers execution

### Possible Drawbacks
- This event is assumed not to chain trigger executions at the moment. Developers can break this assumption and reach `unreachable!()`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-09 05:30:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2935" class=".btn">#2935</a>
            </td>
            <td>
                <b>
                    Added more descriptive Readme file.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Documentation</span><span class="chip">1.5</span>
            </td>
            <td>
                Describe how Hyperledger Iroha C++ library works. Provide examples. Show how to install and use the current version of the library.
Show how to run examples with transactions, batch and commands.
Benefits:
End user will know what the library is responsible for and how to use it properly.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-05 12:36:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2934" class=".btn">#2934</a>
            </td>
            <td>
                <b>
                    [ci]: Switсh dev tests to Equinix self-hosted runners
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                ### Description of the Change
1. Substitute default GitHub Actions runners with the `self-hosted` demand persistent instances _[s(1-4)-dev-iroha2-iroha-tech]_ with the following characteristics:
- CPU: 1 x Intel(R) Xeon(R) E-2278G
- RAM: 32 Gb
- Drive: 2 x 500 Gb
- OS: Ubuntu 22.04 LTS

For the following CI test jobs into `I2::Dev::Tests` workflow:
- check
- with_coverage
- integration
- unstable

2. Update links to `load-rs` CI.

### Issue
1. A long and heavy jobs from iroha2 CI take too much time on the default GitHub Actions runners.
2. Wrong configuration to call `load-rs` image compiltation.

### Benefits
1. Increase the speed, effectiveness and reliability of the heavy parts of iroha2 CI.
2. Fix `load-rs` CI trigger.

### Possible Drawbacks
1. Using a `self-hosted` runners, especially demand instances, for PR trigger workflows for open repositories is not a good practice: theoretically someone could execute malicious and undesirable code from his fork as PR's code. This requires being attentive and careful.
3. According to GitHub Actions settings, `self-hosted` runner can execute only one job from single workflow per unit of time. We added four instances for now, that means they can execute four jobs in the same time. May be we can try to add this `self-hosted` runners to job that builds `iroha2-dev` image as well. Perhaps we can add several instances more if it will be useful in the future.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-03 19:51:15 +0000 UTC
    </div>
</div>

