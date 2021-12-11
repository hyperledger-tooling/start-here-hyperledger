---
layout: default
title: mirbft
parent: Hyperledger Labs
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger-labs/mirbft
---

# mirbft <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/mirbft){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger-labs/mirbft/issues/79" class=".btn">79</a>
            </td>
            <td>
                <b>
                    Follow-up Events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">good first issue</span>
            </td>
            <td>
                Use the newly introduced `FollowUp` and `FollowUps` methods instead of directly accessing the Event's `Next` field.
This task corresponds to the following TODO:
https://github.com/hyperledger-labs/mirbft/blob/ba531de6b31449865b425cacc086577864c7dd50/pkg/pb/eventpb/methods.go#L3
This task involves looking up all direct accesses to the `Next` field and replacing them by the appropriate calls to `FollowUp` and `FollowUps`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-03 12:10:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger-labs/mirbft/issues/77" class=".btn">77</a>
            </td>
            <td>
                <b>
                    Improve epochFinished predicate in ISS.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span>
            </td>
            <td>
                Resolve this TODO: https://github.com/hyperledger-labs/mirbft/blob/150081aa1f48a695249ff974e6fab443dce3b24b/pkg/iss/iss.go#L521

The changes in the code should be rather straight-forward, but addressing this issue is a good opportunity to get to know the code.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-30 09:57:26 +0000 UTC
    </div>
</div>

