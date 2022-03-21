---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/676" class=".btn">#676</a>
            </td>
            <td>
                <b>
                    feat: Replace old oob invitation with the new one
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I removed all use of `ConnectionInvitationMessage` inside the framework, it is used only in the conversion method from the "old" oob to the "new" one. And also in tests for unused methods, I would like to look at them if I can reuse some tests cases for the new methods.

I also refactored a bit mediation `provision` method by splitting making a connection and requesting mediation as we discussed on the call yesterday.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-17 11:46:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/675" class=".btn">#675</a>
            </td>
            <td>
                <b>
                    refactor(core): renamed BufferEncoder to TypedArrayEncoder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                BufferEncoder is incorrectly named as it accepts Uint8Arrays (and buffers). The name TypedArrayEncoder is more fitting as it fits both versions.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-15 14:00:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/674" class=".btn">#674</a>
            </td>
            <td>
                <b>
                    fix: remove deprecated multibase and multihash
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Removes the dependency on the deprecated `multibase` and `multihash` libraries. They were also using `TextDecoder` which does not work natively in React Native. The replacement library `multiformats` is focused on Node.JS environment so I've also removed it.

I've now added a subset of the functionality that those libraries offer natively to AFJ. This means fewer dependencies which is not a problem I guess. 

Fixes #673 
Fixes #662 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-14 12:24:59 +0000 UTC
    </div>
</div>

