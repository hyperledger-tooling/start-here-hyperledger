---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/284" class=".btn">#284</a>
            </td>
            <td>
                <b>
                    Rebuild Cargo.lock
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-31 12:47:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/282" class=".btn">#282</a>
            </td>
            <td>
                <b>
                    Commit node wrapper package.json, updated dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-30 17:14:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/281" class=".btn">#281</a>
            </td>
            <td>
                <b>
                    Release 0.18.0
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
        Created At 2021-05-26 19:23:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/280" class=".btn">#280</a>
            </td>
            <td>
                <b>
                    Changes related to aries test harness backchannel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">breaking</span><span class="chip">enhancement</span><span class="chip">integration</span>
            </td>
            <td>
                Previously, invitee's states were 
```
Null, Invited, Requested, Completed
```
whereas inviter's states were
```
Null, Invited, Responded, Completed
```
This in order to achieve compatibility with [RFC0160](https://github.com/hyperledger/aries-rfcs/tree/master/features/0160-connection-protocol), this PR adds a new state for both inviter and invitee, making the state set
```
Null, Invited, Requested, Responded, Completed
```
for both.

Moreover, mapping of the states to `VcxStateType` was changed such that the `Null` state (the initial and "errored" state) maps the the zeroth state (`VcxStateNone`) instead of the first state (`VcxStateInitialized`) and the transition progress the mapped `VcxStateType` in unit increments. This is a breaking change.

Finally, to achieve backwards compatibility, an `autohop` flag was added to the state machine, which skips the `Responded` and `Requested` states for invitee and inviter respectively.

Related: https://github.com/hyperledger/aries-agent-test-harness/pull/243

Signed-off-by: Miroslav Kovar <miroslavkovar@protonmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-25 20:36:26 +0000 UTC
    </div>
</div>

