---
layout: default
title: firefly-transaction-manager
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-transaction-manager
---

# firefly-transaction-manager <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-transaction-manager){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/6" class=".btn">#6</a>
            </td>
            <td>
                <b>
                    Move ffcapi to firefly-common, and build config docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Moves over all dependences to `firefly-common` that are now there
- Deletes `ffcapi` now that is has moved
- Uses new `core` package for object definitions still in FireFly Core
- Moves the config prefix to `FF21` to give an extra digit (1000 rather than 100 total error msgs)
- Adds `config.md` auto-generation and link from `README.md`

Depends on (go.mod pulls these in directly):
- https://github.com/hyperledger/firefly-common/pull/4
- https://github.com/hyperledger/firefly/pull/791

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-05 01:33:19 +0000 UTC
    </div>
</div>

