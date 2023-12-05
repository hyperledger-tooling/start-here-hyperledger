---
layout: default
title: fabric-private-chaincode
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-private-chaincode
---

# fabric-private-chaincode <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-private-chaincode){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/748" class=".btn">#748</a>
            </td>
            <td>
                <b>
                    Fix testing on non-Intel CPU
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">urgent</span><span class="chip">Test</span>
            </td>
            <td>
                This PR upgrades the SGX SDK and SSL packages and enables the SKIP_INTELCPU_CHECK flag.
SGX SSL aborts when it's not used on Intel CPUs, even in SIM mode.
However, more recent versions (which require an SDK upgrade) allow to build the package by excluding that check.
Additionally, the PR enables SGX SSL tests to spot these issues early on, since these are only executed when the docker containers need to be rebuilt.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-05 03:56:11 +0000 UTC
    </div>
</div>

