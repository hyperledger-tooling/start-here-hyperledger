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
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/7" class=".btn">#7</a>
            </td>
            <td>
                <b>
                    Refactor FFCAPI to a local API interace, and FFTM to a utility package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is quite a big change.

- Removes the Docker build from this package - this means the existing builds will stay for those using them
- Reinstates the FFCAPI definition here, which was recently moved to FF common, and now removed in https://github.com/hyperledger/firefly-common/pull/15
- Refactors the FFCAPI to be a local interface, rather than remote
   - This is because it's just too complex to having the potential of state mismatch in event state between the FFCAPI and the FFTM, and build a clean interface
 - Removes the `fftm` and `cmd` directories
 - Moves the `internal/manager` to be `pkg/fftm` for use by FFCAPI connectors
   - They will inject their implementation into the `fftm.Manager` to start their server
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-02 02:56:14 +0000 UTC
    </div>
</div>

