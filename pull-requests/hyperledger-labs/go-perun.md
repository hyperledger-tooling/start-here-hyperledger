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
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/330" class=".btn">#330</a>
            </td>
            <td>
                <b>
                    JSON Marshaling of channel.State and Params
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - sim/wallet: Add Address JSON Marshaling
- channel: Add Params, State, Allocation JSON Marshaling

For now, only `States` and `Params` without `App` and `Data` are supported.

While using any particular backend, the implementations of `Asset` and `Address` must be JSON marshalable.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-24 14:16:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/328" class=".btn">#328</a>
            </td>
            <td>
                <b>
                    Release 0.9.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-23 12:24:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/327" class=".btn">#327</a>
            </td>
            <td>
                <b>
                    Wire hybrid bus
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Enables perun-network/perun-websocket-backend#2.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-22 14:25:05 +0000 UTC
    </div>
</div>

