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
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/353" class=".btn">#353</a>
            </td>
            <td>
                <b>
                    Handle update locked
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Our update handling logic allowed potentially left the channel state machine unlocked if not used correctly. Correct usage was neither documented, nor enforced. This PR proposes an update handling mechanism where the channel machine is only unlocked once the update handler is done.

Closes #270 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-24 10:23:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/351" class=".btn">#351</a>
            </td>
            <td>
                <b>
                    Remove settle secondary
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR removes the settle secondary logic. It was not well documented and rarely used, and lead to confusion. We can still implement the same functionality on the application level if necessary.

Closes #81 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-24 07:21:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/350" class=".btn">#350</a>
            </td>
            <td>
                <b>
                    Separate wire address
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #234.

In general, this PR will ensure that `wire.Address` and `wallet.Address` are distinct. Before, `wire.Address` was a synonym for `wallet.Address`, which caused some problems, in particular, mixing up `wire.Address` and `wallet.Address` and adding functionality to `wallet.Address` which was specific to the use case of `wire.Address` (concretely, the `Cmp` function).

In this PR we assign both their own type.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 07:49:31 +0000 UTC
    </div>
</div>

