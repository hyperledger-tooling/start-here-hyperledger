---
layout: default
title: go-perun
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/go-perun
---

# go-perun <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/go-perun){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/400" class=".btn">#400</a>
            </td>
            <td>
                <b>
                    Revert: Remove settle secondary (#351)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is linked to https://github.com/hyperledger-labs/perun-eth-backend/pull/47 and reverts commit https://github.com/hyperledger-labs/go-perun/commit/be6e07257c123309c98fbbea4b86440275be2797.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-20 13:35:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/399" class=".btn">#399</a>
            </td>
            <td>
                <b>
                    #395_Fix_Falling_Unit_Tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description
This PR serves to fix the #395 issue of failing unit tests. 

### App Randomizer Internal Test 
Location: `channel/test/app_randomizer_internal_test.go`

Cause: The issue stems from the lack of Comparator (`Equal`) for MockAppRandomizer. This leads to the test not recognizing that the default appRandomizer has already been set in the internal test.

Solution: Add an identifier to the MockAppRandomizer to compare the old and new appRandomizer.

### Dialer Internal Test
Location: (`wire/net/simple/dialer_internal_test.go`)

Cause: Like @RmbRT has pointed out, there is a race between the init of `wire/simple` and `backend/sim/wire`, which set the RandomAddress and RandomAccount functions to be used in the internal tests.

Solution: Add the initialization of `NewRandomAddress` and `NewRandomAccount` to use the implementation from the `wire/simple`.

Alternative: Remove `init()` of `wire/simple` and only use the init of `backend/sim/wire`. This also results in passing internal tests but might cause issues for packages using `wire/simple` (need further investigation).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-19 14:51:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/397" class=".btn">#397</a>
            </td>
            <td>
                <b>
                    Egoistic funding
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description:
This PR builds upon the changes introduced in https://github.com/hyperledger-labs/perun-eth-backend/pull/45 by extending egoistic funding to cross-chain swaps in the eth-backend.

In this update, we introduce a map for each chain, designating whether a chain is considered egoistic or not. This distinction is crucial in determining the funding order for different chains, ensuring that egoistic chains are funded last.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-15 09:19:01 +0000 UTC
    </div>
</div>

