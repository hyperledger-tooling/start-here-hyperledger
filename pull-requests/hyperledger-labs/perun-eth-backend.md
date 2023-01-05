---
layout: default
title: perun-eth-backend
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/perun-eth-backend
---

# perun-eth-backend <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/perun-eth-backend){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-eth-backend/pull/36" class=".btn">#36</a>
            </td>
            <td>
                <b>
                    Fix `Asset.UnmarshallBinary` not working
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - The method did not have a pointer receiver and thus could not set the value, resulting in the previous (default) value instead of the just unmarshalled one.
- Additionally, the order was different from `Asset.MarshallBinary`, which meant unmarshalling a value just marshalled would result in the wrong value or an error.

The added test coveres both these cases.

Signed-off-by: Jens Winkle <jens@perun.network>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-05 14:58:56 +0000 UTC
    </div>
</div>

