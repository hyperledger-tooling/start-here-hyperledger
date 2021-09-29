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
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/230" class=".btn">#230</a>
            </td>
            <td>
                <b>
                    [README] Add read-the-docs badge.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #229 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 11:56:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/228" class=".btn">#228</a>
            </td>
            <td>
                <b>
                    backend/eth/channel: Fix state app decoding
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Function `FromEthState` did not set the App correctly on a decoded state.

Relates to #226 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-27 20:32:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/227" class=".btn">#227</a>
            </td>
            <td>
                <b>
                    Options to ignore the App + Assets in generic tests.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds `IgnoreApp` and `IgnoreAssets` options to make the `[channel] GenericBackendTest` work with the polkadot backend.

Closes #170 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-27 14:15:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/225" class=".btn">#225</a>
            </td>
            <td>
                <b>
                    Revise generic wallet tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #224 

Depends on #223 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-23 13:32:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/223" class=".btn">#223</a>
            </td>
            <td>
                <b>
                    Extend generic channel tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #219 

Package channel: Adds generic tests for testing funder, adjudicator, and subscription implementation.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-23 12:15:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/222" class=".btn">#222</a>
            </td>
            <td>
                <b>
                    Upgrade go to v1.17
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #221

With go v1.17 the build tag format changes from `+build` to `go:build`.

Also resolves some issues with files using build tags:
- build tag wrap_test was unused and documented as broken
- files race.go and norace.go were using build tags to detect the race flag, but were unused
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-23 11:34:39 +0000 UTC
    </div>
</div>

