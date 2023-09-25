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
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/413" class=".btn">#413</a>
            </td>
            <td>
                <b>
                    Implemented use of generators for chaincode invoke command with TLS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Addressing issue #390 to support invoke command with TLS and uses generators with the following changes:

- New function `peerChaincodeTls` is added to `chaincode-functions-v2.sh` that now handles `docker exec` command
- Removed `expect-invoke-cli-tls.sh` as its implementation is now handled in `expect-invoke-cli.sh` and `peerChaincodeTls` function 
- Test-02 now uses `expect-invoke-cli.sh` instead of `expect-invoke-cli-tls.sh`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-19 10:28:37 +0000 UTC
    </div>
</div>

