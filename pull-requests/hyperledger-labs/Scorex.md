---
layout: default
title: Scorex
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/Scorex
---

# Scorex <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/Scorex){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/Scorex/pull/397" class=".btn">#397</a>
            </td>
            <td>
                <b>
                    handle db errors at higher level
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                @kushti This is the most important part to review. `reportModifierIsValid` and `reportModifierIsInvalid` now return `Try` so this is the "higher level" place where we propagated the DB errors to. I did not publish any event as this is neither `semantically` nor `syntactically` failed modification, it just cannot be persisted. 

It differs as now DB errors leads to returning : 
```
                UpdateInformation(history, updateInfo.state, Some(modToApply), None, updateInfo.suffix)
```
which would lead to another `updateState` call which is probably wrong, it is just to demonstrate that we are handling that effect now.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-30 08:07:11 +0000 UTC
    </div>
</div>

