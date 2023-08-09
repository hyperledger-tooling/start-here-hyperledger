---
layout: default
title: sawtooth-lib
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/sawtooth-lib
---

# sawtooth-lib <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/sawtooth-lib){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/174" class=".btn">#174</a>
            </td>
            <td>
                <b>
                    Move transact::protocol::* to protocol::*
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an incremental step toward integrating transact fully into libsawtooth. This removes the transact feature guard on these protocol structs, with the exception of receipt; receipt needs further refactoring so that it does not reference non-protocol code.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-09 17:04:30 +0000 UTC
    </div>
</div>

