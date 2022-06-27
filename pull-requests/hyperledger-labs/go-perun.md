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
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/355" class=".btn">#355</a>
            </td>
            <td>
                <b>
                    Abstract multiledger test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Makes the multi-ledger test abstract so that it can be reused in other backends.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-27 12:25:33 +0000 UTC
    </div>
</div>

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

