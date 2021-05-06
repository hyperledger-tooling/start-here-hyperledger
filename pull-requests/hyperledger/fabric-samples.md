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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/444" class=".btn">#444</a>
            </td>
            <td>
                <b>
                    Disable Go pprof profiling in test network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Peers and Orderers by default disable Go pprof profiling, however test
network was enabling pprof in peers by default. As a good practice,
pprof should be disabled by default and only enabled when needed
for debug profiling.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-30 11:46:22 +0000 UTC
    </div>
</div>

