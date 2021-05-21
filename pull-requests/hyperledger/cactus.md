---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/979" class=".btn">#979</a>
            </td>
            <td>
                <b>
                    fix(ci): re-run CI when base branch (main) is updated
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span><span class="chip">Triage_Needed</span><span class="chip">dependencies</span>
            </td>
            <td>
                Allegedly, the 'edited' event will get triggerd if the base branch of
the PR gets pushed commits to it (e..g whenever another PR gets
merged).
So we enable running the CI task on that event with this commit.

This is intended to prevent the following scenario from
happening (which also has happened this week)

1. PR 1 is opened, CI passes
2. PR 2 is opened, CI passes
3. PR 2 is merged and it introduces a breaking API change that stops
PR 1 from compiling.
4. Right after PR 2 was merged, PR 1 gets merged as well since it has
the approvals and the CI has passed back when it was opened (based
on the old state of the main branch)
5. Now main is corrupted because the CI never ran against the rebased
version of the branch of PR 1 so it just slips right in with a change that
doesn't even compile let alone pass the tests.

Source of the allegations regarding the 'edited' event:
https://github.community/t/rerun-on-base-branch-change/115594/2

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 21:33:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/978" class=".btn">#978</a>
            </td>
            <td>
                <b>
                    fix(carbon-accounting): deleted incorrect plugin aspect
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #977 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 12:34:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/976" class=".btn">#976</a>
            </td>
            <td>
                <b>
                    feat(htlc-coordinator): new htlc coordinator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                Resolve #953 

Depends on #582
Depends on #580 
Depends on #978
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 10:34:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/972" class=".btn">#972</a>
            </td>
            <td>
                <b>
                    docs(video): video guide added to build.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                Resolve #413 

Depends on #977 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-19 07:40:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/969" class=".btn">#969</a>
            </td>
            <td>
                <b>
                    feat(Go-Ethereum Validator): add getNonceHex on Go-Ethereum Validator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Related to Issue #970 

Contents:
- (main) [Validator] add getNonce as execSyncFunction on Go-Ethereum Validator in order to solve #970.
- (sub) [car-trade] refactor to use the above function instead of web3 function.

Signed-off-by: Takuma TAKEUCHI <takeuchi.takuma@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-17 14:22:50 +0000 UTC
    </div>
</div>

