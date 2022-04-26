---
layout: default
title: caliper-benchmarks
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/caliper-benchmarks
---

# caliper-benchmarks <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/caliper-benchmarks){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper-benchmarks/pull/193" class=".btn">#193</a>
            </td>
            <td>
                <b>
                    Updated and fixed marbles/drm/simple/smallbank go chaincodes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - deleted drm directory
- Updated all the other go chaincode in marbles/go, marbles-norichquery/go, simple/go, smallbank/go
change (run go mod init, go mod tidy, go mod vendor and subbed "github.com/hyperledger/fabric/core/chaincode/shim /n pb "github.com/hyperledger/fabric/protos/peer" with "github.com/hyperledger/fabric-chaincode-go/shim /n pb "github.com/hyperledger/fabric-protos-go/peer")

Closes #155 

Signed-off-by: fraVlaca <ocsenarf@outlook.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-26 10:56:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper-benchmarks/pull/192" class=".btn">#192</a>
            </td>
            <td>
                <b>
                    Fixed and reorganized fixed-asset-base and fixed-asset benchmarks and workloads
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - deleted sample.sh
- deleted api/fabric/base directory and move the files in contract into the api/fabric directory
- renamed lib to workloads
- updated the newly moved benchmarks in api/fabric to the changed location for the workload files
- updated the README.md in networks/fabric to point to the new location for the benchmark files

Closes #163 

Signed-off-by: fraVlaca <ocsenarf@outlook.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-26 09:48:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper-benchmarks/pull/191" class=".btn">#191</a>
            </td>
            <td>
                <b>
                    Chaincode fixes: added collections config to support private data + replaced console.err/error with console.log 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Closes #190  

- Closes #185 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 14:32:32 +0000 UTC
    </div>
</div>

