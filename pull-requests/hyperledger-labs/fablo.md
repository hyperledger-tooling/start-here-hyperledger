---
layout: default
title: fablo
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fablo
---

# fablo <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fablo){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/411" class=".btn">#411</a>
            </td>
            <td>
                <b>
                    Created support for chaincodes list command (with TLS)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Addressing issue #406 
This is the second implementation of `chaincodes list` command for **support TLS (test-02)** with the following changes:

- Added new function `peerChaincodeListTls()` to chaincode functions 
- Deleted `wait-for-chaincode-tls` script. `docker exec` is now handled within `peerChaincodeListTls()`
- Update CHANGELOG with the new feature
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-11 13:13:59 +0000 UTC
    </div>
</div>

