---
layout: default
title: sawtooth-sdk-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/sawtooth-sdk-go
---

# sawtooth-sdk-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/sawtooth-sdk-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-sdk-go/pull/46" class=".btn">#46</a>
            </td>
            <td>
                <b>
                    Resolve build errors  and upgrade golang
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Current build errors are results of problems between the current example dependencies and an out of date golang versions.  This updates the golang version to 1.13 as well as the following

1. Updates the satori/go.uuid version to the latest recommended - which resolves among a few other things, an important issue https://github.com/satori/go.uuid/issues/73
2. Possibly controversially removes the xenial dockerfiles since a) they don't easily support golang-1.13, and b) they no longer appear to be referenced anywhere.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-21 14:44:58 +0000 UTC
    </div>
</div>

