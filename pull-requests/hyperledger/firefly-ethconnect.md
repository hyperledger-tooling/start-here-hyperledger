---
layout: default
title: firefly-ethconnect
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-ethconnect
---

# firefly-ethconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-ethconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/230" class=".btn">#230</a>
            </td>
            <td>
                <b>
                    Move ABI/Contract store to LevelDB from flat files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In the case where you deploy many contracts (hundreds of thousands for example), the flat file based store of contract ABIs/registrations becomes inefficient. This affects startup time and memory usage.

This PR is to make this storage consistent with elsewhere in the codebase, and use LevelDB rather than flat files.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-30 22:06:59 +0000 UTC
    </div>
</div>

