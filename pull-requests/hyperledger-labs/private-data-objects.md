---
layout: default
title: private-data-objects
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/private-data-objects
---

# private-data-objects <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/private-data-objects){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/360" class=".btn">#360</a>
            </td>
            <td>
                <b>
                    Fix build bug in pservice in ubuntu20.04
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                This PR fixes a bug that was causing the pservice build to fail on ubuntu 20.04 machines due to a consistently reproducible race condition between cmake and make expecting enclave_u.c to exist before it was generated. This bug does not occur on ubuntu 18.04 or earlier.

Signed-off-by: Marcela Melara <marcela.melara@intel.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-15 23:59:39 +0000 UTC
    </div>
</div>

