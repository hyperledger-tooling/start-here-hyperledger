---
layout: default
title: ursa
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/ursa
---

# ursa <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/ursa){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/ursa/pull/228" class=".btn">#228</a>
            </td>
            <td>
                <b>
                    make accum public
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is required for anoncreds-rs as we use a different name for the key, [spec](https://hyperledger.github.io/anoncreds-spec/#creating-the-initial-revocation-status-list-object). Making it public makes sure we can just rename it easily, but this does not create a breaking change.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-28 12:39:26 +0000 UTC
    </div>
</div>

