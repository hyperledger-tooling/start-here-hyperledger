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

