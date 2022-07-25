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
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/363" class=".btn">#363</a>
            </td>
            <td>
                <b>
                    MockBackend: Remove context from subscription
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR includes a small update to the mock subscription. Storing a context in a struct is disadvised and not needed here as we can just rely on the functionality of the events channel.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-25 14:29:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/362" class=".btn">#362</a>
            </td>
            <td>
                <b>
                    Add Adjudicator Getter for Multi-Adjudicator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #361.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-25 09:25:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/360" class=".btn">#360</a>
            </td>
            <td>
                <b>
                    Fix local watcher deadlock
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In rare occasions, the local watcher was running into a deadlock when stopping and handling an event at the same time.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-19 21:22:16 +0000 UTC
    </div>
</div>

