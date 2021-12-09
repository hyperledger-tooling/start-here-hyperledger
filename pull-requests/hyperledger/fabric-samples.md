---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/553" class=".btn">#553</a>
            </td>
            <td>
                <b>
                    Updates to asset-transfer-basic Gateway sample to align with docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also fix linting:

- Install goimports globally to run the linting check rather than installing to each gomodule, which was causing dependency conflicts.
- Tidy all go.mod and go.sum files.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 17:45:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/552" class=".btn">#552</a>
            </td>
            <td>
                <b>
                    Fixed configtxlator permission error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: sapthasurendran <saptha.surendran@ibm.com>

Fixed  issue  `configtxlator: error: open /dev/stdout: permission denied, try --help` found  while setting up test-network




            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 08:06:47 +0000 UTC
    </div>
</div>

