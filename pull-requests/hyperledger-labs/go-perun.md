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
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/119" class=".btn">#119</a>
            </td>
            <td>
                <b>
                    Prep82 update bindings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Split some more commits from #83 .

In particular, this PR includes the following:
- Update contract bindings
- Adopt channel data types
- registerRecursive
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-22 15:46:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/117" class=".btn">#117</a>
            </td>
            <td>
                <b>
                    Integrate Resistant Event Subs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Uses resistant event confirmation on *go-perun* in all locations.  
Currently i am having trouble with the `AdjudicatorSub`, which seems to make some end-to-end tests fail.  
Funder and Adjudicator tests themselves seem to work.

Closes #85 
Draft until #40 and #97 are closed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-18 15:50:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/116" class=".btn">#116</a>
            </td>
            <td>
                <b>
                    Resistant event subs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds the `ResistantEventSub` type.  
Also introduced a convenience function `Subscribe(ctx context.Context, cr ethereum.ChainReader, contract *bind.BoundContract, eFact EventFactory, startBlockOffset, confirmations uint64) (*ResistantEventSub, error)` which makes it easier to create a resistant sub.  
I am not happy with the arguments of `Subscribe` yet, since it are so many.

Closes #40 
Draft until #105 is closed
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-18 15:44:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/114" class=".btn">#114</a>
            </td>
            <td>
                <b>
                    Prepare 82 virtual channels
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Splitting some commits from #83 .
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-18 12:42:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/112" class=".btn">#112</a>
            </td>
            <td>
                <b>
                    :sparkles: [pkg/test] Add context to ConcurrentT.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ConcurrentT can now be constructed with an optional context which will cause all stages and waiting operations to fail on expiry.
I diverged from the issue's initial plan, because introducing custom contexts would have made the ConcurrentT object harder to use correctly. Now, there is only one context per ConcurrentT, and not one per wait call. The only adaption needed to use the new feature is to swap out the ConcurrentT's constructor in tests.

Closes #110.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-16 23:45:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/111" class=".btn">#111</a>
            </td>
            <td>
                <b>
                    :boom: [backend/eth/channel] Remove validation of adj in validateAssettHolder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Contract code at adjudicator address is not validated because, the
  it is passed by the caller, hence it is the responsibility of the
  caller to provide a valid address.

Resolves #109.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-16 12:44:17 +0000 UTC
    </div>
</div>

