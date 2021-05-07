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
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/71" class=".btn">#71</a>
            </td>
            <td>
                <b>
                    :sparkles: [channel] Improve Allocation handling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                One step towards making it more convenient to work with `Allocation`.

Closes #63 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-07 13:45:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/70" class=".btn">#70</a>
            </td>
            <td>
                <b>
                    Check for nil parts in ValidateParams.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                Closes #69 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-07 10:10:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/66" class=".btn">#66</a>
            </td>
            <td>
                <b>
                    Enable logging per default
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Enable default logging with level 'Warning' to increase usability.
Closes #64
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-05 08:42:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/61" class=".btn">#61</a>
            </td>
            <td>
                <b>
                    :lock: [client] Verify state signatures for subchannel funding and se…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …ttlement updates

We are intercepting updates for subchannel funding and settlement. However,
we did not check the signatures for these updates. This is fixed now.

Signed-off-by: Matthias Geihs <matthias@perun.network>

Closes #57 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 15:18:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/60" class=".btn">#60</a>
            </td>
            <td>
                <b>
                    :lock: [channel] Check ID after decoding parameters
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When deserializing parameters, it must be checked whether the ID is
correct. Otherwise we might end up with an inconsistent Params object.

Signed-off-by: Matthias Geihs <matthias@perun.network>

Closes #56 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 15:08:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/59" class=".btn">#59</a>
            </td>
            <td>
                <b>
                    :bug: [channel/machine, client] Sub-channel withdrawal without regist…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …ering

The current implementation required a sub-channel to be registered on-chain before it could be withdrawn.
However, in the optimistic case, a sub-channel should be withdrawable into its parent channel without
blockchain interaction. We achieve this by modifying the state machine to allow for a transition from
phase final to phase withdrawing.

Signed-off-by: Matthias Geihs <matthias@perun.network>

Closes #58 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 14:48:17 +0000 UTC
    </div>
</div>

