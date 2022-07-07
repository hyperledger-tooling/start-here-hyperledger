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
                PR <a href="https://github.com/hyperledger/caliper-benchmarks/pull/218" class=".btn">#218</a>
            </td>
            <td>
                <b>
                    readWrite chaincode and benchmark fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                    - read-write asset tx and benchmark
        - chaincode
            - fixed asset and fixed asset base node
                - deleteAssetFromBatch
                    - delete console.log inside for loop
                    - take out curlies
                - readWriteAsset
                    - update function to new code
            - fixed asset and fixed asset base go
                - readWriteAsset
                    - update function to new code and remove unsafe import
                    - remove brackets
                - deleteasset and delte assetsfrombatch
                    - change uuid to key 
                    - delete log in side the for loop in deleteFromBatch
                    - change delete asset and delte assetfrom bach log 
        - workload
            - change default case for switch , no curly braces beause it is in a single line
            - change from JSON.stringify(letter) to just letter
            - delete comments  
            - change keys for writeOptions to match options of benchamark, hten update switch for new keys
        - fix benchmark previoslyRead variable for random round to writeOptions
        - fix delete preloaded asset benchmark

Signed-off-by: fraVlaca <ocsenarf@outlook.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-07 15:17:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper-benchmarks/pull/217" class=".btn">#217</a>
            </td>
            <td>
                <b>
                    fixed 'bytes' issue in helper.js
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: fraVlaca <ocsenarf@outlook.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-07 13:25:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper-benchmarks/pull/214" class=".btn">#214</a>
            </td>
            <td>
                <b>
                    Update docs to include use of the new fabric gateway connector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #156 

Signed-off-by: fraVlaca <ocsenarf@outlook.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-05 10:05:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper-benchmarks/pull/212" class=".btn">#212</a>
            </td>
            <td>
                <b>
                    Remove type: local from the various benchmark files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #194 

Signed-off-by: fraVlaca <ocsenarf@outlook.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-01 14:43:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper-benchmarks/pull/210" class=".btn">#210</a>
            </td>
            <td>
                <b>
                    added readWriteTx benchmark + readWrite tx in node cc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fabric fixed-asset benchmark and cc tx
- created new benchmark for readwrite composte tx.and added itto test.yaml
- added readwrite tx to node fixed asset and fixed-asset-base chaincodes

Closes #201 
Signed-off-by: fraVlaca <ocsenarf@outlook.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-01 10:52:44 +0000 UTC
    </div>
</div>

